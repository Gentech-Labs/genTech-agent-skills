# ⚡ GenTech Agent Kit

**The AAE-compatible agent standard. Identity. Execution. Audit. Baked in.**


---

## Why This Exists

Building an AI agent that works in the agent economy requires:

1. **Identity** — Who is this agent paying on behalf of?
2. **Enforcement** — Make the transaction happen
3. **Audit** — Prove it went through

Integrating these separately takes **weeks**. GenTech Agent Kit bakes them together. One import. All three pieces. Ready to ship.

> "We're the wrapper after all."

---

## The Three Pillars

### 🔐 Identity
> "Agents need to know who they're paying on behalf of."

- Wallet binding (EVM, Solana, Base)
- User verification (ERC-8004 trustless agents)
- Persona isolation (per-user dashboards and data)
- Multi-chain identity resolution

### ⚡ Enforcement
> "Agents need to be enforced to make the transaction."

- x402 payment rails (Circle, USDC)
- Auto-execution with configurable thresholds
- Multi-sig for high-value transactions
- Protocol-native integration (Travala, WURK, LFJ)

### 📋 Audit
> "Agents need to be audited to make sure the transaction went through."

- Transaction logging with receipts
- Proof of execution on-chain
- Dashboard visualization of all activity
- Automated compliance reporting

---

## What's Included

### Brain Layer
```yaml
context_management: true
mess_hall_scratchpad: true
handoff_notes: true
memory_bar: "80-100% only"
cron_snapshots: "every 6 hours"
```

### DeFi Layer
```yaml
lp_tracking: true
yield_scouting: true
milestone_progression: true
live_price_feeds: "DexScreener, Birdeye"
supported_chains: [avalanche, ethereum, base, solana]
```

### Protocol Layer
```yaml
payments: "x402, Circle USDC"
travel: "Travala integration"
tasks: "WURK.fun microtasks"
privacy: "COTI private transactions"
```

### Automation Layer
```yaml
context_snapshots: "every 6 hours"
nightly_housekeeping: "11 PM ET"
weekly_maintenance: "Monday 10 AM"
health_monitoring: "every 6 hours"
```

### Presentation Layer
```yaml
dashboard_engine: "38KB, zero deps"
section_types: 8
field_formats: 7
themes: 5
mobile_first: true
```

---

## Quick Start

### 1. Clone the Kit
```bash
git clone https://github.com/Gentech-Labs/genTech-agent-kit.git
cd genTech-agent-kit
```

### 2. Copy to Your Hermes Profile
```bash
cp -r skills/* ~/.hermes/profiles/your-profile/skills/
cp -r cron/* ~/.hermes/profiles/your-profile/cron/
```

### 3. Set Up Your Vault
```bash
cp -r vault-structure/* ~/your-vault/
```

### 4. Configure Your Agent
```yaml
# config.yaml
agent:
  name: "Your Agent"
  identity:
    wallet: "0x..."  # Your EVM wallet
    chain: "avalanche"
  enforcement:
    auto_execute: true
    threshold: 100  # USD
  audit:
    logging: true
    dashboard: true
```

### 5. Deploy
```bash
hermes start
```

Your agent now has identity, enforcement, and audit baked in.

---

## Agent Architecture

```
GenTech Agent
│
├── 🧠 Brain Layer
│   ├── Proactive context saving
│   ├── Mess Hall scratchpad
│   ├── Handoff notes
│   └── Memory bar (80-100%)
│
├── 📁 Vault Layer
│   ├── Green Room (ideas)
│   ├── Mess Hall (thinking)
│   ├── Archive (history)
│   └── INDEX.md (navigation)
│
├── 💰 Identity Layer
│   ├── Wallet binding (EVM/Solana/Base)
│   ├── User verification (ERC-8004)
│   ├── Persona isolation
│   └── Multi-chain resolution
│
├── ⚡ Enforcement Layer
│   ├── x402 payments (Circle)
│   ├── Auto-execution engine
│   ├── Multi-sig support
│   └── Protocol integration
│
├── 📋 Audit Layer
│   ├── Transaction logging
│   ├── Proof of execution
│   ├── Dashboard visualization
│   └── Compliance reporting
│
├── 🔍 DeFi Layer
│   ├── LP position tracking
│   ├── Yield scout fleet
│   ├── Fee milestones
│   └── Live price feeds
│
├── 🔗 Protocol Layer
│   ├── x402 payments
│   ├── WURK.fun tasks
│   ├── Travala travel
│   └── COTI privacy
│
├── 🤖 Automation Layer
│   ├── Context snapshots (6h)
│   ├── Nightly housekeeping
│   ├── Weekly maintenance
│   └── Health monitoring
│
└── 📊 Presentation Layer
    ├── Dashboard Engine (38KB)
    ├── Persona dashboards
    ├── Scout visualization
    └── Milestone progression
```

---

## Chain Support

| Chain | Status | Protocols |
|-------|--------|-----------|
| **Avalanche** | ✅ Live | LFJ, Pangolin, Benqi |
| **Ethereum** | ✅ Live | Uniswap, Aave, Lido |
| **Base** | ✅ Live | Uniswap, Aerodrome |
| **Solana** | 🔄 Coming | Raydium, Orca, Jito |
| **BNB Chain** | 🔄 Coming | PancakeSwap, Venus |
| **Arbitrum** | 🔄 Coming | Uniswap, GMX |

**Each chain gets the GenTech spin:**
- Native protocol integrations
- Optimized gas strategies
- Chain-specific yield opportunities
- Local compliance handling

---

## Troubleshooting

### Gateway Configuration Errors

If your gateway crash-loops with `TypeError: string indices must be integers, not 'str'`, check the `home_channel` configuration format. See [docs/hermes-gateway-troubleshooting.md](docs/hermes-gateway-troubleshooting.md) for details.

---

## Contributing

We welcome contributions! Here's how:

### For Developers
1. Fork the repo
2. Add your integration
3. Submit a PR with tests
4. Get merged, ship it

### For Protocol Teams
1. Open an issue with your protocol details
2. We'll add native integration
3. Your protocol gets GenTech Agent support

### For Community
1. Share your use cases
2. Request new chains/protocols
3. Report bugs, suggest features

---

## Roadmap

### Q3 2026
- [ ] Solana integration
- [ ] BNB Chain support
- [ ] Multi-agent coordination
- [ ] Advanced audit dashboard

### Q4 2026
- [ ] Mobile agent app
- [ ] Voice command interface
- [ ] Cross-chain atomic swaps
- [ ] Institutional compliance module

### 2027
- [ ] AI agent marketplace
- [ ] Agent-to-agent payments
- [ ] Regulatory framework integration
- [ ] Enterprise deployment tools

---

## License

MIT — use it for anything. Built by GenTech Labs for the agent economy.

---

**Built with ❤️ by [GenTech Labs](https://github.com/Gentech-Labs)** — Tough love for the agent economy.
