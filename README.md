# aisling-jwks

Public JWKS for the Aisling Platform's eCW Backend Services integration.

The single key in `jwks.json` is the public half of an RSA-2048 keypair used to
sign client_credentials JWT assertions when authenticating to eCW's FHIR
sandbox at `staging-fhir.ecwcloud.com`. Private key is stored only in
Azure Key Vault (`kv-dev-integration-ais` / `ds-connection-eclinicalworkssandbox-system`).

This repo exists solely to provide a stable public URL eCW can fetch from.
