# Creativity in LLM-based Multi-Agent Systems: A Survey
<div align="center">
<a href="https://ieeexplore.ieee.org/document/10531702"><img src="https://img.shields.io/badge/arXiv-2310.14414-b31b1b.svg" alt="arXiv Badge"/></a>
<a href="https://github.com/ge25nab/Awesome-VLMs-in-Autonomous-Driving-and-ITS/blob/main/LICENSE"><img src="https://img.shields.io/github/license/ge25nab/Awesome-VLMs-in-Autonomous-Driving-and-ITS" alt="License Badge"/></a>
</div>

Large language model (LLM)-driven multi-agent systems (MAS) are transforming how humans and AIs collaboratively generate ideas and artifacts. While existing surveys provide comprehensive overviews of MAS infrastructures, they largely overlook the dimension of creativity, including how novel outputs are generated and evaluated, how creativity informs agent personas, and how creative workflows are coordinated.

**This survey offers a structured framework and roadmap for advancing the development, evaluation, and standardization of creative MAS.**
<!--
<p align="center">
<img src="Assets/figure1.png" width="330" height="330"/>
</p>
-->
## :fire: Update

## 🤝  Citation
<!--- Please visit [Creativity in LLM-based Multi-Agent Systems: A Survey) for more details and comprehensive information. If you find our paper and repo helpful, please consider citing it as follows: -->

```BibTeX
@ARTICLE{10531702,
  author={Zhou, Xingcheng and Liu, Mingyu and Yurtsever, Ekim and Zagar, Bare Luka and Zimmer, Walter and Cao, Hu and Knoll, Alois C.},
  journal={IEEE Transactions on Intelligent Vehicles}, 
  title={Vision Language Models in Autonomous Driving: A Survey and Outlook}, 
  year={2024},
  pages={1-20},
  keywords={Autonomous vehicles;Task analysis;Planning;SData models;Surveys;Computational modeling;Visualization;Vision Language Model;Large Language Model;Autonomous Driving;Intelligent Vehicle;Conditional Data Generation;Decision Making;Language-guided Navigation;End-to-End Autonomous Driving},
  doi={10.1109/TIV.2024.3402136}}

```

## :page_with_curl: Introduction
**MAS** comprises multiple autonomous entities: software agents, robots, or human-AI hybrids. This structure enables emergent collaboration and richer exploration of open-ended creative spaces, significantly underlying the practice for computational creativity.
Here, **computational creativity** refers to the creation of artifacts—such as ideas, behaviors, or solutions—that are both novel and valuable, demonstrating clear usefulness or appeal rather than being random.

This survey focuses on systems whose inputs and outputs span text and images. We aim to map the current landscape of techniques, datasets, evaluations, and challenges to foster and measure creativity in such multimodal and heterogeneous systems. By analyzing how different agents interact, we reveal how collaborative structures can unlock creative potentials that exceed what isolated LLMs or individuals can achieve.

<p align="center">
<img src="assets\Creativity MAS.drawio_v6.png"/>
</p>

## 🌟 MAS Workflow and Proactivity

<p>
  <img src="assets\2-2.jpg"/>
</p>

### Overall Proactivity across Process and Decision-Making
| Method                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | Year | Process          |  Decision-Making                 |                                              
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|-----------------------|------------------------------|
| [Rapid AIdeation: Generating Ideas With the Self and in Collaboration With Large Language Models](https://arxiv.org/abs/2403.12928)      | arxiv(2024) | low              | low                     |             
| [AI and the Future of Collaborative Work: Group Ideation with an LLM in a Virtual Canvas](https://dl.acm.org/doi/10.1145/3663384.3663398)  | CHIWork 2024 | low          |  low                |       
| ["It Felt Like Having a Second Mind": Investigating Human-AI Co-creativity in Prewriting with Large Language Models](https://arxiv.org/abs/2307.10811) | arxiv(2024) | low          |  low                    |       
| [StoryDrawer: A Child–AI Collaborative Drawing System to Support Children's Creative Visual Storytelling](https://dl.acm.org/doi/10.1145/3491102.3501914)   | CHI 2022 | low       |    low                  |      
| [CharacterMeet: Supporting Creative Writers' Entire Story Character Construction Processes Through Conversation with LLM-Powered Chatbot Avatars](https://dl.acm.org/doi/10.1145/3613904.3642105)  | CHI 2024 | low      |  low     |            
| [SPARKIT: A Mind Map-Based MAS for Idea Generation Support](https://dl.acm.org/doi/10.1007/978-3-031-71152-7_1)    | EMAS 2024 | medium      |   low    |    
| [Human–machine co-creation: a complementary cognitive approach to creative character design process using GANs](https://link.springer.com/article/10.1007/s11227-024-06083-z)  | The Journal of Supercomputing 2024 | medium        |   low        |     
| [Towards Inclusive Co-creative Child-robot Interaction: Can Social Robots Support Neurodivergent Children's Creativity?](https://dl.acm.org/doi/10.5555/3721488.3721531)       | HRI 2025 | medium       |  low         |    
| [MAxPrototyper: A Multi-Agent Generation System for Interactive User Interface Prototyping](https://arxiv.org/abs/2405.07131)                                                                                                                                                                                                                                                                                                                                                                      | arxiv(2024) | medium  |  low       |  
| [ContextCam: Bridging Context Awareness with Creative Human-AI Image Co-Creation](https://dl.acm.org/doi/10.1145/3613904.3642129#sec-9)                                                                                                                                                                                                                                                                                                                 | 2024 | medium   |    low              |      
| [Scideator: Human-LLM Scientific Idea Generation Grounded in Research-Paper Facet Recombination](https://arxiv.org/abs/2409.14634)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       | arxiv(2025) | medium      |   low                  | 
| [C2Ideas: Supporting Creative Interior Color Design Ideation with a Large Language Model](https://dl.acm.org/doi/abs/10.1145/3613904.3642224)                                                                                                                                                                                                                                                                                                                      | CHI 2024 | medium  | low  |                | 
| [Colin: A Multimodal Human-AI Co-Creation Storytelling System To Support Children's Multi-Level Narrative Skills](https://arxiv.org/abs/2405.06495)   | arxiv(2025) | medium            |     low         |    
| [Creative Wand: A System to Study Effects of Communications in Co-Creative Settings](https://arxiv.org/abs/2310.15065)    | arxiv(2023) | medium   | low  |   
| [AI-Augmented Brainwriting: Investigating the use of LLMs in group ideation](https://dl.acm.org/doi/10.1145/3613904.3642414)   | CHI 2024 | medium   | low  |  
| [ChainBuddy: An AI-assisted Agent System for Generating LLM Pipelines](https://dl.acm.org/doi/10.1145/3706598.3714085)   | CHI 2025 | medium   | low  |  
| [CoQuest: Exploring Research Question Co-Creation with an LLM-based Agent](https://dl.acm.org/doi/pdf/10.1145/3613904.3642698)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/yiren-liu/coquest) |  CHI 2024   | medium   | low  |  
| [An Interactive Co-Pilot for Accelerated Research Ideation](https://aclanthology.org/2024.hcinlp-1.6/)   | HCINLP 2024 | medium   | low  |  
| [A Collaborative, Interactive and Context-Aware Drawing Agent for Co-Creative Design](https://dl.acm.org/doi/10.1109/TVCG.2023.3293853)    | IEEE Transactions on Visualization and Computer Graphics 2023 | medium   | medium  |   
| [Mathemyths: Leveraging Large Language Models to Teach Mathematical Language through Child-AI Co-Creative Storytelling](https://dl.acm.org/doi/10.1145/3613904.3642647)    | CHI 2024 | medium   | medium  |  
| [PersonaFlow: Boosting Research Ideation with LLM-Simulated Expert Personas](https://arxiv.org/pdf/2409.12538)    | arxiv(2024) | high  | low  |  
| [DesignGPT: Multi-Agent Collaboration in Design](https://doi.org/10.1109/ISCID59865.2023.00056) | ISCID 2023 | medium   | medium  | 
| [Towards an AI co-scientist](https://arxiv.org/abs/2502.18864)   | arxiv(2025) | medium   | high  | 
| [LawLuo: A Multi-Agent Collaborative Framework for Multi-Round Chinese Legal Consultation](https://arxiv.org/abs/2407.16252)   | arxiv(2024) | medium   | high  |  
| [StoReys: A neurosymbolic approach to human-AI co-creation of novel action-oriented narratives in known story worlds](https://computationalcreativity.net/iccc24/papers/ICCC24_paper_16.pdf)   | ICCC 2024 | medium   | high  | 
| [AgentReview: Exploring Peer Review Dynamics with LLM Agents](https://aclanthology.org/2024.emnlp-main.70/)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/ahren09/agentreview) | EMNLP 2024 | medium   | high  |  
| [StoryVerse: Towards Co-authoring Dynamic Plot with LLM-based Character Simulation via Narrative Planning](https://dl.acm.org/doi/10.1145/3649921.3656987)    | FDG 2024 | medium   | high  |  
| [PersonaGym: Evaluating Persona Agents and LLMs](https://arxiv.org/pdf/2407.18416)   [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/vsamuel2003/PersonaGym)            [<img src="https://www.svgrepo.com/show/405739/globe-with-meridians.svg" width="30" />](https://personagym.com/)     | arXiv(2025) | high  | medium  | 
| [AgentCoord: Visually Exploring Coordination Strategy for LLM-based Multi-Agent Collaboration](https://arxiv.org/abs/2404.11943)    | arxiv(2024) | high  | medium  |   
| [CollabStory: Multi-LLM Collaborative Story Generation and Authorship Analysis](https://arxiv.org/abs/2406.12665)   | arxiv(2025) | medium   | high  |   
| [MaCTG: Multi-Agent Collaborative Thought Graph for Automatic Programming](https://arxiv.org/abs/2410.19245)  | arxiv(2025) | high   | high  |  
| [Many Heads Are Better Than One: Improved Scientific Idea Generation by A LLM-Based Multi-Agent System](https://arxiv.org/abs/2410.09403)   [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/open-sciencelab/Virtual-Scientists)    | arxiv(2025) | high   | high  |  
| [Generative Agents: Interactive Simulacra of Human Behavior](https://dl.acm.org/doi/10.1145/3586183.3606763)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/joonspk-research/generative_agents)  | UIST 2023 | high   | high  |  
| [HoLLMwood: Unleashing the Creativity of Large Language Models in Screenwriting via Role Playing](https://aclanthology.org/2024.findings-emnlp.474/)  | EMNLP 2024 | high   | high  |  
| [LLM Discussion: Enhancing the Creativity of Large Language Models via Discussion Framework and Role-Play](https://arxiv.org/abs/2405.06373)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/lawraa/LLM-Discussion)  | arxiv(2024) | high   | high  |  
| [Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate](https://aclanthology.org/2024.emnlp-main.992/) [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/Skytliang/Multi-Agents-Debate) | EMNLP 2024 | high   | high  |  
| [Unleashing the Emergent Cognitive Synergy in Large Language Models: A Task-Solving Agent through Multi-Persona Self-Collaboration](https://arxiv.org/abs/2307.05300) [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/MikeWangWZHL/Solo-Performance-Prompting) | arxiv(2024) | high   | high  |  
| [Systematic Idea Refinement for Machine Learning Research Agents](https://openreview.net/forum?id=z0LxrMfFRi)   | Tsinghua University Course:AML 2024 | high   | high  |  
| [Unlocking AI Creativity: A Multi-Agent Approach with CrewAI](https://www.researchgate.net/publication/386306828_Unlocking_AI_Creativity_A_Multi-Agent_Approach_with_CrewAI)  | Journal of Trends in Computer Science and Smart Technology 2024 | high   | high  |  
| [On Generative Agents in Recommendation](https://dl.acm.org/doi/10.1145/3626772.3657844)   | SIGIR 2024 | high   | high  |  
| [MARG: Multi-Agent Review Generation for Scientific Papers](https://arxiv.org/abs/2401.04259)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/allenai/marg-reviewer) | arxiv(2024) | high   | high  |  


## 🌟 MAS Techniques for Creativity

### Divergent Exploration
| Method | Year | Task | Code Link |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----:|:--------------------------------------------------------------|:-------------------------------------------------------------|
| [Human Creativity in the Age of LLMs: Randomized Experiments on Divergent and Convergent Thinking](https://doi.org/10.1145/3706598.3714198) | 2024 | AUT and RAT|  |
| [PersonaGym: A Reinforcement Learning Environment for Training Multi-Persona Agents](https://arxiv.org/abs/2407.18416) | 2024 | Character Design|  |
| [Creativity Support in the Age of Large Language Models](https://arxiv.org/abs/2309.12570) | 2024 | Creative Writing |  |
| [One Does Not Simply “Meme” Alone: Self-Dialogue for Creative Ideation](https://doi.org/10.1145/3708359.3712094) | 2024 | Humor Co-Creation |  |
| [Rapid AIdeation: Generating Ideas With the Self and in Collaboration With LLMs](https://arxiv.org/abs/2403.12928) | 2024 | Idea Generation |  |
| [AI-Augmented Brainwriting: Exploring Idea Flow Between Groups and Large Language Models](https://doi.org/10.1145/3613904.3642414) | 2024 | Idea Generation |  |
| [AI and the Future of Collaborative Work: Group Ideation With an LLM in a Virtual Canvas](https://doi.org/10.1145/3663384.3663398) | 2024 | Idea Generation |  |
| [ContextCam: Bridging Context Awareness With Creative Human-AI Image Co-creation](https://doi.org/10.1145/3613904.3642129) | 2024 | Image Generation |  |
| [C2Ideas: Supporting Creative Interior Color Design Ideation With an LLM](https://dl.acm.org/doi/full/10.1145/3613904.3642224) | 2024 | Interior Color Design Ideation |  |
| [IRIS: An Interactive Co-pilot for Accelerated Research Ideation](https://aclanthology.org/2024.hcinlp-1.6/) | 2023 | Research Ideation |  |
| [PersonaFlow: Dynamic Multi-persona Interaction Framework](https://github.com/Ate329/PersonaFlow) | 2024 | Research Ideation|  |
| [VirSci: Autonomous Team-Leader Agent for Virtual Scientific Collaboration](https://arxiv.org/abs/2409.12538) | 2025 | Scientific Research Co-creation |  |
| [StoryDrawer: Sketch-Based Storyboarding With Multi-agent Discussion](https://arxiv.org/abs/2410.09403) | 2024 | Sketches Generation |  |
| [ICCRI: Inclusive Co-creative Child-Robot Interaction](https://dl.acm.org/doi/10.5555/3721488.3721531) | 2025 | Story Generation |  |
| [Sparkit: Mind-Map-Based Multi-Agent System for Idea Generation Support](https://doi.org/10.1007/978-3-031-71152-7_1) | 2024 | Story Generation |  |

### Iterative Refinement
| Method | Year | Task | Code Link |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----:|:--------------------------------------------------------------|:-------------------------------------------------------------|
| [CharacterMeet: Supporting Creative Writers' Entire Story Character Construction Processes Through Conversation with LLM-Powered Chatbot Avatars](https://doi.org/10.1145/3613904.3642105)                                                    | 2024 | Character Design                      |           |
| [Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate](https://aclanthology.org/2024.emnlp-main.992/)                                                                                                           | 2024 | Debating (Fairness)                  |           |
| [Interpreting and Mitigating Hallucination in MLLMs through Multi-agent Debate](https://arxiv.org/abs/2407.20505)                                                                                                                             | 2024 | Hallucination Mitigation             |           |
| [LawLuo: A Multi-Agent Collaborative Framework for Multi-Round Chinese Legal Consultation](https://arxiv.org/abs/2407.16252)                                                                                                                  | 2024 | Legal Consultation                   |           |
| [ChainBuddy: An AI-assisted Agent System for Generating LLM Pipelines](http://dx.doi.org/10.1145/3706598.3714085)                                                                                                                             | 2025 | LLM Pipeline Generation              |           |
| [DesignGPT: Multi-Agent Collaboration in Design](https://doi.org/10.1109/ISCID59865.2023.00056)                                                                                                                                               | 2023 | Product Design                       |           |
| [Systematic Idea Refinement for Machine Learning Research Agents](https://openreview.net/forum?id=z0LxrMfFRi)                                                                                                                                | 2024 | Scientific Research Co-creation      |           |
| [HoLLMwood: Unleashing the Creativity of Large Language Models in Screenwriting via Role Playing](https://aclanthology.org/2024.findings-emnlp.474.pdf)                                                                                      | 2024 | Screenwriting                        |           |
| [A Collaborative, Interactive and Context-Aware Drawing Agent for Co-Creative Design](https://dl.acm.org/doi/10.1109/TVCG.2023.3293853)                                                                                                       | 2024 | Sketches Generation                  |           |
| [Generative Agents: Interactive Simulacra of Human Behavior](https://doi.org/10.1145/3586183.3606763)                                                                                                                                         | 2023 | Social Simulation                    |           |



### Collaborative Synthesis

| Method | Year | Task | Code Link |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|:----:|:--------------------------------------------------------------|:-------------------------------------------------------------|
| [TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks](https://arxiv.org/abs/2412.14161)                                                                                                                 | 2024 | Agent Benchmarking                          |                                                        |
| [AgentCoord: Visually Exploring Coordination Strategy for LLM-based Multi-Agent Collaboration](https://arxiv.org/abs/2404.11943)                                                                                               | 2024 | Agent Collaboration Visualization           |                                                        |
| [Unleashing the Emergent Cognitive Synergy in Large Language Models: A Task-Solving Agent through Multi-Persona Self-Collaboration](https://arxiv.org/abs/2307.05300)                                                         | 2024 | Cognitive Synergy                           |                                                        |
| ["It Felt Like Having a Second Mind": Investigating Human-AI Co-creativity in Prewriting with Large Language Models](https://dl.acm.org/doi/10.1145/3637361)                                                                  | 2024 | Creative Writing                            |                                                        |
| [Creative Agents: Simulating the Systems Model of Creativity with Generative Agents](https://arxiv.org/abs/2411.17065)                                                                                                         | 2024 | Creativity Simulation                       |                                                        |
| [ProofNet: Autoformalizing and Formally Proving Undergraduate-Level Mathematics](https://arxiv.org/abs/2302.12433)                                                                                                             | 2023 | Formal Proof                                |                                                        |
| [Beyond Code Generation: LLM-supported Exploration of the Program Design Space](http://dx.doi.org/10.1145/3706598.3714154)                                                                                                     | 2025 | Program Design                              |                                                        |
| [Agent4Rec: On Generative Agents in Recommendation](https://doi.org/10.1145/3626772.3657844)                                                                                                                                   | 2024 | Recommendation                              |                                                        |
| [How AI Processing Delays Foster Creativity: Exploring Research Question Co-Creation with an LLM-based Agent](https://dl.acm.org/doi/10.1145/3613904.3642698)                                                                  | 2024 | Research Ideation                           |                                                        |
| [MARG: Multi-Agent Review Generation for Scientific Papers](https://arxiv.org/abs/2401.04259)                                                                                                                                  | 2024 | Research Peer Review                        |                                                        |
| [AgentReview: Exploring Peer Review Dynamics with LLM Agents](https://aclanthology.org/2024.emnlp-main.70/)                                                                                                                    | 2024 | Scientific Peer Review                      |                                                        |
| [Unlocking AI Creativity: A Multi-Agent Approach with CrewAI](https://irojournals.com/tcsst/article/pdf/6/4/2)                                                                                                                  | 2024 | Scientific Research Co-creation             |                                                        |
| [Towards an AI co-scientist](https://arxiv.org/abs/2502.18864)                                                                                                                                                                 | 2025 | Scientific Research Co-creation             |                                                        |
| [Human--machine co-creation: a complementary cognitive approach to creative character design process using GANs](https://link.springer.com/article/10.1007/s11227-024-06083-z)                                                | 2024 | Silhouette Generation                       |                                                        |
| [ChatDev: Communicative Agents for Software Development](https://aclanthology.org/2024.acl-long.810/)                                                                                                                          | 2024 | Software Engineering                        |                                                        |
| [MaCTG: Multi-Agent Collaborative Thought Graph for Automatic Programming](https://arxiv.org/abs/2410.19245)                                                                                                                   | 2025 | Software Engineering                        |                                                        |
| [CollabStory: Multi-LLM Collaborative Story Generation and Authorship Analysis](https://arxiv.org/abs/2406.12665)                                                                                                              | 2024 | Story Generation                            |                                                        |
| [Colin: A Multimodal Human-AI Co-Creation Storytelling System To Support Children's Multi-Level Narrative Skills](https://arxiv.org/abs/2405.06495)                                                                           | 2024 | Story Generation                            |                                                        |
| [Mathemyths: Leveraging Large Language Models to Teach Mathematical Language through Child-AI Co-Creative Storytelling](https://doi.org/10.1145/3613904.3642647)                                                              | 2024 | Story Generation                            |                                                        |
| [StoReys: A neurosymbolic approach to human-AI co-creation of novel action-oriented narratives in known story worlds](https://computationalcreativity.net/iccc24/papers/ICCC24_paper_16.pdf)                                   | 2024 | Story Generation                            |                                                        |
| [StoryVerse: Towards Co-authoring Dynamic Plot with LLM-based Character Simulation via Narrative Planning](https://doi.org/10.1145/3649921.3656987)                                                                           | 2024 | Story Generation                            |                                                        |
| [MAxPrototyper: A Multi-Agent Generation System for Interactive User Interface Prototyping](https://arxiv.org/abs/2405.07131)                                                                                                  | 2024 | UI Prototyping   


## 🌟 Persona and Agent Profile
### Coarse-Grained
| Method                                                                                                                                                                                   | Publication        | Profiling Method                                   | Agent Persona                                                             |                                               
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------|------------------------------------------------------------------| 
| [Unleashing the Emergent Cognitive Synergy in Large Language Models: A Task-Solving Agent through Multi-Persona Self-Collaboration](https://arxiv.org/abs/2307.05300)                         [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/MikeWangWZHL/Solo-Performance-Prompting)                     | arXiv(2024) | Model-Generated           |Self-Defined      |
| [LLM Discussion: Enhancing the Creativity of Large Language Models via Discussion Framework and Role-Play](https://arxiv.org/abs/2405.06373)      [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/lawraa/LLM-Discussion)                   | COLM 2024 | Model-Generated            | Self-Defined         |
| [PersonaGym: Evaluating Persona Agents and LLMs](https://arxiv.org/abs/2407.18416)   [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/vsamuel2003/PersonaGym)            [<img src="https://www.svgrepo.com/show/405739/globe-with-meridians.svg" width="30" />](https://personagym.com/)            | arXiv(2025) | Human-defined          | Self-Defined         |
| [Systematic Idea Refinement for Machine Learning Research Agents](https://openreview.net/forum?id=z0LxrMfFRi)                                                                                       | Tsinghua University Course:AML 2024 | Human-Defined | Assitant         |
| [Sparkit: A mind map-based mas for idea generation support.](https://link.springer.com/chapter/10.1007/978-3-031-71152-7_1)                                                                            | EMAS 2024 | Human-Defined            |  Self-Defined            |
| [Encouraging Divergent Thinking in Large Language Models through Multi-Agent Debate](https://aclanthology.org/2024.emnlp-main.992/)     [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/Skytliang/Multi-Agents-Debate)                                       | EMNLP 2024 | Human-Defined           | Debater       |
| [An Interactive Co-Pilot for Accelerated Research Ideation](https://aclanthology.org/2024.hcinlp-1.6)                                                                                                                 | HCINLP 2024 | Human-Defined    | Mentor & Colleague   |
| [ChainBuddy: An AI-assisted Agent System for Generating LLM Pipelines](https://dl.acm.org/doi/10.1145/3706598.3714085)                                                                                     | CHI 2025 | Human-Defined  | Mentor & Planner   |


### Medium-Coarse-Grained
| Method                                                                                                                                                                                   | Publication        | Profiling Method                                   | Agent Persona                                                             |                                               
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------|------------------------------------------------------------------| 
| [TheAgentCompany: Benchmarking LLM Agents on Consequential Real World Tasks](https://arxiv.org/abs/2412.14161)       [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/TheAgentCompany/TheAgentCompany)            [<img src="https://www.svgrepo.com/show/405739/globe-with-meridians.svg" width="30" />](https://the-agent-company.com/)                                                                                      |  arXiv(2025) | Model-Generated            | Company Employee |
| [HOLLMWOOD: Unleashing the Creativity of Large Language Models in Screenwriting via Role Playin](https://aclanthology.org/2024.findings-emnlp.474)                                                                                                                                     | EMNLP 2024 | Human-Defined         | Artist  |
| [TRIZ Agents: A Multi-Agent LLM Approach for TRIZ-Based Innovation](https://repo.pw.edu.pl/info/article/WUT0cd2725a4fd94bea8e54cedcae00132f/)                                                                                                                 | ICAART 2025 |       Human-Defined   | Problem Solver      |
| [Towards an AI co-scientist](https://arxiv.org/abs/2502.18864)   | arxiv(2025) | Human-Defined  | Researcher         |
| [MaCTG: Multi-Agent Collaborative Thought Graph for Automatic Programming](https://arxiv.org/abs/2410.19245)  | arxiv(2025) |    Human-Defined | Programmer    |
| [DesignGPT: Multi-Agent Collaboration in Design](https://doi.org/10.1109/ISCID59865.2023.00056) | ISCID 2023 | Human-Defined  |  Self-Defined    |
| [CoQuest: Exploring Research Question Co-Creation with an LLM-based Agent](https://dl.acm.org/doi/10.1145/3613904.3642698)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/yiren-liu/coquest) |  CHI 2024  | Human-Defined  | Researcher        |
| [LawLuo: A Multi-Agent Collaborative Framework for Multi-Round Chinese Legal Consultation](https://arxiv.org/abs/2407.16252)   | arxiv(2024)| Human-Defined |  Lawyer |
| [MARG: Multi-Agent Review Generation for Scientific Papers](https://arxiv.org/abs/2401.04259)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/allenai/marg-reviewer) | arxiv(2024) | Human-Defined | Expert| 


### Fine-Grained
| Method                                                                                                                                                                                   | Publication        | Profiling Method                                   | Agent Persona                                                             |                                               
|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------|------------------------------------------------------------------| 
| [PersonaFlow: Boosting Research Ideation with LLM-Simulated Expert Personas](https://arxiv.org/pdf/2409.12538)    | arxiv(2024) | Data-Derived | Researcher |
| [Many Heads Are Better Than One: Improved Scientific Idea Generation by A LLM-Based Multi-Agent System](https://arxiv.org/abs/2410.09403)   [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/open-sciencelab/Virtual-Scientists)   | arxiv(2025) |  Data-Derived   |  Researcher       |
| [On Generative Agents in Recommendation](https://doi.org/10.1145/3626772.3657844)                 | SIGIR 2024 | Data-Derived  |  Media User |
| [[PersonaLLM: Investigating the Ability of Large Language Models to Express Personality Traits]](https://aclanthology.org/2024.findings-naacl.229/)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/hjian42/PersonaLLM)   |   NAACL 2024  |  Model-Generated | 
  Self-Defined         |
| [The Power of Personality: A Human Simulation Perspective to Investigate Large Language Model Agents](https://arxiv.org/abs/2502.20859)                                                                            | arXiv(2025) | Model-Generated |   Self-Defined    |
| [Creative Agents: Simulating the Systems Model of Creativity with Generative Agents](https://arxiv.org/abs/2411.17065) | arXiv(2024) | Model-Generated |   Artist        |
| [Synergizing Human-AI Agency: A Guide of 23 Heuristics for Service Co-Creation with LLM-Based Agents](https://arxiv.org/abs/2310.15065)                                                                                                                 | arXiv(2023) | Model-Generated |     Self-Defined        |

| [Generative Agents: Interactive Simulacra of Human Behavior](https://dl.acm.org/doi/10.1145/3586183.3606763)   [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/joonspk-research/generative_agents)  | UIST 2023   | Conditional Video Generation            |    Human-defined | Sandbox Character     |
|[AgentReview: Exploring Peer Review Dynamics with LLM Agents](https://aclanthology.org/2024.emnlp-main.70/)  [![GitHub](https://img.shields.io/badge/GitHub-Visit-black?logo=github)](https://github.com/ahren09/agentreview) | EMNLP 2024| Human-defined  |  Reviewer   |

## 🌟 Evaluation

### Text Artifact Evaluation
| Papers | Year | Task | Subjective | Objective | Code Link |                                               
|:-------|------|------|------------|-----------|-----------| 
| [Human Creativity in the Age of LLMs: Randomized Experiments on Divergent and Convergent Thinking](https://dl.acm.org/doi/pdf/10.1145/3706598.3714198) | 2025 | AUT and RAT | TTCT, Boden’s Criterion, and others | Semantic similarity |  |
| [The Power of Personality: A Human Simulation Perspective to Investigate Large Language Model Agents](https://arxiv.org/pdf/2502.20859)  | 2025 | AUT and others | TTCT | - |  |
| [LLMDiscussion: Enhancing the Creativity of Large Language Models via Discussion Framework and Role-Play](https://arxiv.org/pdf/2405.06373) | 2024 | AUT and others | TTCT  | - | [Github](https://github.com/lawraa/LLM-Discussion) |
| [ An Innovative Solution to Design Problems: Applying the Chain-of-Thought Technique to Integrate LLM-Based Agents With Concept Generation Methods](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10747324)  | 2025 | Conceptual Design | TTCT | - |  |
| [Rapid AIdeation: Generating Ideas With the Self and in Collaboration With Large Language Models](https://arxiv.org/pdf/2403.12928) | 2024 | Idea Generation | TTCT | - |  |
| [AI-Augmented Brainwriting: Investigating the use of LLMs in group ideation](https://dl.acm.org/doi/pdf/10.1145/3613904.3642414) | 2024 | Idea Generation | Innovation, Insightfullness, and others | Semantic Similarity |  |
| [LawLuo: A Multi-Agent Collaborative Framework for Multi-Round Chinese Legal Consultation](https://arxiv.org/pdf/2407.16252) | 2024 | Legal Consultation  | Personalization and Professionalism | - | |
| [ProofNet: Autoformalizing and Formally Proving Undergraduate-Level Mathematics](https://arxiv.org/pdf/2302.12433) | 2023 | Mathematical Proving  | - | BLEU Score | [Github](https://github.com/zhangir-azerbayev/proofnet)  |
| [DesignGPT: Multi-Agent Collaboration in Design](https://ieeexplore.ieee.org/document/10494260) | 2023 | Product Design  | Novelty, Completeness, and Feasibility | - |  |
| [Using Generative AI Personas Increases Collective Diversity in Human Ideation](https://arxiv.org/pdf/2504.13868) | 2025 | Plot Generation  | - | Semantic Similarity |  |
| [Creativity Support in the Age of Large Language Models: An Empirical Study Involving Emerging Writers](https://arxiv.org/pdf/2309.12570) | 2024 | Poem Writing | Fluency and Creativity | - |  |
| [MARG: Multi-Agent Review Generation for Scientific Papers](https://arxiv.org/pdf/2401.04259) | 2024 | Paper Review Generation  | Specificity and Overall Rating | - | [Github](https://github.com/allenai/marg-reviewer)  |
| [CoQuest: Exploring Research Question Co-Creation with an LLM-based Agent](https://dl.acm.org/doi/pdf/10.1145/3613904.3642698) | 2024 | Research Ideation | Boden’s criterion | - | [Github](https://github.com/yiren-liu/coquest)  |
| [PersonaFlow: Boosting Research Ideation with LLM-Simulated Expert Personas](https://arxiv.org/pdf/2409.12538) | 2024 | Research Ideation | Creativity, Usefulness, and Helpfulness | - |  |
| [HOLLMWOOD:Unleashing the Creativity of Large Language Models in Screenwriting via Role Playing](https://aclanthology.org/2024.findings-emnlp.474.pdf) | 2024 | Screenwriting | Interestingness, Relevance, and others | Entropy-n, Self-BLEU, and others | [Github](https://github.com/litmirror123/HoLLMwood)  |
| [Towards an AI co-scientist](https://arxiv.org/pdf/2502.18864) | 2025 | Scientific Research Co-creation | Novelty and Impact | - | [Github](https://github.com/ai-in-pm/AI-Co-Scientist)  |
| [Mixed-Initiative Methods for Co-Creation in Scientific Research](https://dl.acm.org/doi/10.1145/3635636.3664627) | 2024 | Scientific Research Co-creation | Novelty, Specificity, and others | Semantic Similarity |   |
| [Many Heads Are Better Than One: Improved Scientific Idea Generation by A LLM-Based Multi-Agent System](https://arxiv.org/pdf/2410.09403) | 2025 | Scientific Research Co-creation | Novelty, Clarity, Feasibility | Semantic Euclidean Distance | [Github](https://github.com/RenqiChen/Virtual-Scientists)  |
| [Mathemyths: Leveraging Large Language Models to Teach Mathematical Language through Child-AI Co-Creative Storytelling](https://dl.acm.org/doi/10.1145/3613904.3642647) | 2024 | Story Generation | Readability, Perceived Creativity, and others | - | [Github](https://github.com/zhangchaodesign/mathemyths)  |
| [StoReys: A neurosymbolic approach to human-AI co-creation of novel action-oriented narratives in known story worlds](https://computationalcreativity.net/iccc24/papers/ICCC24_paper_16.pdf) | 2024 | Story Generation | Interactivity, Coherence, and others | Self-BLEU |  |
| [Creative Wand: A System to Study Effects of Communications in Co-creative Settings](https://dl.acm.org/doi/pdf/10.1609/aiide.v18i1.21946) | 2022 | Story Generation  | Goal completion and Satisfication | - | [Github](https://github.com/eilab-gt/CreativeWand)  |
| [CollabStory: Multi-LLM Collaborative Story Generation and Authorship Analysis](https://arxiv.org/pdf/2406.12665) | 2024 | Story Generation  | Creativity | Entropy and others | [Github](https://github.com/saranya-venkatraman/CollabStory)  |
| [Towards Inclusive Co-creative Child-robot Interaction: Can Social Robots Support Neurodivergent Children's Creativity?](https://dl.acm.org/doi/10.5555/3721488.3721531) | 2025 | Story Generation  | TTCT | - |  |


### Image Artifact Evaluation
| Papers | Year | Task | Subjective | Objective | Code Link |                                               
|:-------|------|------|------------|-----------|-----------| 
| [C2Ideas: Supporting Creative Interior Color Design Ideation with a Large Language Model](https://dl.acm.org/doi/full/10.1145/3613904.3642224) | 2024 | Interior Color Design Ideation | Inspiring, Reasonableness, and others | - |  |
| [CREA:ACollaborative Multi-Agent Framework for Creative Content Generation with Diffusion Models](https://arxiv.org/pdf/2504.05306) | 2025 | Image Editing & Generation  | Expressiveness, Aesthetic appeal, and others | CLIP scores and others |  |
| [One Does Not Simply Meme Alone: Evaluating Co-Creativity Between LLMs and Humans in the Generation of Humor](https://dl.acm.org/doi/10.1145/3708359.3712094) | 2025 | Meme Generation | Funniness, Creativity, and Shareability | - |  |
| [StoryDrawer: A Child–AI Collaborative Drawing System to Support Children's Creative Visual Storytelling](https://dl.acm.org/doi/10.1145/3491102.3501914) | 2022 | Sketches Generation | TTCT | FID, TIE ,and Semantic loss |  |
| [A Collaborative, Interactive and Context-Aware Drawing Agent for Co-Creative Design](https://dl.acm.org/doi/10.1109/TVCG.2023.3293853) | 2024 | Sketches Generation | TTCT | - | [Github](https://github.com/fibarrola/reframer_dockerized)  |
| [Drawing with Reframer: Emergence and Control in Co-Creative AI](https://dl.acm.org/doi/10.1145/3581641.3584095) | 2023 | Sketches Generation | Novelty and Surprise within MICSI | - | [Github](https://github.com/fibarrola/reframer_dockerized)  |
| [Human–machine co-creation: a complementary cognitive approach to creative character design process using GANs](https://link.springer.com/article/10.1007/s11227-024-06083-z) | 2024 | Silhouette Generation | Designer’s review | FID |  |
| [MAxPrototyper: A Multi-Agent Generation System for Interactive User Interface Prototyping](https://arxiv.org/pdf/2405.07131) | 2024 | UI Prototype Generation  | - | FID and Generation Diversity|  |

### Interaction Evaluation with User Study
| Papers | Year | Task | Code Link |                                               
|:-------|------|------|-----------| 
| [ContextCam: Bridging Context Awareness with Creative Human-AI Image Co-Creation](https://dl.acm.org/doi/10.1145/3613904.3642129) | 2024 | Image Generation |   |
| [AI and the Future of Collaborative Work: Group Ideation with an LLM in a Virtual Canvas](https://dl.acm.org/doi/10.1145/3663384.3663398) | 2024 | Idea Generation |  |
| [How AI Processing Delays Foster Creativity: Exploring Research Question Co-Creation with an LLM-based Agent](https://dl.acm.org/doi/10.1145/3613904.3642698) | 2024 | Research Ideation |   |
| ["It Felt Like Having a Second Mind": Investigating Human-AI Co-creativity in Prewriting with Large Language Models](https://dl.acm.org/doi/10.1145/3637361) | 2024 | Creative Writing |   |


## 🌟 Dataset

### Psychological Test Datasets
| Dataset                                                                                                                                                                                                                                                                                           | Year | Task                       | Data Link                                             |                                               
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|----------------------------|-------------------------------------------------------| 

### Task Specific Datasets
| Paper | Task | Year | Data Link |                                              
|------|------------|-----------|-----------|
|[MacGyver: Are Large Language Models Creative Problem Solvers?](https://aclanthology.org/2024.naacl-long.297.pdf)| Problem-Solving in Physically Grounded Scenarios |2023| [Link](https://github.com/allenai/MacGyver)   |
|[Creativity Support in the Age of Large Language Models: An Empirical Study Involving Emerging Writers](https://arxiv.org/pdf/2309.12570)| Creative Writing |2023| [Link](https://collab-stories.github.io/)   |
|[Large Language Models for Human-AI Co-Creation of Robotic Dance Performances](https://arxiv.org/pdf/2309.12570)| Robot Dance Creation |2024| [Link](https://github.com/alleDe/LLMsChoreography) |
|[Human–machine co-creation: a complementary cognitive approach to creative character design process using GANs](https://link.springer.com/article/10.1007/s11227-024-06083-z)| Character Design  |2024| [Link](https://data.mendeley.com/datasets/sdwbf4xrwz/3) |
|[TriviaQA](https://aclanthology.org/P17-1147/)| Open-ended question task.   |2017| [Link](https://github.com/mandarjoshi90/triviaqa) |
|[Generative Agents: Interactive Simulacra of Human Behavior](https://dl.acm.org/doi/10.1145/3586183.3606763)| Open-ended question task.   |2023| [Link](https://github.com/joonspk-research/generative_agents) |
|[GPQA: A Graduate-Level Google-Proof Q&A Benchmark](https://arxiv.org/abs/2311.12022)| Open-ended question task   |2023| [Link](https://github.com/idavidrein/gpqa) |
|[Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models](https://arxiv.org/abs/2206.04615)| Codenames Task   |2022| [Link](https://github.com/google/BIG-bench) |
|[ProofNet: Autoformalizing and Formally Proving Undergraduate-Level Mathematics](https://arxiv.org/abs/2302.12433)| Mathematical Formal Proof Generation and Verification   |2023| [Link](https://github.com/zhangir-azerbayev/ProofNet) |
|[AI Idea Bench 2025: AI Research Idea Generation Benchmark](https://arxiv.org/abs/2504.14191)| Idea Generation   |2025| [Link](https://huggingface.co/datasets/yanshengqiu/AI_Idea_Bench_2025) |
|[LiveIdeaBench: Evaluating LLMs' Divergent Thinking for Scientific Idea Generation with Minimal Context](https://arxiv.org/abs/2412.17596)| Idea Generation   |2024| [Link](https://github.com/x66ccff/liveideabench) |
|COMPAS dataset| Fairness-Aware Debating   |2016| [Link](https://github.com/propublica/compas-analysis) |
## License

This repository is released under the [Apache 2.0 license](https://github.com/ge25nab/Awesome-VLMs-in-Autonomous-Driving-and-ITS/blob/main/LICENSE).
