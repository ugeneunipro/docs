---
title: "Installation on Linux"
weight: 400
---


# Installation on Linux

The following UGENE package delivery types are available on 64-bit Linux:

*   **Online installer:** updates to new versions are supported
*   **TAR.GZ archive:** does not require Internet connection to be installed

Other packages for older UGENE version are available on the web page [http://ugene.net/download-all.html](http://ugene.net/download-all.html).

### Attention: **O**nline installer has been removed from UGENE since version 39.0.

### Installation using online installer

*   Download an archive with the online installer file ("ugeneInstaller\_64bit.tar").
*   Unpack the archive.
*   Run the extracted "ugeneInstaller\_64bit" executable file.

    cd ~/Downloads
    tar -xf ugeneInstaller\_64bit.tar
    ./ugeneInstaller\_64bit

*   Follow the installation wizard.


![](/images/65929248/65929249.png)

On a new UGENE version release, a notification will appear with an option to update the package.

### Installation using TAR.GZ archive

*   Download the TAR.GZ archive.

*   Unpack the archive - in the Terminal run "tar -xzf _archive\_file_".
*   From the unpacked folder run "./ugeneui" (here "ui" states for "User Interface"). For example:

    cd ~/Downloads
    tar -xzf ugene-current-version-x86-64.tar.gz
    cd ugene-current-version
    ./ugeneui


On a new UGENE version release, a notification will appear. However, to install the new version, it is required to manually download the package again.
