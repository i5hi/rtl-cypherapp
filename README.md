# rtl-cypherapp

rtl cypherapp config

## init

```
git clone https://github.com/i5hi/rtl-cypherapp /path/to/cyphernode/dist/apps/rtl
cd /path/to/cyphernode/dist/apps/rtl
```

## .env

```
touch .env
vi .env

RTL_DATAPATH=/path/to/cyphernode/dist/apps/rtl/data
BITCOIN_DATAPATH=/path/to/.cyphernode/bitcoin/testnet3
LIGHTNING_DATAPATH=/path/to/.cyphernode/lightning/testnet
GATEKEEPER_DATAPATH=/path/to/.cyphernode/gatekeeper
```

## data/RTL-Config.json

```
cp data/sample_RTL-Config.json data/RTL-Config.json
```

## issues

This config is not stable and is in progress. 

It will currently serve RTL UI at localhost:3009 or 0.0.0.0:3009 

RTL UI currently errors when accessed via traefik.

It is unable to access the files inside the `rtl` container under `/RTL/frontend`

Ideally the UI must be served only via traefik.
