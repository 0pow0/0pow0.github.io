---
title: "Self-correction for LLMs"
math: true
---

# Review of Self-Correction for LLMs

[1] distinguishes two types of self-correction based on the **source of feedback**:  
(1) **Intrinsic** and (2) **External**.

[2] and [3] belong to intrinsic self-correction, where the domain provides **ground-truth supervision** (i.e., *oracle labels*) that can be leveraged during training.

According to [1], when these oracle labels are **not available**, the performance improvements of intrinsic self-correction **disappear**, which contrasts with [2] and [3], where such labels are present and yield gains.

Building on [1], [4] excludes not only **external feedback** but also limits **multi-round iterative prompting**, which could otherwise hint to the model that its prior response was incorrect.  
Instead, [4] replaces this with **sampling multiple independent responses**.

[1] further re-evaluates [4] under the setting where **ground truth is unavailable**, requiring LLMs to **decide independently when to stop the self-correction process**—for example, whether to retain or revise their previous answers.  
The results show that in this setting, **the improvements disappear**, suggesting that LLMs cannot truly self-correct without external or oracle guidance.

---

## Self-Consistency vs. Self-Correction

**Self-consistency** can be viewed as a “majority vote” mechanism — generating multiple samples and selecting the most consistent outcome across them.  
**Self-correction**, in contrast, involves iterative reflection and revision of previous outputs.

---

### References

[1] Huang, Jie, et al. *"Large Language Models Cannot Self-Correct Reasoning Yet."* arXiv preprint arXiv:2310.01798 (2023).  

[2] Geunwoo Kim, Pierre Baldi, and Stephen McAleer. *"Language Models Can Solve Computer Tasks."* Advances in Neural Information Processing Systems, 2023.  

[3] Noah Shinn, Federico Cassano, Beck Labash, Ashwin Gopinath, Karthik Narasimhan, and Shunyu Yao. *"Reflexion: Language Agents with Verbal Reinforcement Learning."* Advances in Neural Information Processing Systems, 2023.  

[4] Li, Yanhong, Chenghao Yang, and Allyson Ettinger. *"When Hindsight is Not 20/20: Testing Limits on Reflective Thinking in Large Language Models."* arXiv preprint arXiv:2404.09129 (2024).  

[5] Wang, Xuezhi, et al. *"Self-Consistency Improves Chain-of-Thought Reasoning in Language Models."* arXiv preprint arXiv:2203.11171 (2022).
