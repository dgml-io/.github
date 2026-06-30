# `</> DGML` — the domain-native document format

**DGML** (Document Graph Markup Language) is a semantic XML representation of business documents. Where raw source files give you layout and pixels, DGML gives you meaning: tags that describe what each element *is* in the document's domain — a contract clause, an invoice line item, a policy definition — not how it appeared on the page.

The headline feature is **cross-document tag consistency**: documents of the same kind share the same semantic vocabulary. This is what separates DGML from a raw extraction or a structural transcription, and what makes it suitable for reasoning over a corpus rather than a single file.

A second fundamental property is **complete semantic preservation**. Traditional extraction pipelines make an irreversible upfront decision: choose the fields to pull, discard everything else. This works when the questions are known in advance. It fails the moment a new use case emerges — a regulatory change, a derivative product, a counterparty due diligence request — that requires a field no one thought to extract. DGML preserves the full semantic structure of the document: every element, every relationship, every typed value. Nothing is discarded. A document processed once remains fully queryable without going back to the source. This is not a feature of the tooling — it is a property of the format.

A third fundamental property is **document order with graph semantics**. Most graph formats treat documents as unordered collections of facts. But in business documents, order is meaning: definitions precede usage, clause sequence governs interpretation, provenance depends on exact position. DGML preserves document order as a first-class property of the format, while also representing relationships across elements and documents as a graph.

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
| [dgml-io/dgml](https://github.com/dgml-io/dgml) | Python reference implementation |
| [dgml-io/dgml.io](https://github.com/dgml-io/dgml.io) | Website source |

---

## Open standard

DGML is an open initiative founded by [Docugami](https://www.docugami.com) and [Inveniam](https://www.inveniam.io), **Apache 2.0 licensed**. The specification is live. The community is forming. A formal steering committee will be established to guide the evolution of the format, with representation from contributors and adopters.

There are two ways to participate — and organizations that do have real influence over what DGML becomes:

- **Shape the spec** — open an issue or discussion in [dgml-io/dgml-spec](https://github.com/dgml-io/dgml-spec) to propose a change, challenge a design decision, or bring a use case the founding organizations haven't encountered.
- **Build the implementation** — contribute to [dgml-io/dgml](https://github.com/dgml-io/dgml), the Python reference implementation. Use it, break it, improve it. The implementations that emerge from real use cases are what harden a standard.

- 📄 [Read the spec](https://github.com/dgml-io/dgml-spec/blob/main/spec.md)
- 💬 [Start a discussion](https://github.com/dgml-io/dgml-spec/discussions)
- 🌐 [dgml.io](https://dgml.io)
