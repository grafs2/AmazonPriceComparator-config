# AmazonPriceComparator – signed configuration

Public, static hosting for the signed configuration of the AmazonPriceComparator browser extension
(parser rules, store list, tax tables, feature switches).

- `config.signed.json` – signed envelope (ECDSA P-256 / SHA-256). The extension verifies the signature
  against public keys bundled in the extension and rejects anything invalid, expired or older than
  the active version.
- Do not edit by hand. Source of truth: `config/config.json` in the main repository, signed with
  `npm run config -- sign <keyId>`.
