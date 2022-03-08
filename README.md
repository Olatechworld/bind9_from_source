# bind9_from_source
Install from source

Installation of bind 9.16 > from source
first install Library libcrypto, libssl • libuv-dev• perl • pkg-config / pkgconfig / pkgconf,libnhttps2-dev, perl, libcap-dev
After to install Library, go to site bind9 to get the version that you need, In my case I will install bind9.18

Step1 :
Download the source
wget https://downloads.isc.org/isc/bind9/9.18.0/bind-9.18.0.tar.xz

step2:
untar your source with command
tar -xvf bind-9.18.0

Step3
Go in folder bind9.18.0, run a commands
./configure (after ./configure to run, i fou are see error) fix error, generally it is need to download package
If you are need to install a other packages, please see the documentation of administrator in the link https://downloads.isc.org/isc/bind9/9.18.0/doc/arm/Bv9ARM.pdf
Note: the dfault configuration is store in folder /usr/local(/usr/loca/etc), but if you want to change the directory of the configuration run the command
./configure --prefix /usr/local
