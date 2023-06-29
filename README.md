# PULSE-COVID-19: A Large Language Model for knowledge extraction on COVID-19
<!-- select Model and/or Data and/or Code as needed>
### Welcome to OpenMEDLab! 👋

<!--
**Here are some ideas to get you started:**
🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->

<!-- Insert the project banner here -->

<p align="center" width="100%">
<img src="Images/BannerDesign.png" alt="MOSS" style="width: 100%; min-width: 350px; display: block; margin: 30px;">
</p>

[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-brightgreen.svg)](./LICENSE)
[![Model License](https://img.shields.io/badge/Model%20License-GNU%20AGPL%203.0-red.svg)](./MODEL_LICENSE)

This repository provides the official PyTorch implementation of the model **PULSE-COVID-19: A Large Language Model for knowledge extraction on COVID-19** <br>

## Introduction
This model was fine-tuned based on the [PULSE](https://github.com/openmedlab/PULSE) LLM, incorporating an in-house corpus of COVID-19 knowledge databases from the Guangzhou Laboratory. The objective was to augment the capabilities of LLMs in assimilating and responding to disease-specific knowledge. This enhanced understanding is expected to contribute towards future epidemic prevention and disease treatment efforts.

## Contributors
- Guangzhou Laboratory: [Yixue Li](https://scholar.google.com/citations?hl=en&user=Qv27G1cAAAAJ), [Feng Gao](https://scholar.google.com/citations?hl=en&user=deiLMp8AAAAJ), [Junwei Liu](https://scholar.google.com/citations?hl=en&user=VuuF5pIAAAAJ), Yiping Chen, Lu Zhou.

- Shanghai AI Laboratory: [Shaoting Zhang](https://scholar.google.com/citations?user=oiBMWK4AAAAJ&hl=en&oi=ao), [Xiaofan Zhang](http://www.qingyuan.sjtu.edu.cn/a/zhang-xiao-fan-1.html).

## Key Features
[//]: # (key feature bulletin points here)

- Developed a Large Language Model (LLM) specifically for the COVID-19 disease domain.
- Incorporated a comprehensive, in-house COVID-19 knowledge dataset from Guangzhou Laboratory.
- Provides more reliable question answering and knowledge extraction related to the COVID-19 epidemic and SARS-COV-2 virus.

<!-- [Code] may link to your project at your institute>
<!-- give a introduction of your project -->

## Details
> Large language models (LLMs) have demonstrated their promising performance in comprehending natural languages and adapting to multiple downstream tasks. Despite their robust generalized abilities, the use of LLMs in certain domains, notably in the medical and clinical fields, is limited due to the potential for inaccurate responses and incorrect knowledge extraction. The COVID-19 epidemic has had a global impact, causing millions of deaths and significantly affecting the world economy. As a response, scientists have carried out extensive basic and clinical research to understand the virological characteristics, mutational landscapes, and clinical aspects of the SARS-CoV-2 virus to aid in its diagnosis and treatment. This has resulted in thousands of scientific papers and the establishment of disease-specific regulatory mechanisms, presenting an opportunity for LLMs to fine-tune with these COVID-19-related datasets for reliable knowledge queries and responses. In this study, we combined the in-house COVID-19 disease knowledge datasets from our collaborator at Guangzhou Laboratory with our new LLM framework (PULSE), to construct a SARS-COV-2 disease-specific LLM model (PULSE-COVID-19). Our disease-specific LLM outperforms other existing LLMs of similar size of parameters in disease-related question answering and SARS-COV-2-related knowledge extraction, demonstrating the potential of applying LLMs in various specific domains.

## Get Started
### Installation
1. Download the contents of this repository to your local/remote server.

```bash
git clone https://github.com/openmedlab/PULSE-COVID-19
cd PULSE-COVID-19
```

2. Create a conda environment and install dependencies.

```bash
conda env create -f llm.yml
conda activate llm
```
### Evaluation

**Gradio**

```bash
python web_demo_gradio_gd.py
```

## COVID-19 Question Answering

---

**Q1: 新冠病毒感染人体细胞的基本原理是什么？**

新冠病毒感染人体细胞的基本原理是通过其表面的刺突蛋白（S蛋白）结合到人体细胞表面的ACE2蛋白上，从而进入细胞内部。ACE2蛋白是一种细胞膜上的受体蛋白，在人体内广泛分布，特别是在肺部和肾脏中。当新冠病毒与ACE2蛋白结合时，病毒会利用ACE2蛋白的转运机制进入细胞内部，并利用细胞内的酶系统复制自身。
在细胞内，新冠病毒利用细胞内的酶系统复制自身，并释放出病毒颗粒。这些病毒颗粒可以在细胞间传播，并感染其他细胞。此外，新冠病毒还可以通过飞沫传播、接触传播和空气传播等方式传播给他人。
总之，新冠病毒感染人体细胞的基本原理是通过其表面的刺突蛋白结合到人体细胞表面的ACE2蛋白上，从而进入细胞内部，利用细胞内的酶系统复制自身，并释放出病毒颗粒，在细胞间传播，并感染其他细胞。

---

---

**Q2: 为什么新冠病毒感染对有基础疾病的患者不友好？**

新冠病毒感染对有基础疾病的患者不友好的原因有以下几个方面：
1.免疫功能下降：基础疾病会导致患者的免疫功能下降，使得新冠病毒容易入侵体内并引起感染。
2.comorbidity：许多基础疾病都伴随着其他健康问题，这些健康问题可能会增加患者感染新冠病毒并出现严重后果的风险。
3.药物使用：某些药物可能会影响患者的免疫功能，或者与新冠病毒相互作用，增加感染的风险。
4.并发症：基础疾病往往会导致并发症，如高血压、糖尿病等，这些并发症可能会使患者更容易出现严重后果，如呼吸困难、心脏衰竭等。
因此，对于有基础疾病的患者，建议采取预防措施，如佩戴口罩、勤洗手、保持社交距离等，以减少感染新冠病毒的风险。如果出现发热、咳嗽、呼吸困难等症状，应及时就医。

---

---

**Q3: 如何定义新冠病毒变异株的致病力？**

新冠病毒变异株的致病力是指变异株引起疾病的能力。这可能涉及到变异株引起疾病的程度、严重程度、持续时间以及是否易于治疗等方面。
目前，科学家们使用多种方法来评估新冠病毒变异株的致病力。其中一种方法是使用临床表现来评估变异株引起的疾病严重程度。例如，一些研究使用临床症状的严重程度来评估变异株引起的疾病，包括发热、咳嗽、呼吸急促、乏力等症状的严重程度。
另一种方法是使用实验室检测来评估变异株引起的疾病。例如，一些研究使用细胞培养实验来评估变异株引起的病毒复制能力，或者使用动物实验来评估变异株引起的疾病严重程度。
此外，一些研究还使用流行病学方法来评估变异株的致病力。例如，一些研究使用追踪病例的方法来评估变异株引起的疾病传播速度和范围。
总之，评估新冠病毒变异株的致病力是了解变异株引起的疾病的重要一步，有助于制定更有效的预防和治疗方案。

---

---

**Q4: 人工智能方法在新冠疫情中发挥了什么作用？**

人工智能方法在新冠疫情中发挥了多种作用，包括：
1.病毒传播预测：利用机器学习算法，可以对新冠病毒传播进行预测，帮助政府制定更有效的防控措施。
2.病毒基因组测序：利用人工智能方法，可以快速、准确地对新冠病毒的基因组进行测序，加速病毒研究进程。
3.疫苗研发：利用人工智能方法，可以加速疫苗研发过程，提高疫苗研发成功率。
4.临床诊断：利用人工智能方法，可以辅助医生进行新冠病毒临床诊断，提高诊断准确率。
5.追踪接触者：利用人工智能方法，可以追踪新冠病毒接触者，帮助政府进行疫情防控。
总之，人工智能方法在新冠疫情中发挥了多种作用，为疫情防控提供了有力的支持。

---

## Note

Please note that certain responses or conclusions provided by this model regarding COVID-19-specific knowledge queries may be inaccurate, outdated, or limited. Our team continuously strives to enhance the answers' accuracy and reliability by improving and updating the model's training corpus and algorithms. We greatly appreciate user feedback and corrections as they help us refine the model and deliver an improved service.

## License

The code of this project is licensed under Apache 2.0, and the model weights are licensed under GNU AGPL 3.0. If the models contained in this project, or any modified versions thereof, are used in a service which results in misleading or harmful statements causing adverse effects, the responsibility lies with the service provider and is not associated with or attributable to this project.



