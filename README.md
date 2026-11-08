# BingwaPulse Web

Browser workspace for the BingwaPulse product family.

## Current implementation
A local-first browser workspace for managing draft offers and viewing operational summaries. Records are stored in this browser only. It is a single-device prototype—not an authenticated multi-agent portal and not connected to Android, Connect, M-PESA or a fulfilment provider.

## Run
Open `index.html` in a modern browser, or serve this folder with any static HTTP server.

## Before production
A secured backend is required for sign-in, tenant isolation, authorization, audit history, encrypted sync, backups and authoritative payment/fulfilment status. Do not place credentials or customer payment data in browser storage.

See [the integration contract](docs/INTEGRATION_CONTRACT.md).
