# Building med

This project uses the D programming language and the DUB package manager.

## Prerequisites

You will need a D compiler (DMD) and the DUB package manager. The recommended version is DMD 2.111.0 or later.

### On Debian/Ubuntu

You can install DMD and DUB using the `d-apt` repository.

1.  **Add the d-apt repository:**
    ```sh
    sudo wget https://netcologne.dl.sourceforge.net/project/d-apt/files/d-apt.list -O /etc/apt/sources.list.d/d-apt.list
    ```

2.  **Install the keyring and update:**
    ```sh
    sudo apt-get update --allow-insecure-repositories
    sudo apt-get -y --allow-unauthenticated install --reinstall d-apt-keyring
    sudo apt-get update
    ```

3.  **Install the compiler and dub:**
    ```sh
    sudo apt-get install -y dmd-compiler dub
    ```

### Other Systems

For other systems, please refer to the official D language download page: <https://dlang.org/download.html>

## Building

Once you have the prerequisites installed, you can build the project by running the following command in the root of the repository:

```sh
dub build
```

The compiled executable will be placed in the `bin/` directory.
