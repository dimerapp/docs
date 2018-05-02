---
permalink: dimer-for-linux
category: root
---

# Dimer for Linux

During beta, we have released command line binaries for every major operating system, including Linux. Being a Linux user you must be pretty comfortable with the command line.

Head over to your dashboard [https://dimerapp.com/dashboard](https://dimerapp.com/dashboard) and click `Linux` button. It will download the file with `.sh` extension.

Assuming you downloaded the file inside the `~/Downloads` directory, let's get into the same directory by running the following command.

```bash
cd ~/Downloads

pwd
# /Users/<your-name>/Downloads
```

The downloaded file is a binary, we need to run it as follows.

```bash
sh ./dimer-for-linux.sh

# Output
# Verifying archive integrity...  100%   All good.
# Uncompressing Dimer linux  100%
```

Once done! You will be able to execute commands by running `dimer` from your command line.

```bash
dimer
```

If you can see the following output on your terminal, then you have successfully installed **Dimer for Linux.**

![](http://res.cloudinary.com/adonisjs/image/upload/q_100/v1525059195/dimer-help_gwctqj.png)

Run the following command to check the CLI version.

```bash
dimer --version
```

## Useful links

- [Getting started with dimer](getting-started)
