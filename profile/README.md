# `</> DGML` — the domain-native document format

**DGML** (Document Graph Markup Language) is an open standard for representing business documents as semantic XML. Where raw source files give you layout and pixels, DGML gives you meaning: tags that describe what each element *is* in the document's domain — not how it appeared on the page.

**The headline feature:** cross-document tag consistency. Documents of the same kind share the same semantic vocabulary. An agent that can query one contract's `<LiabilityCap>` can query the same element across a thousand contracts — identical logic, no per-document prompt engineering.

---

## Repositories

| Repo | Purpose |
|------|---------|
| [dgml-io/dgml](https://github.com/dgml-io/dgml) | Python reference implementation |
| [dgml-io/dgml-spec](https://github.com/dgml-io/dgml-spec) | Format specification — the community hub |
| [dgml-io/dgml.io](https://github.com/dgml-io/dgml.io) | Website source |

---

## Four layers. One coherent format.

| Layer | What it gives you |
|-------|------------------|
| **Semantic** | Tags that name what things *are* — fewer tokens, more signal |
| **Spatial** | `dg:origin` — pixel-precise coordinates back to the source page |
| **Attestation** | Element-level Proof of Origin on any external blockchain |
| **Readable** | Human-readable in any browser, zero extra tooling |

---

## Open standard

DGML is an open initiative founded by [Docugami](https://www.docugami.com) and [Inveniam](https://www.inveniam.io), **Apache 2.0 licensed**. The specification is live. The community is forming. A formal steering committee will be established to guide the evolution of the format, with representation from contributors and adopters.

- 📄 [Read the spec](https://github.com/dgml-io/dgml-spec/blob/main/spec.md)
- 💬 [Start a discussion](https://github.com/dgml-io/dgml-spec/discussions)
- 🌐 [dgml.io](https://dgml.io)
