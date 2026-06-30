# Changelog

All notable changes to Lumia Pulse are documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Entries before the first release were reconstructed from internal development history.

## [2026.06] - 2026-06-30

_Overview page_

### Added

- **dashboard** — Overview page bringing node, staking and reward figures together in one view
- **api** — Aggregated figures behind the overview page

### Changed

- **admin** — Reward contract configuration updated for the current airdrop round

## [2026.05] - 2026-05-27

_Delegation, claims and operator tooling_

### Added

- **dashboard** — Node delegation and reward claiming from the participant dashboard
- **dashboard** — Airdrop claim shows a staker eligibility preview, a countdown to the claim window and a shareable result card
- **admin** — Airdrop administration: configuration, claim statistics, participant search and wallet balances
- **admin** — Failed claims can be rolled back and retried
- **api** — Unstaking, additional reward buckets and cached staking state for faster dashboard loads

### Changed

- **api** — Staker reward tiers reworked

### Fixed

- **dashboard** — Wallet connection, claim signing and reward state loading no longer fail on reload

### Security

- **api** — Social account links are verified server-side during airdrop eligibility checks

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
