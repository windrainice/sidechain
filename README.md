#### These are test only keys and should never be used for the production blockchain. 

Private key: EOS6MRyAjQq8ud7hVNYcfnVPJqcVpscN5So8BhtHuGYqET5GDW5CV

Public key: 5KQwrPbwdL6PhXujxW37FSSQZ1JiwsST4cqQzDeyXtP79zkvFD3


## For Block Producers: Join blockchain network to producing


### Step 1. Install
```
git clone https://github.com/meet-one/eos.git
cd eos
git checkout meetone-sidechain
git submodule update --init --recursive
./eosio_build.sh
sudo ./eosio_install.sh
```


### Step 2. Create new account

```
http://35.221.207.136:6677/newaccount?name=testnet115.m
```


### Step 3. Configure the initial set of nodeos

#### 1. open your config.ini
 
#### 2. replace producer-name to your producer name 
 
#### 3. replace signature-provider to your producer public key and private key


### Step 4. Launch the node

```
nodeos --data-dir ./nodeos/producer-node/data-dir --config-dir ./nodeos/producer-node/config-dir --genesis-json ./nodeos/producer-node/config-dir/genesis.json
```


## For EOS Developers: [https://developers.eos.io](https://developers.eos.io)