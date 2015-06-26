#SJWCoin [SJW]



SJWCoin is an open source peer-to-peer crytocurrency.
#Cause Cancer..
<img src="http://postox.com/images/2015/06/17/splash.png" /> 

#What is SJWCoin?  

SJWCoin is like Bitcoin, and based on FooCoin, which was a clone of TacoCoin. It is a scrypt based cryptocurrency.
I picked TacoCoin because of them being pioneers in scrypt merge mining (as far as I can tell) and this coin will sure as the fuck need
that to get any sort of traction because who the fuck really needs yet another coin?  really..

#Why SJWCoin?

Cause why the fuck not, I say.  Or ask?  It does kind of look like a question.  You fucking decide.

#What's broken?

Probably lots of shit... you find it!!
<br />
https://www.dropbox.com/ is not where it is at
<br />
#SJWcoin-Qt on Ubuntu 14.04
<img src="http://postox.com/images/2015/06/17/linux_qt_wallet_FOR-SOCIAL-JUSTICE.png" />
#SJWcoin-Qt on Winders 8.1
<img src="http://postox.com/images/2015/06/18/windows_8_1_qt_wallet.png" />
<br />
This is a giant pain in the ass to roll on winders
<br />
Follow this guide. https://bitcointalk.org/index.php?topic=149479.0<br />
Steps 1 all the way to 2.7 (use a newer openssl..  it's at 1.1o now)<br />
then compile leveldb (msys shell)<br />
```
cd /C/bitcoin-0.8.6/src/leveldb
TARGET_OS=NATIVE_WINDOWS make libleveldb.a libmemenv.a
```
then it's time to make it (windows CMD prompt, make sure QT \bin is in your %PATH% and the VAR PATHS are right in the .pro)<br />
```
qmake "USE_QRCODE=1" "USE_UPNP=-" "USE_IPV6=-" sjwcoin-qt.pro
mingw32-make -f Makefile.Release
```
And It'll end up in the Releases folder
<br />
For linux qt building
```
sudo apt-get install build-essential libssl-dev libboost-all-dev
sudo apt-get install libtool autotools-dev autoconf pkg-config libssl-dev
apt-cache search libminiupnpc
sudo apt-get install libminiupnpc-dev
sudo add-apt-repository ppa:bitcoin/bitcoin
sudo apt-get update
sudo apt-get install libdb4.8-dev libdb4.8++-dev
sudo apt-get install qt5-qmake libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev-tools
 
sudo apt-get install qt5-qmake
sudo apt-get install qt-sdk
 
git clone https://github.com/sjwcoin/sjwcoin
```
Comment out the windows LIB PATHs
nano sjwcoin-qt.pro 

#BOOST_LIB_SUFFIX=-mgw49-mt-s-1_57
#BOOST_INCLUDE_PATH=C:/deps2/boost_1_57_0
#BOOST_LIB_PATH=C:/deps2/boost_1_57_0/stage/lib
#BDB_INCLUDE_PATH=C:/deps2/db-4.8.30.NC/build_unix
#BDB_LIB_PATH=C:/deps2/db-4.8.30.NC/build_unix
#OPENSSL_INCLUDE_PATH=C:/deps2/openssl-1.0.1o/include
#OPENSSL_LIB_PATH=C:/deps2/openssl-1.0.1o
#MINIUPNPC_INCLUDE_PATH=C:/deps2/
#MINIUPNPC_LIB_PATH=C:/deps2/miniupnpc
#QRENCODE_INCLUDE_PATH=C:/deps2/qrencode-3.4.4
#QRENCODE_LIB_PATH=C:/deps2/qrencode-3.4.4/.libs
```
then build it.
```
qmake
make
```
in that same directory you will find sjwcoin-qt


#Where can you find us?

website: http://sjwcoin.com<br />
Reddit: https://voat.co/v/fatpeoplehate<br />  
Freenode: #sjwcoin
