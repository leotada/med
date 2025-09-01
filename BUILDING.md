# Building med

This project uses the D programming language and the DUB package manager.

## Prerequisites

You will need a D compiler (DMD) and the DUB package manager. The recommended version is DMD 2.111.0 or later.

### On Debian/Ubuntu

If you have the DMD `.deb` package, you can install it using `dpkg`. For example:

```sh
sudo dpkg -i dmd_2.111.0-0_amd64.deb
```

If you encounter any dependency issues after installation, run the following command to fix them:

```sh
sudo apt-get install -f
```

### Other Systems

For other systems, please refer to the official D language download page: <https://dlang.org/download.html>

## Building

Once you have the prerequisites installed, you can build the project by running the following command in the root of the repository:

```sh
dub build
```

The compiled executable will be placed in the `bin/` directory.
