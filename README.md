# NFT staking
 - pays out constant reward rate per token

*note manually added mintAddresses in Config fields in the anchor IDL file


# Solana Program using Anchor - Staking

## Anchor

### Build

```sh
anchor build
```

### Deploy

```sh
solana program deploy --programid <keypair> target/verifiable/nft_staking.so
```

```sh
anchor test
```

## configure CLI

### Set CLI config url to localhost cluster

```sh
solana config set --url localhost
```

### Create CLI Keypair

```sh
solana-keygen new -o "./test-key.json"
```

## Start local Solana cluster

### Start a local Solana cluster

```sh
solana-test-validator
```

### Listen to transaction logs

```sh
solana logs
```

## Build the on-chain program

```sh
npm run build:anchor
```

## Deploy the on-chain program

```sh
solana program deploy target/deploy/nft_staking.so
```

## Run js client

```sh
npm run start
```

### create own token
```sh
spl-token create-token
```

### supply
```sh
spl-token supply EHkcswrrUs3Ej3gFYCmjmAMwSQC8j1cQtJCFEEzUYrpa
```

### create token account
```sh
spl-token create-account EHkcswrrUs3Ej3gFYCmjmAMwSQC8j1cQtJCFEEzUYrpa
```

### mint token
```sh
spl-token mint EHkcswrrUs3Ej3gFYCmjmAMwSQC8j1cQtJCFEEzUYrpa 1000000000000
```
