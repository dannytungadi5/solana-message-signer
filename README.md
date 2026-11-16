# Solana Message Signer

Sign arbitrary messages with a Solana wallet, entirely in your browser.

Live page: <https://dannytungadi5.github.io/solana-message-signer/>

## What it does

- Connects to a browser wallet that implements the Solana wallet standard (for example Phantom or Solflare).
- Shows the exact message text that will be signed before you approve anything in the wallet.
- Produces a base58-encoded Ed25519 signature you can copy and verify elsewhere.

## How to use

1. Open the page.
2. Paste the exact message you were asked to sign into the message box and compare it character by character with the request you received.
3. Click **Connect wallet** and approve the connection in your wallet.
4. Click **Sign message** and review the message shown by your wallet before approving.
5. Copy the resulting signature.

## Properties

- Single self-contained `index.html`: no build step, no dependencies.
- No external scripts, fonts, analytics, or network calls of its own. The only network activity comes from the wallet extension itself.
- Nothing is stored or transmitted; refreshing the page clears everything.

## Safety notes

- Only sign a message when you know who asked for it and the text matches exactly what you were shown.
- Signing a message does not move funds or approve a transaction, but a signature can be used as proof of wallet ownership, so treat it as sensitive.
