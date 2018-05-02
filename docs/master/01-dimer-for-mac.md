---
permalink: dimer-for-mac
category: root
---

# Dimer for Mac

During beta, we have released command line binaries for every major operating system, including Mac. You don't have to be super technical in order to use the CLI, but being familiar with the command line is important.

Head over to your dashboard [https://dimerapp.com/dashboard](https://dimerapp.com/dashboard) and click `Mac OS X` button. It will download the file with `.sh` extension.

Assuming you downloaded the file inside the `~/Downloads` directory, let's get into the same directory by running the following command.

```bash
cd ~/Downloads

pwd
# /Users/<your-name>/Downloads
```

The downloaded file is a binary, we need to run it as follows.

```bash
sh ./dimer-for-mac.sh

# Output
# Verifying archive integrity...  100%   All good.
# Uncompressing Dimer mac  100%
```

Once done! You will be able to execute commands by running `dimer` from your command line.

```bash
dimer
```

If you can see the following output on your terminal, then you have successfully installed **Dimer for Mac.**

![](http://res.cloudinary.com/adonisjs/image/upload/q_100/v1525059195/dimer-help_gwctqj.png)

Run the following command to check the CLI version.

```bash
dimer --version
```

## Useful links

- [Getting started with dimer](getting-started)
