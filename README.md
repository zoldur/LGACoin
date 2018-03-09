# League Coin
Shell script to install a [Leagued Masternode](https://league.express/) on a Linux server running **Ubuntu 14.04**. Use it on your own risk.
***

## Installation
```
wget -q https://raw.githubusercontent.com/zoldur/LGACoin/master/lgacoin_install.sh  
bash lgacoin_install.sh
```
***

## Desktop wallet setup  

After the MN is up and running, you need to configure the desktop wallet accordingly. Here are the steps:  
1. Open the Leagued Wallet.  
2. Go to RECEIVE and create a New Address: **MN1**  
3. Send **3000** **LGA** to **MN1**.  
4. Wait for 16 confirmations.  
5. Go to **Help -> "Debug Window - Console"**  
6. Type the following command: **masternode outputs**  
7. Go to **Masternodes** tab  
8. Click **Create** and fill the details:  
* Alias: **MN1**  
* Address: **VPS_IP:PORT**  
* Privkey: **Masternode Private Key**  
* TxHash: **First value from Step 6**  
* Output index:  **Second value from Step 6**  
* Reward address: leave blank  
* Reward %: leave blank  
9. Click **OK** to add the masternode  
10. Click **Start All**  
***

## Usage:
```
Leaguedd masternode status  
Leaguedd getinfo
```
Also, if you want to start/stop **Leagued**, run one of the following commands as **root**:

```
/etc/init.d/Leagued start #To start League service  
/etc/init.d/Apollon stop #To stop League service
```  
***

## Donations

Any donation is highly appreciated  

**LGA**: mgWBmWsoQ2FH6PQD9uES9CH5EhR73gVtVU  
**BTC**: 3MQLEcHXVvxpmwbB811qiC1c6g21ZKa7Jh  
**ETH**: 0x39d10fe57611c564abc255ffd7e984dc97e9bd6d  
**LTC**: LNZpK4rCd1JVSB3rGKTAnTkudV9So9zexB
