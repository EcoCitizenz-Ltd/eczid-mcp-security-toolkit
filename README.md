# ECZ-ID MCP Security Toolkit

![ECZ-ID MCP Security Toolkit architecture and configuration-review visual](https://raw.githubusercontent.com/EcoCitizenz-Ltd/.github/main/assets/repository-visuals/eczid-mcp-security-toolkit.jpg)

## Know what your MCP can do before you let it act.

Free, practical MCP security resources from EcoCitizenz Ltd / ECZ-ID.

### Start here

[**Install MCP Trust Free**](https://marketplace.visualstudio.com/items?itemName=ecocitizenz.eczid-mcp-trust)

[**Get a free MCP Passport**](https://developers.ecocitizenz.com/quickstarts/mcp/?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=free-mcp-passport)

[**Choose from all seven free machine Passport families**](https://developers.ecocitizenz.com/get-started/free-passport/?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=free-passports)

[**Download the MCP & AI Agent Trust Preflight**](https://developers.ecocitizenz.com/downloads/eczid-mcp-agent-trust-preflight.pdf?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=preflight)

[**Get MCP Trust Pro / Developer Trust**](https://developers.ecocitizenz.com/developer-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=mcp-trust-pro)

[**Explore MCP Assurance**](https://developers.ecocitizenz.com/mcp-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=mcp-assurance)

[**Need a professional MCP review?**](https://mcp.ecocitizenz.com?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=services)

---

## The problem

Connecting an MCP server can expose tools, schemas, network access, files, environment-variable names and other capabilities inside an increasingly agentic development environment.

The useful questions are:

- What MCP servers are configured?
- What tools and schemas are exposed?
- Which credential-shaped environment names are present?
- What changed since the previous review?
- Which capabilities deserve additional review?
- Is runtime traffic actually being mediated where enforcement is claimed?
- Can operator evidence be independently re-checked?

---

## MCP Trust Community

Free and local-first.

Use ECZ-ID MCP Trust Community to inspect supported MCP configuration, inventory surfaces and identify change without requiring an ECZ-ID account.

[Install MCP Trust →](https://marketplace.visualstudio.com/items?itemName=ecocitizenz.eczid-mcp-trust)

If you operate the MCP server, you can also give that logical server a free ECZ-ID MCP Passport. The Passport is identity and a public pointer for re-checkable current state; it is not a safety, approval or certification claim.

[Get the free MCP Passport →](https://developers.ecocitizenz.com/quickstarts/mcp/?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=community-passport)

---

## MCP Trust Pro

**MCP Trust Pro** is the optional paid local Developer Trust software layer. It adds the supported deeper local history and runtime controls that belong to the `MCP_TRUST_PRO` entitlement, including:

- Protect This MCP through the Local Trust Gate for supported transports;
- Secret Shield;
- Trust Epochs and local history;
- Advanced Tool X-Ray;
- deterministic local ALLOW / WARN / REVIEW / BLOCK / QUARANTINE policy;
- reviewable remediation with backup and rollback.

The MCP Passport remains the free core identity. MCP Trust Pro does not create or replace that Passport and does not issue canonical Resolver proof. **Developer Trust Pro Bundle** unlocks both MCP Trust Pro and Agent Trust Pro.

[Get MCP Trust Pro / Developer Trust →](https://developers.ecocitizenz.com/developer-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=get-mcp-trust-pro)

---

## Separate organisational product: MCP Assurance

**MCP Assurance is separate from MCP Trust Pro.** It is a higher-level organisational MCP assurance product and must not be presented as the customer-facing name of the `MCP_TRUST_PRO` software entitlement.

Use MCP Assurance when the organisational requirement is broader than local developer inspection, mediation and policy controls. Buying MCP Assurance does not redefine MCP Trust Pro, and buying MCP Trust Pro does not create MCP Assurance.

[Explore MCP Assurance →](https://developers.ecocitizenz.com/mcp-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=get-mcp-assurance)

Payment does not make an MCP server safe, approved, certified or compliant, and it does not change the meaning of public Resolver evidence.

---

## Product boundary

| Layer | Product / capability |
|---|---|
| Free local review | MCP Trust Community |
| Free durable identity | MCP Passport |
| Optional paid local developer software | MCP Trust Pro |
| Optional paid developer bundle | Developer Trust Pro Bundle — MCP Trust Pro + Agent Trust Pro |
| Separate higher-level organisational product | MCP Assurance / MCP Assurance Plus |
| Public proof | ECZ-ID Resolver |

These layers may work together, but they are not aliases for one another.

---

## Organisation or enterprise requirement?

For teams requiring professional assessment, migration or enterprise implementation:

[Explore MCP Readiness Services →](https://mcp.ecocitizenz.com?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=audit)

---

## Public operator proof

**ECZ-ID public identity evidence - ECZ-GB-RBS1NW**
[View current public identity & evidence →](https://resolver.ecocitizenz.org/p/ECZ-GB-RBS1NW)

ECZ-ID publishes evidence for review. It does not certify a server as safe or replace the relying party's policy.

---

## Use ECZ-ID inside GitHub

### Pull-request and committed-configuration review

Use **ECZ-ID MCP & Agent Check** for supported committed MCP and agent configuration. It reviews repository changes and reports deterministic findings without executing repository code.

[Install ECZ-ID MCP & Agent Check](https://github.com/marketplace/ecz-id-mcp-agent-check)

### Public Resolver posture in CI

Use **ECZ-ID MCP Verifier** when you have an ECZ-ID parent reference and want a repeatable public Resolver-posture check in CI.

```yaml
- name: Check ECZ-ID public Resolver posture
  uses: Ecocitizenz/ecz-id-mcp-verifier@v0.9.1
  with:
    target: ECZ-GB-RBS1NW
    policy: PREFER
```

[ECZ-ID MCP Verifier source and usage](https://github.com/Ecocitizenz/ecz-id-mcp-verifier)

The verifier reads and reports public Resolver posture. It does not inspect arbitrary target contents or replace your local policy.
