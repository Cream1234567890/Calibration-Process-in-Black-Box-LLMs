# Calibration Process in Black-Box LLMs
> Given the vague definitions of Calibration methods in recent research literature, we have defined the concept of the Calibration Process. It includes three steps: Confidence Estimation, Calibration Error Measurement, and Calibration Alignment.

:smile: This repository collects recent papers on Confidence Estimation, Calibration Error Measurement, and Calibration Alignment in black-box LLMs.

:star: At the same time, we have organized these methods in black-box models into a survey paper.
## Content

---
- [Calibration Process in Black-Box LLMs](#calibration-process-in-black-box-llms)
  - [Content](#content)
  - [Papers](#papers)
    - [:paperclip:Confidence Estimation Methods](#paperclipconfidence-estimation-methods)
      - [:book:Consistency Methods](#bookconsistency-methods)
      - [:book:Self-Reflection Methods](#bookself-reflection-methods)
      - [:book:Hybrid Methods](#bookhybrid-methods)
    - [:paperclip:Calibration Error Measurement Methods](#paperclipcalibration-error-measurement-methods)
    - [:paperclip:Calibration Alignment Methods](#paperclipcalibration-alignment-methods)

## Papers
### :paperclip:Confidence Estimation Methods
#### :book:Consistency Methods
- [[paper]](https://arxiv.org/abs/2303.08896)SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models`(2023)`[[code]](https://github.com/potsawee/selfcheckgpt)
- [[paper]](https://aclanthology.org/2023.trustnlp-1.28/)Strength in Numbers: Estimating Confidence of Large Language Models by Prompt Agreement`(2023)`[[code]](https://github.com/JHU-CLSP/Confidence-Estimation-TrustNLP2023)
- [[paper]](https://arxiv.org/abs/2406.04370)Large Language Model Confidence Estimation via Black-Box Access`(2024)`
- [[paper]](https://arxiv.org/abs/2305.19187)Generating with Confidence: Uncertainty Quantification for Black-box Large Language Models`(2023)`[[code]](https://github.com/zlin7/UQ-NLG)
- [[paper]](https://arxiv.org/abs/2405.20003)Kernel Language Entropy: Fine-grained Uncertainty Quantification for LLMs from Semantic Similarities`(2024)`
- [[paper]](https://aclanthology.org/2024.findings-acl.728/)Bayesian Prompt Ensembles: Model Uncertainty Estimation for Black-Box Large Language Models`(2024)`[[code]](https://github.com/amzn/BayesPE)
- [[paper]](https://arxiv.org/abs/2306.13063)Can LLMs Express Their Uncertainty? An Empirical Evaluation of Confidence Elicitation in LLMs`(2023)`[[code]](https://github.com/MiaoXiong2320/llm-uncertainty)
- [[paper]](https://arxiv.org/abs/2403.20279)LUQ: Long-text Uncertainty Quantification for LLMs`(2024)`[[code]](https://github.com/caiqizh/LUQ)
#### :book:Self-Reflection Methods
- [[paper]](https://arxiv.org/abs/2403.09972)Think Twice Before Trusting: Self-Detection for Large Language Models through Comprehensive Answer Reflection`(2024)`
- [[paper]](https://arxiv.org/abs/2401.02009)Self-Contrast: Better Reflection Through Inconsistent Solving Perspectives`(2024)`
- [[paper]](https://arxiv.org/abs/2402.12563)Confidence Matters: Revisiting Intrinsic Self-Correction Capabilities of Large Language Models`(2024)`[[code]](https://github.com/MBZUAI-CLeaR/IoE-Prompting)
- [[paper]](https://aclanthology.org/2024.findings-acl.515/)Fact-and-Reflection (FaR) Improves Confidence Calibration of Large Language Models`(2024)`[[code]](https://github.com/colinzhaoust/fact-and-reflection)
#### :book:Hybrid Methods
- [[paper]](https://arxiv.org/abs/2308.16175)Quantifying Uncertainty in Answers from any Language Model and Enhancing their Trustworthiness`(2023)`
- [[paper]](https://arxiv.org/abs/2311.08877)Llamas Know What GPTs Don't Show: Surrogate Models for Confidence Estimation`(2023)`
- [[paper]](https://aclanthology.org/2024.acl-long.824/)Calibrating Large Language Models Using Their Generations Only`(2024)`[[code]](https://github.com/parameterlab/apricot)
- [[paper]](https://arxiv.org/abs/2311.01740)SAC3: Reliable Hallucination Detection in Black-Box Language Models via Semantic-aware Cross-check Consistency`(2023)`[[code]](https://github.com/intuit/sac3)
- [[paper]](https://arxiv.org/abs/2402.00367)Don't Hallucinate, Abstain: Identifying LLM Knowledge Gaps via Multi-LLM Collaboration`(2024)`[[code]](https://github.com/BunsenFeng/AbstainQA)
- [[paper]](https://arxiv.org/abs/2402.06544)Calibrating Long-form Generations from Large Language Models`(2024)`[[code]](https://github.com/kkkevinkkkkk/calibration)
- [[paper]](https://arxiv.org/abs/2406.03441)Cycles of Thought: Measuring LLM Confidence through Stable Explanations`(2024)`
### :paperclip:Calibration Error Measurement Methods
|Error-Based Methods | Correlation-Based Methods |
|-------------|-------------|
| ECE, MCE, MacroCE, TL-ECE, smECE, Reliability Diagram(Visualization Tool), Brier Score, BSS, Quadratic Score, Logarithmic Score, NLL| AUROC, AUPRC, Weighted AUROC, AUARC, PCC, SCC, [RCE](https://arxiv.org/abs/2404.03163)`(2024)`[[code]](https://github.com/shuoli90/Rank-Calibration/tree/main)|
### :paperclip:Calibration Alignment Methods
- Post-Processing Based Methods
  - Histogram Binning: [[paper]](https://dl.acm.org/doi/10.1145/502512.502540)Learning and making decisions when costs and probabilities are both unknown`(2001)`
  - Isotonic Regression: [[paper]](https://pubmed.ncbi.nlm.nih.gov/22211175/)Smooth isotonic regression: a new method to calibrate predictive models`(2011)`
  - Multicalibration: [[paper]](https://arxiv.org/abs/1711.08513)Calibration for the (Computationally-Identifiable) Masses`(2018)`
  - Multicalibration: [[paper]](https://arxiv.org/abs/2404.04689)Multicalibration for Confidence Scoring in LLMs`(2024)`
- Third-Party Proxy Based Methods
  - Bayesian Calibration Network: [[paper]](https://www.tandfonline.com/doi/abs/10.1080/07350015.1996.10524625)A Bayesian Approach to Calibration.`(1996)`
  - Bayesian Calibration Network: [[paper]](https://arxiv.org/abs/2109.10092)Bayesian Confidence Calibration for Epistemic Uncertainty Modelling.`(2021)`[[code]](https://github.com/EFS-OpenSource/calibrationframework)
  - Auxiliary Calibration Model: [[paper]](https://aclanthology.org/2024.acl-long.824/)Calibrating Large Language Models Using Their Generations Only`(2024)`[[code]](https://github.com/parameterlab/apricot)
  - Auxiliary Calibration Model: [[paper]](https://arxiv.org/abs/2110.07586)Can Explanations Be Useful for Calibrating Black Box Models?`(2022)`[[code]](https://github.com/xiye17/InterpCalib)
  - Auxiliary Calibration Model: [[paper]](https://aclanthology.org/2024.acl-long.745/)LLM-Rubric: A Multidimensional, Calibrated Approach to Automated Evaluation of Natural Language Texts`(2024)`[[code]](https://github.com/microsoft/llm-rubric)
