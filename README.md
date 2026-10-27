# Shaji Sivaraman

**Forward Deployed Engineer · Enterprise AI · Microsoft**

I work with customers to turn business problems into software their teams can use. My work spans AI agents, enterprise integrations and the engineering around them: authentication, state, orchestration, deployment and validation.

Before Microsoft, I was a product manager at Amazon, Skyscanner and SAP, working on ML systems, developer tooling and enterprise applications. That experience shapes how I build: understand the workflow, make the trade-offs explicit, and connect the implementation to a useful outcome.

[LinkedIn](https://www.linkedin.com/in/shajisivaraman/)

## Selected engineering work

### Financial statement processing

A PDF-to-Excel workflow for credit analysts, connecting a Python extraction pipeline, asynchronous Azure Functions, Copilot Studio and a Power Apps review interface.

The implementation separates long-running extraction from synchronous connector calls and provides structured statements for analyst review. My accompanying sample was **merged into the PnP Microsoft 365 Copilot community repository**.

[Implementation and setup](https://github.com/sgshaji/AI-Finance-Statement-Extractor) · [Accepted contribution](https://github.com/pnp/copilot-pro-dev-samples/pull/138)

### Private-network agent integration

A Python A2A broker and Terraform infrastructure connecting Copilot Studio to a private Foundry backend.

The design separates public agent discovery from authenticated invocation, uses managed identity for Azure access, and reaches the backend through private endpoints. The repository includes the infrastructure, application code, integration findings and deployment instructions.

[Implementation](https://github.com/sgshaji/mcs-azure-foundry-a2a-vnet) · [Architecture and findings](https://github.com/sgshaji/mcs-azure-foundry-a2a-vnet/blob/main/docs/architecture.md)

### Agent capability validation

Python tooling for testing what an agent can actually use, beyond whether a file upload succeeds.

Controlled test artefacts, independently generated canaries and scoped evidence ledgers support reproducible boundary experiments. The tooling has a standard-library test suite and passing CI; live platform results are recorded separately for the environment and path tested.

[Methodology and implementation](https://github.com/sgshaji/copilot-studio-limits-validator) · [Tests](https://github.com/sgshaji/copilot-studio-limits-validator/tree/main/tests) · [CI](https://github.com/sgshaji/copilot-studio-limits-validator/actions/workflows/test.yml)

## Further work

- **[SharePoint document regeneration](https://github.com/sgshaji/file-iterator):** large-library investigation, dry-run cost gates, generated orchestration and explicit conversion outcomes. In development; tenant execution remains unverified.
- **[RetailDaddy](https://github.com/sgshaji/RetailDaddy):** mobile retail sales and inventory workflows with React and Supabase.
- **[PlanProof](https://github.com/sgshaji/PlanProof):** collaborative planning-application validation with document analysis, rules, evidence-linked findings and human review.

## Open-source contributions

| Work | Evidence |
|---|---|
| Copilot Studio financial-statement agent | [Merged into PnP](https://github.com/pnp/copilot-pro-dev-samples/pull/138) |
| Financial Statement Intelligence skill | [Submission](https://github.com/microsoft/cat-agent-skills/pull/387) |
| LLMDriftTracker Python compatibility and null-handling fixes | [Open pull request](https://github.com/kaul-vineet/LLMDriftTracker/pull/2) |

**Tools I work with:** Python, TypeScript/JavaScript, APIs, Azure Functions, Foundry, Copilot Studio, Microsoft 365, Terraform, A2A and MCP.

Interested in enterprise AI delivery, agent interoperability and evaluation? [Connect on LinkedIn](https://www.linkedin.com/in/shajisivaraman/), or open an issue on the relevant project.
