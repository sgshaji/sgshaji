# Shaji Sivaraman

**Forward-deployed engineering for enterprise AI.**

I build applications around business workflows and the integration layers that make them useful: financial-document processing, agent orchestration, private-network connectivity, and evidence-driven validation.

The work below connects a concrete problem to implementation, engineering trade-offs, and inspectable evidence.

## Selected work

### Financial statement processing

**Problem:** turn PDF financial reports into structured statements and Excel workbooks that an analyst can review.

**Implementation:** a Python extraction pipeline, asynchronous Azure Functions, a Copilot Studio conversation, and a Power Apps review interface. Long-running extraction is separated from the connector's synchronous request.

**External contribution:** my [finance-statement agent sample](https://github.com/pnp/copilot-pro-dev-samples/tree/main/samples/mcs-finance-statement-agent) was [merged into the PnP community samples](https://github.com/pnp/copilot-pro-dev-samples/pull/138) on 11 May 2026.

[Source and setup](https://github.com/sgshaji/AI-Finance-Statement-Extractor) | [Pipeline and tests](https://github.com/sgshaji/AI-Finance-Statement-Extractor/tree/main/azure-functions)

### Private-network agent integration

**Problem:** connect an external agent client to a Foundry agent without making the Foundry resources and data stores publicly reachable.

**Implementation:** Terraform infrastructure and a Python A2A broker with public discovery, authenticated invocation, managed identity, and VNet-integrated access to private endpoints.

**Engineering boundary:** the broker has public ingress; the Foundry backend remains private. The repository documents the integration decisions and deployment steps, rather than claiming that the whole system has no public surface.

[Source and deployment](https://github.com/sgshaji/mcs-azure-foundry-a2a-vnet) | [Architecture and integration findings](https://github.com/sgshaji/mcs-azure-foundry-a2a-vnet/blob/main/docs/architecture.md)

### Agent capability validation

**Problem:** a successful upload or a documented limit does not establish how much content an agent can actually use.

**Implementation:** controlled test artefacts, independent canaries, scoped evidence ledgers, boundary planning, and reports that distinguish measured results from assumptions.

**Verification:** a standard-library Python test suite and CI cover the tooling. Live platform measurements require their own isolated experiment and recorded scope.

[Source and methodology](https://github.com/sgshaji/copilot-studio-limits-validator) | [Tests](https://github.com/sgshaji/copilot-studio-limits-validator/tree/main/tests) | [CI](https://github.com/sgshaji/copilot-studio-limits-validator/actions/workflows/test.yml)

## More engineering work

- **[SharePoint document regeneration](https://github.com/sgshaji/file-iterator):** investigation and orchestration around large libraries, dry-run cost gates, explicit outcomes, and recovery. Static validation passes; tenant import and end-to-end execution remain unverified.
- **[RetailDaddy](https://github.com/sgshaji/RetailDaddy):** a mobile-first retail application for products, sales, and inventory, using React and Supabase.
- **[PlanProof](https://github.com/sgshaji/PlanProof):** a collaborative planning-application validation project combining document analysis, rules, evidence-linked findings, and human review.

## Upstream contributions

| Contribution | Evidence |
|---|---|
| Finance-statement agent sample | [Merged PR](https://github.com/pnp/copilot-pro-dev-samples/pull/138) |
| Financial Statement Intelligence skill | [Submitted PR](https://github.com/microsoft/cat-agent-skills/pull/387) |
| Python compatibility and null-handling fixes for LLMDriftTracker | [Submitted PR](https://github.com/kaul-vineet/LLMDriftTracker/pull/2) |

Submission states were checked on 27 October 2026. A submission is not an accepted contribution; a merged sample is not evidence of production adoption.

## Engineering focus

- **Build:** Python, TypeScript/JavaScript, APIs, document-processing pipelines, and review interfaces.
- **Integrate:** Copilot Studio, Microsoft 365, Azure Functions, Foundry, A2A, and MCP.
- **Deliver responsibly:** infrastructure as code, explicit authentication boundaries, bounded workflows, and reproducible validation.

I welcome practical discussions about enterprise AI delivery, agent integration, and evaluation. Repository issues are a good place to discuss a specific implementation or trade-off.
