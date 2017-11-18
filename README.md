BitBlissCoin 
===========================
BitBlissCoin (BIBC) is a PoS + PoW based altcoin.
<table>
<tr>
  <th>Algorithm </th>
  <td>Scrypt </td>  
</tr>
  <tr>
  <th>Type </th>
  <td>POW+POS </td>  
</tr>
  <tr>
  <th>Coin Name </th>
  <td>BitBlissCoin </td>  
</tr>
  <tr>
  <th>Abbreviation </th>
  <td>BIBC </td>  
</tr>
  <tr>
  <th>P2P Port </th>
  <td>26305 </td>  
</tr>
  <tr>
  <th>RPC Port </th>
  <td>26306 </td>  
</tr>
  <tr>
  <th>Block Reward </th>
  <td>55 Coins </td>  
</tr>  
 </table>
  
## Mine a Block
Open your wallet, and make sure you are connected to another wallet.<br/>
The message "No block source available" will disappear once you mine your first block. <br/>
Close your wallet and create the file `mycoin.conf` in the folder `%APPDATA%\mycoin\`.

<b>Important: replace "mycoin" with the name of your coin.</b>

```
rpcuser=rpc_user
rpcpassword=rpc_password
rpcallowip=127.0.0.1
listen=1
server=1
```

Download the latest version of cpuminer from <a href="https://bitcointalk.org/index.php?topic=55038.0">here</a> and extract the zip file.<br/>
Create a `.bat` file named `mine.bat` and paste the following text into `mine.bat`.
```
minerd --url=http://127.0.0.1:RPC_port --userpass=rpc_user:rpc_password
```
Save the file inside the extracted cpuminer folder.<br/>
Open your wallet and execute `mine.bat` to start mining your first coins.

## Start Staking
Open your wallet, and make sure you are connected to another wallet.<br/><br/>

Leave your wallet open and unlocked to stake.
Keep in mind that stake can only be generated when you have a balance in your wallet.

<b>Important: The following only applies if you encrypted your wallet.</b> <br/><br/>
You can unlock your wallet using the following instructions.<br/><br/>
Go to Help. <br/>
Click Debug Window. <br/> 
This is the console where you will execute all commands. <br/><br/>
Type this command to start staking:
```
walletpassphrase YOUR_PASSWORD 9999999 true
```
Replace the text "YOUR_PASSWORD" with your password.<br/><br/>
The number 9999999 is the amount of seconds you want to leave your wallet unlocked for staking.

## Disable Staking

One can disable staking by adding a parameter to your config file.<br/><br/>
Close your wallet and paste the following text into `mycoin.conf` and save the file.

```
staking=0
```
Staking will be disabled.
