# Changelog

All notable changes to Lumia Pulse are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Entries before the first release were reconstructed from internal development history.

## [2026.04] - 2026-04-29

_First release of the node rewards platform_

### Added

- **api** — Reward engine that computes daily emissions for node operators
- **api** — Staking tiers with three delegation levels, and endpoints reporting staked node counts per participant
- **api** — Token price service backing reward valuations
- **dashboard** — Participant dashboard with home, node power and rewards pages
- **dashboard** — Airdrop claim flow with eligibility checks and typed-data signing
- **admin** — Operator views over participant wallets and reward state

### Changed

- **api** — Reward calculations aligned with the published HyperNodes reward model, with the model itself documented alongside the API

### Security

- **api** — Internal wallets are excluded from reward eligibility across every endpoint
