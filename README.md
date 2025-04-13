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
# 🚀 MCoT reasoning
## A Chain of Thought (CoT) is a method of having a model generate a series of intermediate reasoning steps to gradually arrive at a final answer. On this basis, multi-channel thinking chain reasoning considers a variety of information input channels (such as text, images, speech, etc.), and uses the information of different channels to carry out a more comprehensive reasoning process.In page5 of this Survey, there is already a clear classification framework and literature citations[[Paper]](https://arxiv.org/abs/2503.12605)
# 🤖Application of Embodied-AI
## EmbodiedGPT [39]; E-CoT [[41]](https://arxiv.org/pdf/2407.08693); ManipLLM [[139]](http://openaccess.thecvf.com/content/CVPR2024/html/Li_ManipLLM_Embodied_Multimodal_Large_Language_Model_for_Object-Centric_Robotic_Manipulation_CVPR_2024_paper.html); CoTDiffusion [[136]](http://openaccess.thecvf.com/content/CVPR2024/html/Ni_Generate_Subgoal_Images_before_Act_Unlocking_the_Chain-of-Thought_Reasoning_in_CVPR_2024_paper.html);Emma-X [[140]](https://arxiv.org/abs/2412.11974); SpatialCoT [[141]](https://arxiv.org/abs/2501.10074); MCoCoNav [[142]](https://arxiv.org/abs/2412.18292); MCoT-Memory [[133]](https://openreview.net/forum?id=Z1Va3Ue4GF)
## Due to the works above all,we have an classification
### 🐳Based on CoT:This part is mainly the use of LLMs for multi-step reasoning, clear the middle decision-making process, like human problem-solving, step by step think clearly and then start.The work is E-CoT,EMMA-X
### 🐍Goal-driven：The teacher becomes a sub-target, and then deduces and performs actions according to the target，Visualize a few key images of the future and execute accordingly.The work is CoTDiffusion
### 🎈Operation action prediction：Deduce actions or positions directly from visual language, identify the operating point at a glance, and directly tell the robot, where to grab, where to grab。The work is ManipLLM
### 🧠Memory enhancement reasoning：Introduce task memory, selectively store reasoning process, learn to "duplicate disk" and "experience reuse", and do better.The work is MCoT-Memory
### 👁️Multi-cooperative reasoning：With multiple agents sharing information, collaborative reasoning, a group of robots "think separately and cooperate with each other" to complete complex navigation or collaborative tasks.The work is MCoCoNav
## 🌎Contribution：
### Major contribution: There is a common trend in these articles that the reasoning mode of large models is CoT paradigm and the reasoning is output in text and other ways, and the interpretability is enhanced. From the previous end to end (input a thing output no intermediate process, the middle is a black box, do not know the reasoning process) but now there is text output in the middle, and then the text as a guide to guide the next action. (Stepwise language), and put forward the construction of the mechanism of multi-modal joint reasoning. It also puts forward scene memory, puts high quality CoT into memory bank, retrieves past similar experience when doing new task, and makes transfer reuse of inference. And when dealing with long-term tasks, reasoning can also assist in the formation of subitems and decompose multiple intermediate states. The CoT Diffusion model generates intermediate image processing tasks, and finally combines swarm artificial intelligence to think and reason independently and learn the actions of others, getting closer and closer to the way humans think

  
