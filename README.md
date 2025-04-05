# AI-Reasoning
  ## AI reasoning refers to the ability of artificial intelligence systems to make logical deductions, infer conclusions, and solve problems based on available data. It involves processes like decision-making, pattern recognition, and applying rules to understand and interpret complex information, aiming to mimic human cognitive reasoning abilities
# 🚀Classification by survey
  ## This survey on multimodal large model inference, mainly from 1) inference capability, evaluation protocol 3) multimodal instruction tuning 4) inference-intensive tasks 5) benchmarking results 6) development of these aspects [[Paper]](https://arxiv.org/pdf/2401.06805)
# 🧠1.Datasets and benchmarks
## which is placed on pure language and multimodal inference data sets, such as reasoning mathematical problems, common sense reasoning, and symbolic reasoning [65,66,67,68]. Multimodality includes data sets for image content and letter understanding, visual question answering, etc. [71,72,73].
# 🧠2.Increase the reasoning ability of LLM
##   1) [corpos](https://arxiv.org/abs/2403.18120) 
##   2)[instruction tuning](https://arxiv.org/abs/1906.02361)
###        MiniGPT has different task-specific instruction modules,[and mpLVG-owl2](https://arxiv.org/abs/2304.14178) use the model collaboration,[[126]](https://arxiv.org/abs/2306.05425)improve the OpenFlamingo,instruction compliance,effective use of context.[CogVLM](https://proceedings.neurips.cc/paper_files/paper/2024/hash/dc06d4d2792265fb5454a6092bfd5c6a-Abstract-Conference.html),additional vision specialists have been brought in.
##   3)[context learning](https://arxiv.org/abs/2205.10625)
### [[lmg2LLM]](https://openaccess.thecvf.com/content/CVPR2023/html/Guo_From_Images_to_Textual_Prompts_Zero-Shot_Visual_Question_Answering_With_CVPR_2023_paper.html)Automatically generate prompts with LLM unknowable examples and formulate questions corresponding to answers
##   4)[prompt engineering](https://proceedings.neurips.cc/paper_files/paper/2022/hash/9d5609613524ecf4f15af0f7b31abca4-Abstract-Conference.html?ref=https://githubhelp.com)
##   5)Variant of CoT[[104]](https://proceedings.neurips.cc/paper_files/paper/2022/hash/9d5609613524ecf4f15af0f7b31abca4-Abstract-Conference.html?ref=https://githubhelp.com) [[107]](https://arxiv.org/abs/2210.00720) [[108]](https://www.chatgpthero.io/wp-content/uploads/2023/12/2210.03493.pdf)
##   6)Interacting with the outside world(using tool)[[109]](https://proceedings.mlr.press/v202/gao23f)[[110]](https://arxiv.org/abs/2211.12588)[[111]](https://par.nsf.gov/biblio/10451467)
# ‼️3.Embodied-AI Reasoning
##    Embodied agents have a powerful reasoning ability to perceive and make decisions,some initial studies focused less on additional traning of models.The reasoning of embodied agency is divided into four categories 1)Individual component reasoning 2)MW reasoning 3) Feedback reasoning 4)Policy generation reasoning 5)Robot data reasoning
## 1.Individual component reasoning
### [CLIPort](https://proceedings.mlr.press/v164/shridhar22a.html),CLIP helps with broad semantic understanding,other works like [SMS](https://arxiv.org/abs/2204.00598),[LM-NAV](https://proceedings.mlr.press/v205/shah23b)use language as bridge decomposition instruction.[[173]](https://arxiv.org/abs/2302.00763)
## 2.MW reasoning
### [[174]](https://ieeexplore.ieee.org/abstract/document/10610634/)To perform a task involving a distant past or fact, knowledge is represented by a world state, but the downside is that specific task cues are required and world model state updates can be inaccurate.
## 3.Feedback reasoning
### [[175]](https://arxiv.org/abs/2207.05608)Good methods try to mimic human thought processes with natural language.
## 4.Policy generation reasoning
### [[176]](https://ieeexplore.ieee.org/abstract/document/10160591/)LLM generates policy code and expands the scope of inference tasks, but the disadvantage is that the API and control primitives are limited, and there is no feasible mechanism to evaluate a given instruction
## 5.Robot data reasoning
### [[177]](https://arxiv.org/abs/2211.11736) [[178]](https://arxiv.org/abs/2301.12507)VLM embeddings embody agent, integration of discrete text markup.PaLM-E,inputs from different schemas can be converted into LLM-compatible formats, enabling embodied agents to interact across schemas


  
