---
title: "Installation on Linux"
weight: 400
---

# Installation on Linux

The following UGENE package delivery types are available on 64-bit Linux:

*   **Online installer:** updates to new versions are supported.
*   **TAR.GZ archive:** does not require an Internet connection to be installed.

Other packages for older UGENE versions are available on the webpage [http://ugene.net/download-all.html](http://ugene.net/download-all.html).

### Attention: The online installer has been removed from UGENE since version 39.0.

### Installation using the online installer

1. Download an archive with the online installer file ("ugeneInstaller\_64bit.tar").
2. Unpack the archive.
3. Run the extracted "ugeneInstaller\_64bit" executable file.

    ```bash
    cd ~/Downloads
    tar -xf ugeneInstaller_64bit.tar
    ./ugeneInstaller_64bit
    ```

4. Follow the installation wizard.

![UGENE Installation Screenshot](/images/65929248/65929249.png)

Upon the release of a new UGENE version, a notification will appear with an option to update the package.

### Installation using TAR.GZ archive

1. Download the TAR.GZ archive.
2. Unpack the archive - in the Terminal run: 

    ```bash
    tar -xzf archive_file
    ```

3. From the unpacked folder, run `./ugeneui` (here "ui" stands for "User Interface"). For example:

    ```bash
    cd ~/Downloads
    tar -xzf ugene-current-version-x86-64.tar.gz
    cd ugene-current-version
    ./ugeneui
    ```

Upon the release of a new UGENE version, a notification will appear. However, to install the new version, it is required to manually download the package again.