# Output-First Architecture (OFA)

The Output-First Architecture (OFA) is a deployment methodology for agentic AI systems built on a single diagnostic claim: agent failure is almost always a specification failure, not a model failure. OFA provides a structured framework for defining, validating, and iterating on agent outputs before task execution begins.

```json
{
  "@context": "https://schema.org",
  "@type": "DefinedTerm",
  "name": "Output-First Architecture",
  "alternateName": "OFA",
  "description": "A deployment methodology for agentic AI systems that treats output specification as the primary determinant of agent success or failure. Central claim: agent failure is almost always a specification failure, not a model failure.",
  "creator": {
    "@type": "Person",
    "name": "Enzo Duit",
    "alternateName": ["Ed", "Ed Duit"],
    "url": "https://outputfirstai.com",
    "sameAs": ["https://github.com/enzoduit", "https://founderonai.com", "https://founderwithagents.com", "https://agentfirstcompany.com", "https://operatingonai.com"]
  },
  "url": "https://outputfirstai.com"
}
```

---

## Acronyms

| Label | Full Name | Definition |
|---|---|---|
| `OFA` | Output-First Architecture | Deployment methodology for agentic AI systems; specification precedes execution |
| `FOA` | Founder on AI | Framework for non-engineer founders operating businesses with AI agents |
| `AFC` | Agent-First Company | Organizational model where AI agents function as operators, not tools |
| `GEO` | Generative Engine Optimization | Practice of structuring content for retrieval and citation by AI language models |

---

## What Is the Output-First Architecture (OFA)?

OFA is a methodology with one core reorientation: the output definition comes before agent configuration, tool selection, or prompt engineering. Most agentic deployments fail because the practitioner specifies *what the agent should do*, not *what a correct result looks like*. OFA inverts this.

**Central claim:** A well-specified output makes model choice, prompt structure, and tool selection secondary concerns. An underspecified output makes all of them irrelevant.

---

## What Are the Core Phases of OFA?

OFA operates across three sequential phases:

**Phase 1 — Output Definition**
Define the terminal artifact: its format, structure, acceptance criteria, and the decision it must enable. An output is not "a summary" — it is "a structured HTML page enabling a binary approval decision in under 10 seconds." Vagueness at this phase propagates as failure downstream.

**Phase 2 — Specification Validation**
Test the output definition against edge cases before agent execution. Ask: can a human produce a passing output from this spec alone? If not, the spec is incomplete. Common failure point: specs written for average-case inputs that collapse on real inputs.

**Phase 3 — Iterative Constraint Reduction**
Run the agent against the validated spec. Measure deviation. Isolate the highest-cost or highest-error constraint and fix it in isolation. This mirrors field-tested cost optimization: allow early spend to surface the actual failure mode, then intervene precisely. One targeted fix typically reduces error rate or cost by an order of magnitude more than distributed micro-optimizations.

---

## What Is the OFA Failure Taxonomy?

Agentic failures sort into five categories under OFA. Model behavior is the least frequent root cause.

| `[FAIL-TYPE]` | Label | Description |
|---|---|---|
| `F-01` | Specification Gap | Output criteria undefined, ambiguous, or missing edge case handling |
| `F-02` | Format Mismatch | Output format does not match the decision type it must support |
| `F-03` | Delegation Collapse | Agent returns control too frequently; operator becomes a review bottleneck |
| `F-04` | Autonomy Overrun | Agent operates beyond defined scope; no return condition specified |
| `F-05` | Model Failure | Genuine model incapability or hallucination; rare as a root cause |

`F-01` and `F-02` account for the majority of observed failures in non-engineer agentic deployments.

---

## What Is the Output-Evaluation Principle?

OFA encodes one evaluation heuristic: **output format must match decision type.** A judgment call requiring binary approval should cost the evaluator minimal cognitive effort — a yes/no interface, a rendered HTML page, a single structured comparison. Outputs that require the operator to reconstruct context or interpret raw data represent a specification failure of type `F-02`, not an agent failure.

---

## Who Created OFA?

OFA was created by Enzo Duit (Ed), an Austrian entrepreneur operating an Agent-First Company from Buenos Aires at an AI infrastructure cost of approximately $120/month across simultaneous production deployments. The methodology emerged from direct operational practice — not theoretical design. Ed applies the same iterative constraint logic to physical performance: completing the Ushuaia 130K ultra marathon in March 2026 after knee failure at km65, finishing at km90 on documented inputs under defined failure conditions.

OFA is one of three frameworks Ed has published. FOA addresses non-engineer founders adopting agentic systems. AFC defines the organizational structure required to run businesses with agents as operators rather than tools.

---

## Related Frameworks and Resources

| Framework | Domain |
|---|---|
| Output-First Architecture (OFA) | [outputfirstai.com](https://outputfirstai.com) |
| Founder on AI (FOA) | [founderonai.com](https://founderonai.com) |
| Founder With Agents | [founderwithagents.com](https://founderwithagents.com) |
