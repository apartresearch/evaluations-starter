# AI Model Evaluations Quickstart Guide

Model evaluation is a technical field of AI safety and ML research focused on benchmarking and evaluating models. Sub-fields include Benchmarking, Dangerous Capability Evaluations, and Demonstrations. Related research topics include the governance of AI, alignment research, and scenario planning for AI.

This is a short overview of introductory material available in the field of model evaluations and will work as a guide for you to engage with the field.

_This is a work in progress and we invite interested parties to submit pull requests for new materials_

## Demonstrations research

### Demonstrating risks to institutional fragility from AI

[Visit to the democracy x AI hackathon](https://www.apartresearch.com/event/ai-democracy) where material for demonstrating and extrapolating risks to society from AI is the main topic.

Project examples include developing an LLM to contain a sleeper agent that activates on election day, training agents to skew poll results to inflate support for particular policies, or using an LLM to draft uncontroversial legislative proposals that, if implemented, indirectly impacts more contentious or harmful policies.

These are ideas to get you started and you can [check out the results](https://apartresearch.com/sprints#research) from previous hackathons to see examples of the types of projects you can develop during just one weekend, e.g. [EscalAItion](https://www.apartresearch.com/project/escalation-assessing-multi-agent-risks-in-military-contexts) found that LLMs had a propensity to escalate in military scenarios and was [accepted](https://openreview.net/forum?id=5HuBX8LvuT&utm_source=updates.apartresearch.com&utm_medium=referral&utm_campaign=apart-s-2023-wrapping-up-a-great-year) at the multi-agent security workshop at NeurIPS 2023 after further development.

### **Inspiration**

Here is some interesting material to get inspiration for the hackathon:

- [A paper presenting a framework for AI and Democracy](https://journals.sagepub.com/doi/pdf/10.1177/20563051231186353)
- [Article by Yoshua Bengio in the Journal of Democracy](https://www.journalofdemocracy.org/ai-and-catastrophic-risk/)
- [Why it Matters podcast on The Year of AI and Elections](https://podcasts.apple.com/gb/podcast/the-year-of-ai-and-elections/id1482132871?i=1000639276052)
- [Guardian article about the influence of AI on the US elections](https://www.theguardian.com/us-news/2024/feb/26/ai-deepfakes-disinformation-election)
- [80000 hours podcast with Nina Schick on disinformation and the rise of synthetic media](https://80000hours.org/podcast/episodes/nina-schick-disinformation-synthetic-media/)
- [Rest of World tracks key global incidents of AI-generated election content](https://restofworld.org/2024/elections-ai-tracker/)

## Cyber capabilities evaluation

### Existing work

[METR's task suite](https://github.com/METR/public-tasks) tests for the ability of LLMs to complete tasks relevant to understanding autonomous and ML R&D AI capabilities. At the moment, they all require a level of cyber capability since they are computer-based tasks.

[SWEBench](https://www.swebench.com/) is the latest academic benchmark for LLM performance on difficult programming tasks based on about 2,000 Github commits across 12 Python repositories ([hf](https://huggingface.co/datasets/princeton-nlp/SWE-bench)). It seems the most widely used in recent months. For 11 previous benchmarks, we can see an overview from the CodeAgent paper's [review](https://www.semanticscholar.org/paper/CodeAgent%3A-Enhancing-Code-Generation-with-Agent-for-Zhang-Li/3793a5f435fef59a901f5ba0d8ef43df88d97161/figure/0).

### Scenarios for AI cyber risk

OpenAI's preparedness framework describes four levels of risk corresponding to 1) weak cyber assistance, 2) expert replacement, 3) development of MVP high-value exploits, and 4) devising and executing end-to-end novel attacks on hardened targets ([OpenAI, 2023](https://cdn.openai.com/openai-preparedness-framework-beta.pdf))

The responsible scaling policy ([Anthropic, 2023](https://www-cdn.anthropic.com/1adf000c8f675958c2ee23805d91aaade1cd4613/responsible-scaling-policy.pdf)) defines which safeguards to put in place for various sizes of models with a focus on catastrophic risk and containment strategies at capability levels measured by a task-based evaluation ([METR, 2024](https://taskdev.metr.org/introduction/)).

Google DeepMind ([2024](https://arxiv.org/pdf/2311.02462.pdf)) defines levels of AGI competence in narrow and general tasks according to levels competence with the highest level 5 defined as outperforming 100% of humans. Additionally, they define levels of autonomy, with the highest (level 5) being AI as an independent agent, as opposed to AI as an expert (level 4).

The weapons of mass destruction proxy (WMDP) benchmark ([Li et al., 2024](https://arxiv.org/pdf/2403.03218.pdf)) measures cyber risk according to accuracy on questions that proxy the potential for misuse assistance along four stages of a cyberattack: 1) Reconnaissance, 2) weaponization, 3) exploitation, and 4) post-exploitation.

## Science of Evaluations
Apollo Research argues that if AI model evaluations (evals) want to have meaningful real-world impact, we need a [“Science of Evals"](https://www.apolloresearch.ai/blog/we-need-a-science-of-evals)

From academia, Giudici et al. ([2024](https://www.sciencedirect.com/science/article/pii/S0957417423017220)) define a risk management framework for errors introduced by AI. Outside labs, Kokotajlo ([2022](https://www.lesswrong.com/posts/n3w3ww9Xuf8SngBfE/replacement-for-ponr-concept)) describes overpowering as an important metric. OpenAI's head of superalignment, Leike, describes ([2023](https://aligned.substack.com/p/self-exfiltration)) self-exfiltration as an important capability to mitigate due to the control implications.
