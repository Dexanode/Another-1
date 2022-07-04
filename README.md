## Another -1 Testnet

```bash
  wget -q -O another-1-rekap.sh https://raw.githubusercontent.com/nadi555/Another-1/main/another-1-rekap.sh && chmod +x another-1-rekap.sh && sudo /bin/bash another-1-rekap.sh
```



#### after installation

```bash
  source $HOME/.bash_profile
```


#### validator info

```bash
anoned status 2>&1 | jq .ValidatorInfo

anoned status 2>&1 | jq .SyncInfo

anoned status 2>&1 | jq .NodeInfo
```
#### Create your wallet
Add New Wallet

```bash
anoned keys add wallet
```
#### Recover Existing Wallet

```bash
anoned keys add wallet --recover
```
#### List All Wallet

```bash
anoned keys list
```

#### Check Wallet Balance

```bash
anoned q bank balances $(anoned keys show wallet -a)
```
