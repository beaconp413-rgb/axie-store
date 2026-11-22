# Axie Store

A separate copy of [Axie Team Builder](https://github.com/beaconp413-rgb/axie-team-builder) that sells only the Axies in the
store wallet `0x64386aad85ecb4b8f5c7e6718482c86891b22049`, with GCash checkout: the buyer pays and types the GCash
reference number, the seller approves in Telegram, and the Worker sends the Axies to the buyer's Ronin address.

- Site: https://beaconp413-rgb.github.io/axie-store/ (seller mode: add `#seller`)
- Backend: the same Cloudflare Worker `axie-shop` (code in the axie-team-builder repo, `/worker`), using its `/store/*`
  routes, which have their own price list and wallet snapshot, so this site never changes the original shop.
