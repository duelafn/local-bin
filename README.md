
LOCAL-BIN
=========

Various scripts and utilities that I've written.

Released under the CC-BY License.



DEPENDENCIES
============

- Dean::Util  (http://dean.serenevy.net/code/projects/Dean::Util)
- Path::Class



Debian/Ubuntu Packages
----------------------

The following steps will install debian/Ubuntu packages used by these
scripts and Dean::Util.

Add my Debian Repository to your sources.list:

    echo "deb http://serenevy.net/debian bullseye main" | sudo tee /etc/apt/sources.list.d/dean-serenevy.list

Load my public-key into apt:

    # pub   4096R/0xE4E6033FE5D0AA3A 2013-11-21
    #       Key fingerprint = 3A4D 51DF 68FC D20B FC0C  1C5F E4E6 033F E5D0 AA3A
    # uid                 [ultimate] Dean Serenevy <dean@serenevy.net>
    wget https://dean.serenevy.net/about/gpg/dean_serenevy-public_key-2013-11-21.gpg
    sudo mv dean_serenevy-public_key-2013-11-21.gpg /etc/apt/trusted.gpg.d/

Install dependencies (and some packages suggested by Dean::Util)

    sudo apt-get update
    sudo apt-get install libdate-manip-perl libdatetime-perl libdean-util-perl libfile-chdir-perl libpath-class-perl libperlio-gzip-perl libterm-readkey-perl libwww-perl libxml-libxml-perl libyaml-perl
