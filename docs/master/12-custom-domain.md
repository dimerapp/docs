---
permalink: custom-domain
category: root
---

# Custom domain
Dimer let you map a custom domain to your subdomain. In this guide we learn how to create a `Cname` entry with your DNS provider and then tell dimer about the same.

#### General steps
1. If you already don't have a domain, buy one with a domain registration service.
2. Add the [custom domain](#custom-domain) to your config file.
3. Update your [DNS provider](#update-dns-provider) to point to the dimer subdomain.
4. Test that is works. There maybe some delay while DNS changes are reflected.

## Custom domain
The custom domain is defined inside the config file `dimer.json`. Make sure to not include `http` or `https`, it should just be the hostname.

```json
{
  "cname": "adonisjs.com"
}
```

## Update DNS provider
Next step is add a `CNAME` with your DNS provider, which points to the subdomain of your website.

| Name | Value |
|------|--------|
| `custom-domain` | [subdomain].dimerapp.com |
