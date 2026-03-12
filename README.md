# Quantum Bridge — OpenClaw Skill

Translate quantum circuits between frameworks and run them on real hardware, right from your OpenClaw agent.

## What It Does

- **Transpile** OpenQASM 2.0 → OriginIR (and reverse)
- **Validate** OriginIR syntax
- **Run IBC Consensus** — quantum multi-agent consensus
- **Submit to Wukong** — real 72-qubit quantum hardware
- **CLI wrapper** included (`qbridge.sh`)

## Install

```bash
clawhub install quantum-bridge
```

Or manually copy the `quantum-bridge/` folder into your OpenClaw skills directory.

## Setup

1. Get a free API key (50 credits) at https://quantum-api.gpupulse.dev
2. Set `QUANTUM_BRIDGE_KEY=qb_...` in your environment

## Usage

Your OpenClaw agent will automatically use this skill when you ask about quantum circuits, transpilation, or hardware submission.

### CLI

```bash
export QUANTUM_BRIDGE_KEY=qb_your_key
./scripts/qbridge.sh transpile circuit.qasm
./scripts/qbridge.sh submit circuit.qasm wukong
./scripts/qbridge.sh consensus agents.json
./scripts/qbridge.sh balance
```

## Pricing

| Tier | Credits | Price |
|------|---------|-------|
| Free | 50 | $0 |
| Starter | 500 | $5 |
| Pro | 5,000 | $25 |
| Enterprise | 50,000 | $100 |

## License

MIT
