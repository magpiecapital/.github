<div align="center">
  <img src="https://www.magpie.capital/icon-512.png" alt="Magpie Capital" width="120" />
  <h1>Magpie Capital</h1>
  <p>
    Permissionless SOL lending on Solana. Memecoin and tokenized-stock collateral.
    On-chain credit oracle. Agent-native via x402.
  </p>
  <p>
    <a href="https://magpie.capital">magpie.capital</a> ·
    <a href="https://x.com/MagpieLoans">@MagpieLoans</a> ·
    <a href="https://t.me/magpie_capital_bot">@magpie_capital_bot</a> ·
    <a href="https://t.me/magpietalk">@magpietalk</a>
  </p>
</div>

---

## Active workstreams

We work in the open where it doesn't compromise users, partners, or in-flight commercial conversations. We work in private where confidentiality is load-bearing. Every workstream is listed below; the public ones link to source, the private ones describe the surface so you know we're shipping there too.

### 🟢 Public

| Repo | Description |
|---|---|
| [`magpie-bot`](https://github.com/magpiecapital/magpie-bot) | The Telegram wallet bot, the Anchor lending program, and the core protocol services. |
| [`magpie-site`](https://github.com/magpiecapital/magpie-site) | [magpie.capital](https://magpie.capital) — public landing, dashboard, docs, governance, transparency endpoints. |
| [`magpie-x402`](https://github.com/magpiecapital/magpie-x402) | Pay-per-call AI-agent API on the x402 standard. Credit scores, attestations, build-* endpoints for autonomous flows. |

### 🔒 Private

| Repo | Why private | Outreach |
|---|---|---|
| `magpie-marketing` | Campaign timing, channel relationships, brand iteration — all benefit from confidentiality. The repo's existence is public so users can see marketing is sustained work. | [@MagpieLoans](https://x.com/MagpieLoans) |
| `magpie-partners` | Web2 and web3 partnerships — NDAs, embargoes, commercial terms, ongoing negotiations. The repo's existence is public so partners and prospective partners see we treat partnerships as a real workstream. | DM [@MagpieLoans](https://x.com/MagpieLoans) on X with a one-paragraph intro |

If you don't have access to a private repo and think you should, reach out via the channel listed.

## How Magpie works in one paragraph

Borrowers deposit memecoin or tokenized-stock collateral and receive SOL in seconds, with on-chain liquidation enforcement and an on-chain credit oracle that rewards repayment history. SOL liquidity comes from depositors who earn a share of every loan fee. The $MAGPIE token receives 10% of every loan fee as automatic SOL distributions to holders on a randomized cadence. Agents and other protocols access the same primitives through a permissionless, pay-per-call x402 API. All protocol activity is verifiable at [magpie.capital/api/v1/stats](https://magpie.capital/api/v1/stats).

## Operating principles

- **Fair launch.** $MAGPIE was distributed entirely through pump.fun's bonding curve. No team allocation, no presale, no advisor allocation, no vesting.
- **Permissionless contract surface.** Any wallet can borrow, repay, or liquidate without identification, whitelisting, or operator approval.
- **Layered defense over one-time audits.** Every borrow passes through a runtime gauntlet (TWAP oracle, cross-source price agreement, real-time post-borrow watcher) calibrated against actual attacks seen in production.
- **Transparent operating record.** Stats, supply, security disclosures, audit history, and incident reports are public and live, not curated.
- **Governance with explicit scope.** Holders vote on what's listed in [`magpie-site/GOVERNANCE.md`](https://github.com/magpiecapital/magpie-site/blob/main/GOVERNANCE.md) — operator commits to honor passing votes within bounds. Out-of-scope items are documented explicitly, not left implicit.

## Reporting a vulnerability

See [magpie.capital/security](https://magpie.capital/security) for the security posture and disclosure path. The fastest channel is a GitHub issue tagged `security` on the relevant public repo. For sensitive disclosures, contact via the security page.

## License

Code in public repos is under each repo's stated license (typically MIT). Private repos are proprietary. The Magpie brand and logo are not licensed for third-party use.
