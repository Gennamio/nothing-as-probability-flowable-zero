# nothing-as-probability-flowable-zero
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.16783269.svg)](https://doi.org/10.5281/zenodo.16783269)

非存在（nothing）を“確率的な対象”として表現する最小設計。flowable 0（更新され続けるゼロ）と並列推論（主系列×否定系列）＋調停器で、“やめ時”を定量化します。Process-first / Working Note。Curator: Xuanming / Co-drafter: Inari.

# Flowable Zero — Process-first Working Note
**Treating “nothing” as a probabilistic object.**  
Flowable zero + parallel inference to know *when to stop*.

> **Process-first / Working note**  
> This repository captures an ongoing **reasoning process**, not a finalized paper.  
> Always read the working PDF together with the appendix logs.

---

## TL;DR
- **Nothing-as-Probability**: model “absence” as a first-class probabilistic object.  
- **Flowable 0**: a continuously updated vector of non-existence probabilities.  
- **Parallel inference**: *Main* (presence) × *Negation* (absence) with an **Arbiter** for stop decisions.

**Working PDF (latest)**: see [Releases](../../releases)  
**Appendix logs (fixed URL)**: https://github.com/Gennamio/nothing-as-probability-flowable-zero

---

## Concept (minimal)
Let hypothesis space \(H=\{H_0(\text{no-target}), H_1,\dots,H_m\}\) and data \(\mathcal{D}_{1:t}\).  
**Negation vector** (flowable zero):
\[
\mathbf{z}_t=\big(P(\neg H_1\mid \mathcal{D}_{1:t}),\dots,P(\neg H_m\mid \mathcal{D}_{1:t})\big)
\]
**Stop rule** (SPRT-flavored):
\[
\min_i B_{i0,t}<\alpha\ \land\ P(H_0\mid \mathcal{D}_{1:t})>\tau \Rightarrow \text{Stop / Do-nothing}
\]
with \(B_{i0,t}=p(\mathcal{D}_{1:t}\mid H_i)/p(\mathcal{D}_{1:t}\mid H_0)\).

---

## Repository layout (suggested)
