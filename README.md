# ECZ-ID MCP Security Toolkit

## Know what your MCP can do before you let it act.

Free, practical MCP security resources from EcoCitizenz Ltd / ECZ-ID.

### Start here

[**Install MCP Trust Free**](https://marketplace.visualstudio.com/items?itemName=ecocitizenz.eczid-mcp-trust)

[**Download the MCP & AI Agent Trust Preflight**](https://developers.ecocitizenz.com/downloads/eczid-mcp-agent-trust-preflight.pdf?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=preflight)

[**Explore MCP Trust Pro**](https://developers.ecocitizenz.com/mcp-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=pro)

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

---

## MCP Trust Pro

MCP Trust Pro adds deeper local history and supported local runtime controls including Trust Epochs, Advanced Tool X-Ray, deterministic local policy, remediation and optional Local Trust Gate mediation.

[Explore MCP Trust Pro →](https://developers.ecocitizenz.com/mcp-trust?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=get-pro)

---

## Organisation or enterprise requirement?

For teams requiring professional assessment, migration or enterprise implementation:

[Explore MCP Readiness Services →](https://mcp.ecocitizenz.com?utm_source=github&utm_medium=repository&utm_campaign=mcp-security-toolkit&utm_content=audit)

---

## Public operator proof

**ECZ-ID ✓ VERIFIED — ECZ-GB-RBS1NW**

[View current public identity & evidence →](https://resolver.ecocitizenz.org/passport/ECZ-GB-RBS1NW)

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
  uses: Ecocitizenz/ecz-id-mcp-verifier@v0.8.2
  with:
    target: ECZ-GB-RBS1NW
    policy: PREFER
```

[ECZ-ID MCP Verifier source and usage](https://github.com/Ecocitizenz/ecz-id-mcp-verifier)

The verifier reads and reports public Resolver posture. It does not inspect arbitrary target contents or replace your local policy.
