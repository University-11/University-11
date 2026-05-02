```text
╔══════════════════════════════════════════════════════════════════════════════╗
║                                                                              ║
║      T  I  M  O  F  E  Y     B  O  R  I  S  E  N  K  O                      ║
║      ────────────────────────────────────────────────                        ║
║      data scientist · recommender systems · sequence models                  ║
║                                                                              ║
║      "just normal focusing"                                                  ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

```text
$ whoami
> timofey · @University-11 · "timmy university"
> writes the math first, then the code that obeys it
> pure python as reference, c++17 when the shape is settled
> no autograd until the math has earned it
```

---

```text
══════════════════════════════ current research ═══════════════════════════════
```

```text
┌─ 01 ──────────────────────────────────────────────────────────────────────────┐
│                                                                               │
│   GEOMEMORY KERNEL                                                            │
│   ─────────────────                                                           │
│   hyperbolic geometry · streaming personalization · cover-tree retrieval      │
│                                                                               │
│   A recsys kernel that treats users as trajectories on a Poincaré ball,       │
│   and splits "no interaction" into "exposed-but-rejected" vs                  │
│   "epistemically unknown". Online updates. No full retrain.                   │
│                                                                               │
│       d_c(x, y) = (2/√c) · artanh( √c · ‖(−x) ⊕_c y‖ )                        │
│                                                                               │
│   reference dataset .... MovieLens-1M                                         │
│   stack ................ pure python (ref) · c++17 (core)                     │
│                                                                               │
└───────────────────────────────────────────────────────────────────────────────┘
```

```text
┌─ 02 ──────────────────────────────────────────────────────────────────────────┐
│                                                                               │
│   SPECTRAL STATE MEMORY KERNEL                                                │
│   ────────────────────────────                                                │
│   linear-time scan · sparse associative memory · information-gain writes      │
│                                                                               │
│   A sequence core that splits long context into a stable spectral state       │
│   plus a small, event-triggered memory. No KV cache. No materialised          │
│   attention matrix. Memory writes only when description length drops.         │
│                                                                               │
│       x_{t+1}^(j) = λ_{t,j} · R(ω_j) · x_t^(j) + B_j · u_t                    │
│                                                                               │
│   reference datasets ... TinyStories (byte-level) · CIFAR-10 (patch stream)   │
│   stack ................ pure python · c++17 · int8 weights                   │
│                                                                               │
└───────────────────────────────────────────────────────────────────────────────┘
```

```text
┌─ 03 ──────────────────────────────────────────────────────────────────────────┐
│                                                                               │
│   SHEAF ENERGY KERNEL                                                         │
│   ───────────────────                                                         │
│   sparse constraint fields · equilibrium propagation · intrinsic auditing     │
│                                                                               │
│   Predictions as fixed points of a sparse local-energy system: each patch     │
│   / item / token is a stalk; restriction maps live on edges; the forward      │
│   pass is coordinate descent to a free equilibrium. Every prediction          │
│   decomposes into local violations you can actually read.                     │
│                                                                               │
│       E(h;θ) = Σ_v ‖W_v x_v − h_v‖² + Σ_{(u,v)} ‖R_{e,u} h_u − R_{e,v} h_v‖²  │
│                                                                               │
│   reference datasets ... CIFAR-10 (patch graph) · MovieLens-1M (bipartite)    │
│   stack ................ pure python · c++17 · CSR sparse                     │
│                                                                               │
└───────────────────────────────────────────────────────────────────────────────┘
```

---

```text
$ ls -la ./tools

  python ........ reference implementations, never the bottleneck
  c++17 ......... performance cores, fixed-point where it matters
  numpy ......... when nothing else will do
  pytorch ....... occasional, never structural
  langchain ..... for the agent-side projects
  jupyter ....... where ideas first survive contact with data
```

```text
$ ls -la ./fields

  recsys ........ ranking · retrieval · exposure · cold-start
  sequence ...... state-space · sparse memory · long-context economics
  geometric ml .. hyperbolic embeddings · sheaves · manifolds
  llm tooling ... rag · retrievers · agent memory
```

---

```text
$ ./contact

  github ........ @University-11
  status ........ listening more than posting
  open to ....... readers · collaborators · paper trades
```

---

> *"the next primitive is logic, not flops."*
