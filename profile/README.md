<div align="center">
  <img src="https://www.magpie.capital/icon-512.png" alt="Magpie Capital" width="128" />
  <h1>Magpie Capital</h1>
  <p>
    <b>Permissionless SOL lending on Solana.</b><br/>
    Memecoin and tokenized-stock collateral · On-chain credit oracle · Agent-native via x402.
  </p>
  <p>
    <a href="https://magpie.capital"><img src="https://img.shields.io/badge/site-magpie.capital-0ea5e9?style=flat-square&logo=safari&logoColor=white" alt="site"/></a>
    <a href="https://x.com/MagpieLoans"><img src="https://img.shields.io/badge/X-@MagpieLoans-000000?style=flat-square&logo=x&logoColor=white" alt="X"/></a>
    <a href="https://t.me/magpie_capital_bot"><img src="https://img.shields.io/badge/Telegram-bot-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="bot"/></a>
    <a href="https://t.me/magpietalk"><img src="https://img.shields.io/badge/Telegram-community-26A5E4?style=flat-square&logo=telegram&logoColor=white" alt="community"/></a>
    <a href="https://www.magpie.capital/api/v1/stats"><img src="https://img.shields.io/badge/live%20stats-public-22c55e?style=flat-square&logo=vercel&logoColor=white" alt="stats"/></a>
    <a href="https://www.magpie.capital/security"><img src="https://img.shields.io/badge/security-disclosed-eab308?style=flat-square&logo=shield&logoColor=white" alt="security"/></a>
  </p>
</div>

---

## What we ship

Magpie is a real lending protocol with daily flow, not a roadmap. Every claim below is verifiable on-chain or at a live endpoint:

- **Permissionless SOL borrowing** against memecoin and tokenized-stock collateral with on-chain liquidation enforcement and an on-chain credit oracle. → [`/api/v1/stats`](https://www.magpie.capital/api/v1/stats)
- **Agent-native lending via x402.** The first Solana lending protocol with pay-per-call AI-agent endpoints — credit scores, signed credit attestations, intent-based borrows, and unsigned-tx builders. → [`magpie.capital/x402`](https://www.magpie.capital)
- **Holder distributions in SOL.** Ten percent of every loan fee flows to $MAGPIE holders automatically. → [`/api/v1/stats`](https://www.magpie.capital/api/v1/stats)
- **Layered runtime defense.** Every borrow passes through a TWAP oracle, cross-source price agreement, and a real-time post-borrow watcher. Sub-1.5% lifetime liquidation rate across 450+ loans. → [`/security`](https://www.magpie.capital/security)
- **Off-chain signal governance with explicit scope.** Holders vote on what's listed in [`GOVERNANCE.md`](https://github.com/magpiecapital/magpie-site/blob/main/GOVERNANCE.md). Operator commits to honor passing votes within bounds. → [`/governance`](https://www.magpie.capital/governance)
- **Fair launch.** $MAGPIE was distributed entirely through the pump.fun bonding curve. No team allocation, no presale, no advisor allocation, no vesting cliffs.

---

## Active workstreams

We work in the open where it doesn't compromise users, partners, or in-flight commercial conversations. We work in private where confidentiality is load-bearing. Both modes ship continuously.

### 🟢 Public protocol surfaces

| Repo | What's here | Stars/issues |
|---|---|---|
| **[`magpie-bot`](https://github.com/magpiecapital/magpie-bot)** | Telegram wallet bot, Anchor lending program, credit oracle, full protocol services. The execution layer. | ![issues](https://img.shields.io/github/issues/magpiecapital/magpie-bot?style=flat-square) ![last commit](https://img.shields.io/github/last-commit/magpiecapital/magpie-bot?style=flat-square) |
| **[`magpie-site`](https://github.com/magpiecapital/magpie-site)** | [magpie.capital](https://magpie.capital) — landing, dashboard, docs, governance, transparency endpoints. The trust layer. | ![issues](https://img.shields.io/github/issues/magpiecapital/magpie-site?style=flat-square) ![last commit](https://img.shields.io/github/last-commit/magpiecapital/magpie-site?style=flat-square) |
| **[`magpie-x402`](https://github.com/magpiecapital/magpie-x402)** | Pay-per-call agent API — credit scores, attestations, conditional borrow intents, unsigned-tx builders. The growth layer. | ![issues](https://img.shields.io/github/issues/magpiecapital/magpie-x402?style=flat-square) ![last commit](https://img.shields.io/github/last-commit/magpiecapital/magpie-x402?style=flat-square) |

### 🔒 Private workstreams (ongoing — request access via the contact column)

| Repo | What's shipping there | Who should reach out |
|---|---|---|
| **`magpie-marketing`** | Coordinated campaigns across X, Telegram, blog, podcast outreach, hackathon presence, aggregator listings, brand iteration. Cadence: continuous. Most work here is embargoed until announcement. | Press, podcast hosts, content collaborators, hackathon organizers → DM **[@MagpieLoans](https://x.com/MagpieLoans)** |
| **`magpie-partners`** | Active partnership pipeline across web2 (exchanges, custodians, RWA issuers, distribution platforms) and web3 (DeFi primitives, AI agent frameworks, on-chain data providers, MCP registries). NDA-covered. Multiple deals in flight at any time. | Protocols, exchanges, wallet providers, agent frameworks, RWA issuers → DM **[@MagpieLoans](https://x.com/MagpieLoans)** with a one-paragraph intro |

The fact that these repos *exist* is public on purpose — partnerships and marketing are real, continuous workstreams here, not afterthoughts. Specifics stay private because confidentiality is load-bearing for both surfaces.

---

## Building on Magpie

The fastest paths in:

- **Build an agent that borrows.** [`magpie-x402`](https://github.com/magpiecapital/magpie-x402) exposes the full borrow / repay / extend / topup / partial-repay / liquidate flow as pay-per-call endpoints with no API key, no signup. Conditional borrow intents work like limit orders. The [`MARKETING.md`](https://github.com/magpiecapital/magpie-x402/blob/main/MARKETING.md) doc has the agent-distribution roadmap and open issues for SDK integrations, MCP server, examples directory, and bounties.
- **Add Magpie credit scores to your protocol.** The `/agent/credit-attest` endpoint returns an ed25519-signed credit attestation any consumer can verify on-chain without trusting Magpie. Portable reputation for Solana DeFi.
- **Become a Magpie collateral token.** Submit via `/submit` in the bot or [magpie.capital/submit](https://www.magpie.capital). Runs a six-layer scam audit. Three outcomes: Instant Approval / Submission Needs Review / Declined.

## Operating principles

- **Fair launch and permissionless contract surface.** Any wallet can borrow, repay, or liquidate without identification or whitelisting.
- **Layered runtime defense over one-time audits.** Every borrow runs the full gauntlet on every request — calibrated against attacks seen in production, not abstract threat models.
- **Transparent operating record.** Live stats, supply, governance state, security posture, audit history, and incident reports are all public and live, not curated.
- **Governance with explicit, narrow scope.** What holders can vote on is enumerated. What stays operator-discretion is enumerated. No ambiguity by design.
- **Anonymous founder, identified protocol.** Operator identity is private; protocol activity is fully on-chain and verifiable.

## Security & Audits

Magpie's smart-contract audit process is **actively underway**. Independent security firms have been **engaged to review** the protocol's on-chain lending programs; **reports will be published when complete**. The protocol is **not yet audited** — please don't treat the absence of a published report as a completed review.

| Firm | Engagement status |
|---|---|
| **Sec3** | Repository access granted; review underway (formal scope being finalized). |
| **Hashlock** | Invited (read-only access); engagement in progress. |
| **QuillAudits** | Invited (read-only access); engagement in progress. |
| **OtterSec** | Invited to audit; awaiting response. |

The audit-target program ([`magpie-v4`](https://github.com/magpiecapital)) is kept **private** during pre-audit review, and every engaged firm is granted **read-only** access. Completed reports will be published in [`magpiecapital/audits`](https://github.com/magpiecapital/audits).

**Disclosure path:** see [magpie.capital/security](https://www.magpie.capital/security) for the security posture and reporting path. For routine reports, the fastest channel is a GitHub issue tagged `security` on the relevant public repo. For sensitive disclosures, use the security page.

## License

Code in public repos is under each repo's stated license (typically MIT). Private repos are proprietary. The Magpie brand and logo are not licensed for third-party use.
