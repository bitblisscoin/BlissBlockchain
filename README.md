BitBlissCoin 
===========================
BitBlissCoin (BIBC) is a PoS + PoW based altcoin.

**Algorithm :**	Scrypt  
**Type :** PoW/PoS  
**Coin name :** bitblisscoin  
**Coin abbreviation :**	BIBC  
**Address letter :**	A  
**RPC port :**	26306  
**P2P port :**	26305  
**Block reward :**	55 coins  
  
## Mine a Block
Open your wallet, and make sure you are connected to another wallet.<br/>
The message "No block source available" will disappear once you mine your first block. <br/>
Close your wallet and create the file mycoin.conf in the folder "%APPDATA%\mycoin\".

<b>Important: replace "mycoin" with the name of your coin.</b>

```
rpcuser=rpc_user
rpcpassword=rpc_password
rpcallowip=127.0.0.1
listen=1
server=1
```

Download the latest version of cpuminer<a href="https://bitcointalk.org/index.php?topic=55038.0"></a> from here and extract the zip file.<br/>
Create a .bat file named mine.bat and paste the following text into mine.bat.
```
minerd --url=http://127.0.0.1:RPC_port --userpass=rpc_user:rpc_password
```
Save the file inside the extracted cpuminer folder.<br/>
Open your wallet and execute mine.bat to start mining your first coins.
