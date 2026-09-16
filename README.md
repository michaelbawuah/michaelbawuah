<p align="center">
  <img src="./assets/hero.svg" width="100%" alt="Michael Baffour Awuah — AI/ML Systems Engineering"/>
</p>

<div align="center">

### Building the systems behind intelligent software.

**AI/ML Systems • Software Engineering • ML Infrastructure • Applied AI**

Cornell Engineering · Boston, USA

</div>

---

## 👋 About Me

I'm **Michael Baffour Awuah**, a Cornell Engineering student interested in understanding and building the systems that make modern AI work.

My work spans the ML stack — from **retrieval systems and deep-learning framework internals** to **model serving, inference infrastructure, observability, and production ML systems**.

Previously, I worked at **Microsoft as a Software Engineer Intern — AI Observability & Agent Evaluation**.

I'm especially interested in what happens **underneath and around the model**:

```text
research → frameworks → runtimes → inference → observability → production
```

I like building things deeply enough to understand where the abstractions come from.

---

## 💼 Experience & Leadership

<table>
<tr>
<td width="50%" valign="top">

### Microsoft

**Software Engineer Intern**
*AI Observability & Agent Evaluation*

</td>
<td width="50%" valign="top">

### Cornell Engineering

**Engineering Ambassador**

Representing Cornell Engineering and supporting its student and prospective-student community.

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Cornell University

**Orientation Leader**

Helping incoming students navigate their transition into the Cornell community.

</td>
<td width="50%" valign="top">

### Cornell Bowers CIS

**Finance & Programming Assistant**

Supporting programming, operations, and financial work within Cornell Bowers Computing and Information Science.

</td>
</tr>
</table>

---

## 🧠 Building the ML Stack

I'm deliberately building projects at different layers of the machine-learning systems stack.

```text
                  RESEARCH
                     │
                     ▼
              ┌─────────────┐
              │   ToolRet   │
              │  Retrieval  │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │   Fluxion   │
              │ ML Framework│
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │ ModelForge  │
              │ ML Platform │
              └──────┬──────┘
                     │
                     ▼
              ┌─────────────┐
              │   Edge AI   │
              │  Robotics   │
              └─────────────┘
                     │
                     ▼
                 REAL WORLD
```

The goal isn't simply to collect projects. It's to understand how the pieces of an intelligent system connect.

---

# 🚀 Featured Engineering Projects

## 01 — ModelForge

### Reliability-aware production ML infrastructure

**ModelForge** explores what happens after a model has been developed: how models are versioned, deployed, served, monitored, updated, and safely rolled back.

`ML Infrastructure` · `Inference Serving` · `Reliability` · `Systems Engineering`

**Built so far:**

- Versioned model registry backed by MySQL
- Immutable artifact management with SHA-256 verification
- Transactional deployment lifecycle
- Environment-aware deployment targets
- Promotion and rollback semantics
- Integrity-aware cached inference serving
- PyTorch and ONNX runtime support
- Extensible runtime plugin architecture
- Serving observability and readiness
- Isolated external runtime execution
- Cross-language Go inference runtime

```text
                         ModelForge API
                              │
             ┌────────────────┼────────────────┐
             │                │                │
             ▼                ▼                ▼
       Model Registry   Deployment State  Observability
             │                │
             └───────────┬────┘
                         ▼
                  Runtime Resolver
                         │
                 ┌───────┴───────┐
                 ▼               ▼
            In-Process        External
              Runtime          Runtime
            ┌────┴────┐           │
         PyTorch     ONNX          ▼
                         Go Runtime Service
                                  │
                                  ▼
                              Prediction
```

**Currently building:** reproducible multi-service deployment, runtime resilience, and performance benchmarking.

---

## 02 — Fluxion

### Deep-learning framework internals from first principles

**Fluxion** is my exploration of what exists underneath modern deep-learning frameworks.

Rather than starting with high-level neural-network APIs, I built upward from tensors and automatic differentiation.

`Deep Learning Systems` · `Autograd` · `Transformers` · `Performance`

**Implemented:**

- Tensor abstraction and computational graphs
- Reverse-mode automatic differentiation
- Gradient accumulation
- NumPy-style broadcasting and reductions
- Batched matrix multiplication
- Neural-network module system
- Linear layers, activations, and losses
- SGD and Adam
- Layer normalization and embeddings
- Scaled dot-product and multi-head attention
- Causal self-attention
- Transformer blocks
- GPT-style language model
- Character-level training and generation
- PyTorch numerical validation
- CPU profiling and performance analysis
- Portable C++/BLAS backend
- Experimental CUDA Linear backend

**Current validation:** `72 passed · 2 CUDA-only tests skipped on macOS`

Fluxion taught me that **using an ML framework and understanding one are very different things**.

---

## 03 — ToolRet

### Hybrid retrieval research for large tool collections

**ToolRet** investigates retrieval over a corpus of **37,292 tools**, combining sparse retrieval, dense representation learning, fusion, and reranking.

`Information Retrieval` · `Representation Learning` · `Evaluation`

```text
                         Query
                           │
                  ┌────────┴────────┐
                  ▼                 ▼
                 BM25             MiniLM
             Sparse Search      Dense Search
                  │                 │
                  └────────┬────────┘
                           ▼
                Reciprocal Rank Fusion
                           │
                           ▼
                  Candidate Ranking
                           │
                           ▼
                Cross-Encoder Reranker
```

**Experiments included:**

- BM25 sparse retrieval
- MiniLM dense retrieval
- Reciprocal Rank Fusion
- Weighted RRF
- Hard-negative mining
- Dense retriever fine-tuning
- Cross-encoder reranking
- Frozen-test failure analysis

The project also reinforced an important research lesson: **negative results are still results**. When reranking did not consistently improve the frozen test set, I analyzed and documented the failure cases rather than hiding them.

---

## 04 — Edge AI / Robotics

### Next frontier

The next layer of my systems roadmap moves inference from servers toward **real-time physical systems**.

I'm interested in exploring:

- On-device inference
- Latency-constrained ML
- Sensor pipelines
- Model optimization
- Edge deployment
- Robotics
- Real-time systems

```text
MODEL → OPTIMIZE → DEPLOY → SENSE → INFER → ACT
```

---

## 🛠 Engineering Toolkit

<table>
<tr>
<td width="33%" valign="top">

### Languages

- Python
- Java
- C++
- Go
- SQL

</td>
<td width="33%" valign="top">

### AI / ML

- PyTorch
- ONNX
- Transformers
- Autograd
- Retrieval Systems
- Model Evaluation
- Inference Systems

</td>
<td width="33%" valign="top">

### Systems

- FastAPI
- MySQL
- Docker
- Linux
- Git / GitHub
- REST APIs
- Native C++ extensions
- CUDA experimentation

</td>
</tr>
</table>

---

## 🔬 Current Interests

I'm particularly interested in:

**ML Systems Engineering · AI Infrastructure · Inference · AI Observability & Evaluation · Distributed Model Execution · Performance Engineering · Reliable Production AI**

A question that keeps showing up across my work is:

> **What has to happen around a model for it to become a reliable real-world system?**

That question has taken me from retrieval research → autograd → transformers → native backends → deployment → inference runtimes → observability.

---

## 🧭 Engineering Principles

```text
01  Build below the abstraction.
02  Measure before claiming performance.
03  Treat failures as engineering evidence.
04  Prefer systems that fail safely.
05  Understand why the architecture exists.
06  Keep learning by building.
```

---

## 🌍 Beyond Engineering

I'm based in **Boston, USA**, with **Ghanaian roots 🇬🇭**, and study at **Cornell University**.

Beyond technical work, I care about leadership, mentorship, education, and building communities where people can grow.

At Cornell, I've served across engineering outreach, student orientation, programming, and operational roles while continuing to develop as an engineer.

---

## 📫 Let's Connect

I'm always interested in conversations around **AI systems, ML infrastructure, software engineering, research, and open source**.

<p align="center">
  <b>Build deeply. Measure honestly. Understand the system.</b>
</p>

<p align="center">
  <sub>Michael Baffour Awuah · Cornell Engineering</sub>
</p>