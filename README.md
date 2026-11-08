# BingwaPulse Web

Browser workspace for the BingwaPulse product family.

## Current implementation
- Responsive business workspace for offers, customers, orders and transaction notes.
- Local browser storage for offline work.
- Account registration and sign-in against the shared BingwaPulse API.
- Durable local sync outbox, revision-aware push/pull and cursor persistence.
- Browser session token stored in sessionStorage.

## Run
Open `index.html` using a local static web server. Configure the shared API address in the account panel. The API must allow the website's origin through `CORS_ORIGINS`.

## Data behavior
Local records stay in this browser until the user signs in and syncs. The same account/tenant can be used in Android. Conflicts are not silently overwritten. Transaction notes remain unverified.

## Production requirements
Use HTTPS for both Web and API, managed secrets, tenant authorization, backups, monitoring and a reviewed security deployment. This client does not connect to M-PESA, SMS, USSD or bundle fulfilment.
