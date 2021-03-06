squid-ubuntu
============

> Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator. It runs on most available operating systems, including Windows and is licensed under the GNU GPL.
> <cite> <http://www.squid-cache.org>

This project provides scripts needed to recompile the latest Squid 3.5.19 on Ubuntu 14.04 LTS with support for HTTPS filtering and SSL inspection. These scripts are used in web filtering appliance Web Safety available for VMWare ESXi at http://quintolabs.com/virtual.php. The compiled debian packages for eCap and Squid 3.5.19 are available at ubuntu.diladele.com repository.

**How to Use the Repository at ubuntu.diladele.com**
----------------------------------------------------

If you are installing Squid 3.5.19 for the first time run the following commands:

    # add repo
    echo "deb http://ubuntu.diladele.com/ubuntu/ trusty main" > /etc/apt/sources.list.d/ubuntu.diladele.com.list

    # update the apt cache
    apt-get update

    # install 
    apt-get install libecap3
    apt-get install squid-common
    apt-get install squid 
    apt-get install squidclient

If you have installed previous version 3.5.15 from this repo then please run "sudo apt-get update && sudo apt-get upgrade".  Please also check that your current squid.conf file from previous version is not overwritten. 

**Help**
--------

All questions/comments and suggestions are welcome at support@diladele.com or in squid mailing list http://www.squid-cache.org/Support/mailing-lists.html. Squid documentation can be found at http://www.squid-cache.org

**Contribution guidelines**
---------------------------
Please contact support@diladele.com

**Credits**
-----------
We admire people working on Squid Cache server, who spend their time free of charge and deliver great product to all of us.