# Ballot Project

## Setup Project

Install dependencies

```bash
npm run install
```

Create a .env file and add your env variables

```bash
cp .env.example .env
```

Compile smart contract

```bash
npm run compile
```

## Deploy

Deploy with hardhat

```bash
npm run compile
npm run deploy:hardhat
```

Deploy with Viem

```bash
npm run compile
npm run deploy:viem <PROPOSAL_1> <PROPOSAL_N>
```

See your contract deployed in:

```
https://sepolia.etherscan.io/address/<CONTRACT_ADDRESS>
```

## Interact with the contract

Cast vote:

```bash
npm run contract:cast-vote <CONTRACT_ADDRESS> <PROPOSAL_INDEX>
```

Give right to vote:

```bash
npm run contract:give-right-to-vote <CONTRACT_ADDRESS> <NEW_VOTER_ADDRESS>
```

Delegate vote:

```bash
npm run contract:delegate-vote <CONTRACT_ADDRESS> <DELEGATE_VOTE_ADDRESS>
```

Query winner name:

```bash
npm run contract:query-winner-name <CONTRACT_ADDRESS>
```

Query winning proposals

```bash
npm run contract:query-winning-proposals <CONTRACT_ADDRESS>
```
