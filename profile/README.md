# `</> DGML` — the domain-native document format

**DGML** (Document Graph Markup Language) is a semantic XML representation of business documents. Where raw source files give you layout and pixels, DGML gives you meaning: tags that describe what each element *is* in the document's domain — a contract clause, an invoice line item, a policy definition — not how it appeared on the page.

The headline feature is **cross-document tag consistency**: documents of the same kind share the same semantic vocabulary — what separates DGML from a raw extraction or structural transcription, and what makes it suitable for reasoning over a corpus rather than a single file.

The second property is **complete semantic preservation**. Traditional extraction pipelines choose fields upfront and discard the rest — a decision that fails the moment a new use case emerges and needs a field no one thought to extract. DGML preserves the full semantic structure instead — every element, relationship, and typed value — so a document processed once stays fully queryable without returning to the source.

The third is **document order with graph semantics**. Most graph formats treat documents as unordered collections of facts, but in business documents order is meaning: definitions precede usage, clause sequence governs interpretation, provenance depends on position. DGML preserves document order as a first-class property while also representing relationships across elements and documents as a graph.

The fourth is **attestation**: **Proof of Origin at the data-element level**. Every DGMLX package is tamper-evident — any alteration to its content breaks its cryptographic hash. The deeper innovation is that this hashing isn't limited to the whole document: because the semantic tree is structured, any XML element subtree — a single data point, a payment term, a liability cap — can be hashed and anchored on an external chain independently, proving its origin without producing the entire document.

---

## Four layers. One coherent format.

| Layer | What it gives you |
|-------|------------------|
| **Semantic** | Tags that name what things *are* — fewer tokens, more signal, no per-document prompt engineering |
| **Spatial** | `dg:origin` — pixel-precise coordinates back to the source page |
| **Attestation** | Element-level Proof of Origin on any external blockchain |
| **Readable** | Human-readable in any browser, zero extra tooling |

---

## Repositories

| Repo | Purpose |
|------|---------|
| [dgml-io/dgml-spec](https://github.com/dgml-io/dgml-spec) | Format specification — the community hub |
| [dgml-io/dgml-spec/samples](https://github.com/dgml-io/dgml-spec/tree/main/samples) | Samples of DGML files |
| [dgml-io/dgml](https://github.com/dgml-io/dgml) | Python reference implementation |
| [dgml-io/dgml.io](https://github.com/dgml-io/dgml.io) | Website source |

---

## Open standard

DGML is an open initiative founded by [Docugami](https://www.docugami.com) and [Inveniam](https://www.inveniam.io), **Apache 2.0 licensed**. The specification is live. The community is forming. A formal steering committee will be established to guide the evolution of the format, with representation from contributors and adopters.

There are two ways to participate:

- **Shape the spec** — open an issue or discussion in [dgml-io/dgml-spec](https://github.com/dgml-io/dgml-spec) to propose a change, challenge a design decision, or bring a use case the founding organizations haven't encountered.
- **Build the implementation** — contribute to [dgml-io/dgml](https://github.com/dgml-io/dgml), the Python reference implementation. Use it, break it, improve it. The implementations that emerge from real use cases are what harden a standard.

Organizations that participate now have real influence over what DGML becomes.
