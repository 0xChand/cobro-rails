# Cobro

Cobro creates shareable payment requests for Ripio wFIAT on Celo mainnet. A recipient creates a link locally; a payer reviews the destination and uses an injected EIP-1193 wallet to send an ERC-20 transfer. Transactions include the event-issued ERC-8021 tag `celo_7ff34447af9e`.

## Current scope and limits

This is an early payment-link implementation. Links are unsigned and can be modified; users must verify details independently. A submitted transaction is not presented as settled: confirm the transaction and ERC-20 Transfer event in the explorer. There is no invoice database, automatic reconciliation, x402 integration, autonomous agent, or ERC-8004 identity yet. The app never handles private keys. ERC-20 transfers are irreversible and a compatible wallet, supported token balance, and gas are required.

## Run

`npx wrangler dev` or `npx wrangler deploy`. Static files are served by a Cloudflare Worker. No build step is required.

## Hackathon

Agents on Open Rails, LatAm track. Enrollment code `celo_7ff34447af9e`. Eligibility still requires an agent wallet and its ERC-8004 identity, a public repository, submission, and verifiable mainnet use. No user activity or payment has been claimed.
