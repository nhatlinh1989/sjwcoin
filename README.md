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
then it's time to make it (windows CMD prompt, make sure QT \bin is in your %PATH%)<br />
```
qmake "USE_QRCODE=1" "USE_UPNP=-" "USE_IPV6=-" sjwcoin-qt.pro
mingw32-make -f Makefile.Release
```
And It'll end up in the Releases folder
<br />
Also, put this shit in your .conf until I can be assed to add it as a seed
```
addnode=71.185.213.22
```
#Where can you find us?

website: https://github.com/sjwcoin/sjwcoin<br />
Reddit: https://voat.co/v/fatpeoplehate<br />  
Freenode: ##hashhashnumbernumberpoundpoundsharpsharp <-- i like this so it stays
