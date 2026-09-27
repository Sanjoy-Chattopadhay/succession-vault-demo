# Succession Vault (Sepolia demo)

A browser app for trustee-less digital inheritance on the Ethereum Sepolia test network.

- An owner puts NFTs, tokens and ETH in a vault with a will (a Merkle root of bequests).
- The vault stays alive while the owner sends heartbeats and zero-knowledge proofs of life.
  A key alone can delay the heirs by at most one proof-of-life interval.
- After the deadline and a grace period, heirs claim their bequests with a will package; age-restricted
  bequests are claimed with an in-browser zero-knowledge age proof.

**Live app:** https://sanjoy-chattopadhay.github.io/succession-vault-demo/

This is a research demo. The demo liveness issuer's signing key is public, so anyone can produce its
"proofs of life". Use test assets only.

This repository holds the built static site (bundled JavaScript, the Groth16 circuits and proving keys).
