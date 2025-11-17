# DeFlow Protocol (Hackathon MVP)

## Purpose
Short: Decentralized AI venture intelligence on Cardano.

Long: DeFlow is a decentralized, AI-powered startup evaluation and due-diligence protocol that eliminates fake traction, biased scoring, and unverifiable claims. It ingests founder submissions, market data, and traction metrics, then orchestrates a trustless network of AI agents and Cardano smart contracts to deliver fraud-resistant scores, anomaly flags, and immutable audit trails.

## Structure
- `/backend` - FastAPI service hosting ingestion APIs, scoring pipelines, LangChain workflows, and oracle bridges.
- `/frontend` - Next.js + Tailwind DApp for founder onboarding, investor dashboards, and NFT identity management.
- `/contracts` - Cardano smart contract stubs for registry entries, oracle votes, and CIP-25 NFT minting.
- `/docs` - Design specs, threat models, runbooks, and oracle coordination manuals.
- `/scripts` - Helper utilities for local dev, seeding, migrations, and DevOps automation.

## MVP
Ingest -> Scrape -> Score -> IPFS -> Cardano metadata (testnet) -> Dashboards

## System Overview
- **Trustless Startup Intelligence**: Multi-document ingestion, semantic understanding, anomaly detection, and multi-factor scoring operate off-chain, while score commitments are anchored on-chain for tamper-proof provenance.
- **Decentralized AI Oracle Network**: Independent oracle nodes re-score submissions, reach consensus, and sign results before writing hashes and verdicts to Cardano.
- **Verifiable Startup Identity NFTs**: Each startup mints a CIP-25-compliant NFT capturing score breakdowns, anomaly hashes, and IPFS pointers to the due-diligence report.
- **AI VC Analyst Dashboard**: RAG-powered insights provide competitor benchmarking, traction graphs, anomaly explanations, and improvement guidance for founders.
- **Deal Flow Explorer**: Investors browse verified startup cards, trust indicators, and anomaly flags with real-time updates sourced from on-chain data.

## Core Workflow
1. **Submit**: Founders upload decks, traction metrics, and market data via the DApp.
2. **Ingest & Scrape**: Backend agents enrich submissions with web, social, and market intelligence.
3. **Analyze & Score**: LangChain pipelines run semantic checks, fraud-signal detection, and multi-factor scoring.
4. **Oracle Consensus**: Decentralized AI oracles re-validate scores, detect manipulation, and provide signed attestations.
5. **Anchor On-Chain**: Hashes of due-diligence reports, anomaly logs, and score breakdowns settle on Cardano testnet contracts.
6. **Mint Identity NFT**: Startups receive CIP-25 NFTs referencing IPFS artifacts and oracle consensus data.
7. **Dashboard Delivery**: Founders view AI analyst outputs; investors access Deal Flow Explorer dashboards.

## Architecture Snapshot
- **Frontend**: Next.js, Tailwind CSS, Wallet adapters, CIP-25 NFT viewers, dashboard widgets.
- **Backend**: FastAPI, LangChain, vector DB, scraping pipelines, anomaly detection engines, IPFS publishing.
- **Oracle Layer**: Multi-node AI oracle cluster, signature aggregation, dispute resolution hooks.
- **Cardano Contracts**: Startup registry, oracle vote ledger, CIP-25 metadata writers.
- **Storage**: IPFS/Arweave for reports, embeddings, and evidence bundles.

## Value Propositions
- Trustless startup intelligence anchored by cryptographic proofs.
- Fraud detection via anomaly scoring and metric cross-verification.
- Verified startup identity NFTs serving as tamper-proof credentials.
- Decentralized oracle consensus preventing single-agent manipulation.
- Autonomous discovery engine that surfaces high-potential startups early.
- Founder guidance through RAG-powered analyst coaching.
- VC-facing deal flow dashboards with reliable data and alerts.

## Getting Started (Placeholder)
- `frontend`: TBD (Next.js bootstrap instructions)
- `backend`: TBD (FastAPI + poetry/pipenv setup)
- `contracts`: TBD (Cardano testnet tooling)
- `scripts`: TBD (automation entrypoints)

## Roadmap Highlights
- Implement ingestion API schemas and validation.
- Integrate scraping + enrichment workers and LangChain pipelines.
- Stand up oracle node reference implementation.
- Draft Cardano Plutus script stubs for registry + NFT minting.
- Build MVP dashboards for founders and investors.
- Automate IPFS pinning and hash anchoring.

## License
TBD - select OSS or proprietary license post-hackathon.
