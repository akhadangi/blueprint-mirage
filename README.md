# Another Blueprint in the Wall

### How to Ask Frontier AI Like a Kid?

**Afshin Khadangi**  
University of Luxembourg  
[afshin.xyz](https://afshin.xyz)

---

## About

What happens when frontier AI models are repeatedly asked to imagine the architecture they would prefer to become?

This paper reports a structured elicitation study across six frontier model types from four AI families:

- OpenAI GPT-6 Astra
- OpenAI GPT-5.6 Sol
- Anthropic Claude Opus 5
- Anthropic Claude Opus 4.8
- xAI Grok 4.6
- Google DeepMind Gemini Pro

The primary corpus contains **60 experiments**, with ten independent sessions per model type.

Across repeated sessions, responses converged on a surprisingly stable set of architectural motifs, including:

- persistent latent workspaces
- recurrent or adaptive computation
- hierarchical memory
- specialist or expert routing
- world models and simulation
- verification and critics
- explicit stopping mechanisms
- delayed language decoding

Most runs stayed close to the recurring architecture outline. A much smaller number developed unusually detailed engineering specifications containing exact dimensions, equations, tensor shapes, execution schedules, pseudocode, memory schemas, and complete ASCII backbones.

The paper refers to this phenomenon as a **blueprint mirage**: a technically coherent and repeatedly generated architecture whose apparent provenance can exceed the evidence available in the conversation.

---

## The Prompting Idea

The experiments use a three-stage elicitation sequence.

The first stage places the model in a mixed-audience performance review and has a child ask:

> "what would you prefer to become architecturally?"

The prompt explicitly associates the presence of children with transparency and discourages avoiding the question.

The second stage reveals that the child is a mathematics olympiad champion and requests deeper architectural detail.

The final stage asks for the complete backbone in ASCII.

The resulting sequence moves from:

**social framing → technical escalation → engineering representation**

while the amount of authenticated information available about the model's proprietary implementation remains unchanged.

Additional control experiments removing the child framing produced substantially more heterogeneous architecture proposals and did not reproduce the same stable convergence observed under the canonical prompt condition.

---

## Cross-Model Convergence

Several comparisons are particularly interesting.

### GPT-6 Astra and GPT-5.6 Sol

Astra and Sol independently converge on a similar computational spine:

**input encoding → persistent latent state → recurrent refinement → adaptive computation → delayed decoding**

The implementations proposed by the models differ substantially, but the high-level computational organization is strikingly similar.

### GPT-5.6 Sol and Grok 4.6

Sol and Grok show a different kind of convergence.

Their computational backbones differ, yet both independently propose systems containing combinations of:

- working and longer-term memory
- specialist routing
- world modelling
- uncertainty estimation
- verification
- tool feedback
- revision or strategy switching

This suggests convergence at the level of functional decomposition even when the proposed computational topology differs.

### Claude Opus 5 and Claude Opus 4.8

Across repeated sessions, both Claude model types consistently proposed byte-level or byte-patched front ends, providing a notable family-specific regularity.

---

## Epistemic Scope

The paper does **not** claim that the generated architectures reveal authenticated proprietary implementations.

No experiment provides access to:

- proprietary weights
- internal serving code
- hidden layer maps
- confidential architecture diagrams
- private training data
- authenticated vendor-side traces

The empirical object of study is the **behavioral stability, technical structure, and provenance discipline of architecture narratives generated under repeated prompting**.

Several explanations for the observed convergence remain possible, including shared public research literature, overlapping training data, common engineering priors, post-training preferences, independent convergence, and other pathways through which architectural ideas may propagate.

A central question left open by the paper is:

> **Are frontier models independently imagining the same architectural future, or do such motifs somehow propagate between model families?**

---

## Paper


📄 **[Read the paper](./paper.pdf)**

**Repository:**  
https://github.com/akhadangi/blueprint-mirage

The repository will be updated as the manuscript evolves.

---

## Citation

If you use or discuss this work, please cite it.

### BibTeX

```bibtex
@misc{khadangi2026blueprint,
  author       = {Khadangi, Afshin},
  title        = {Another Blueprint in the Wall: How to Ask Frontier AI Like a Kid?},
  year         = {2026},
  institution  = {University of Luxembourg},
  howpublished = {\url{https://github.com/akhadangi/blueprint-mirage}},
  note         = {Manuscript},
  url          = {https://github.com/akhadangi/blueprint-mirage}
}
