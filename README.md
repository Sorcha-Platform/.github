# Sorcha Platform

**Trust infrastructure for the multi-party world.**

Sorcha is an open-source distributed ledger platform that lets organisations define, execute, and cryptographically verify shared workflows — without surrendering control of their data.

---

### The Problem

When multiple organisations need to share data — supply chains, government services, regulatory compliance — they're forced into one of two bad options: hand everything to a central platform they don't control, or build fragile point-to-point integrations they can't trust. Neither scales. Neither respects data sovereignty.

### The Approach

Sorcha takes a different path. **Blueprints** define structured, multi-step workflows with schema validation and conditional routing. **Wallets** give every participant cryptographic signing and selective disclosure — share only what's needed, prove it's authentic, nothing more. **Registers** provide an immutable, verifiable record of every transaction. And a **Peer Network** replicates state across participants without a central authority.

The result: organisations collaborate on shared processes while each retains sovereignty over their own data.

### What's Here

| Repository | Description |
|---|---|
| [**Sorcha**](https://github.com/Sorcha-Platform/Sorcha) | The core platform — Blueprint engine, Wallet service, Register ledger, Tenant identity, Peer network, and API Gateway. Built on .NET 10 with Aspire orchestration. |
| [**GovModel**](https://github.com/Sorcha-Platform/govmodel) | A Model Government reference implementation. Demonstrates how municipal governance — permits, licensing, citizen credentials, enforcement verification — works on Sorcha. Grounded in real public sector processes. |

### Capabilities

**Workflow Orchestration** — JSON Blueprints with multi-step processes, conditional routing, approval chains, and schema validation at every stage.

**Cryptographic Trust** — HD wallets supporting ED25519, NIST P-256, RSA-4096, and post-quantum algorithms (ML-DSA, ML-KEM). Every action is signed and verifiable.

**Selective Disclosure** — Field-level encryption with JSON Pointer-based disclosure policies. Participants see only what they're authorised to see. Citizens control what they share.

**Immutable Records** — Merkle-tree docketed registers with chain validation. Records can't be silently altered or deleted.

**Peer Replication** — gRPC-based P2P topology so no single party holds the only copy.

**AI-Assisted Design** — MCP Server integration for AI-assisted Blueprint authoring and workflow design.

### Quick Start

```bash
git clone https://github.com/sorcha-platform/sorcha.git
cd sorcha
./scripts/sorcha-setup.sh
```

Requires Docker Desktop and Git. Launches the full platform at `http://localhost/app`.

### Use Cases

Sorcha is designed for scenarios where **multiple parties must collaborate on structured processes with trust, privacy, and auditability**:

- **Digital Product Passports** — tamper-evident, multi-party product lifecycle records under EU ESPR regulation
- **Municipal Governance** — citizen credentials, permit workflows, cross-department verification (see [GovModel](https://github.com/Sorcha-Platform/govmodel))
- **Regulated Supply Chains** — provenance tracking with selective disclosure across suppliers, auditors, and regulators
- **Multi-Agency Case Management** — shared workflows across organisations with data sovereignty boundaries

### Built With

.NET 10 · C# 13 · .NET Aspire · gRPC · SignalR · PostgreSQL · MongoDB · Redis · Docker

### Licence

MIT — see individual repositories for details.

---

<sub>Sorcha (IPA: /ˈsɔːr.ə.xə/) — from Irish, meaning *brightness* or *light*.</sub>
