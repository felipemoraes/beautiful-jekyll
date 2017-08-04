---
layout: post
published: false
title: Information Flow in Dynamic Information Retrieval
---
Back in 2016, I decided to take an Information Theory course at UFMG lectured by Mário S. Alvim. As part of the course, Mário asks his students to write and present about a specific topic in information theory (not covered by him along the semester) or to model a specific topic in our research area. I tried the latter, however, I chose a topic of Mário expertise, information flow and I wrote a short report on how we could model information flow in information retrieval. 

Months later, Mário and I reviewed the report and together with my Master's supervisor, Rodrygo Santos, we decide to make this modeling available to the IR community. Thus, we got this study accepted as a short paper at ICTIR 2017:

```bibtex
@inproceedings{moraes2017ictir-b,
  author = {Felipe Moraes and Mário S. Alvim and Rodrygo L. T. Santos},
  title = {Modeling Information Flow in Information Retrieval},
  booktitle = {Proceedings of the 3rd ACM International Conference on the 
    Theory of Information Retrieval},
  year = {2017},
  address = {Amsterdam, The Netherlands}
}
```

Nowadays people spend a considerable part of their daily lives interacting with information retrieval systems across multiple devices, from web search engines to personal assistants running on a variety of smart devices. To better support information seeking, modern information retrieval systems must dynamically adapt their retrieval strategy as they interact with the user. In particular, given a user's query, a _dynamic information retrieval_ (DIR) system may respond with an initial result set that best matches its understanding of the user's information need. This set may provide the user with an improved understanding of the information available to the system, prompting him or her to respond back (e.g., by performing a query reformulation, a relevance judgment, or a click). The system may then adapt to the user's response and retrieve a further (ideally improved) result set. This conversational process may continue until the desired information is retrieved to the user or until the user decides to abandon the interaction.


The effectiveness of a DIR system is a function of the gain it provides (in terms of the relevance of the retrieved results) and the effort it incurs (in terms of the total interaction time) to the user. Quantifying such effectiveness is challenging, primarily because the behavior of both the user and the system is inherently uncertain. On the one hand, user actions cannot be fully determined by the system outputs alone, as they also depend on non-observable variables, including the user's cultural background and state of mind. On the other hand, system outputs may not be fully determined by the user actions alone, as the system may benefit from further exploration of the output space to improve its knowledge about the user's need. User modeling under uncertainty has been recently investigated in the context of click models for web search, which are probabilistic graphical models aimed to describe and predict user behavior when interacting with a search engine. In turn, probabilistic retrieval systems have been mostly investigated in the context of the multi-armed bandit problem in reinforcement learning, in which the system faces a trade-off between exploring new knowledge and exploiting existing knowledge.


To provide a unified analysis of the mutual interaction between a user and a DIR system, we propose an information-theoretic model to quantify the amount of information flowing between both agents. Building upon recent advances in information theory, we quantify not only the correlation between user and system behavior, but also how much they influence each other. In particular, a high user-system flow may indicate a highly _sensitive_ system, one that could effectively learn about the user's information need and adapt accordingly. In turn, a high system-user flow may indicate a highly _influential_ system, one that could effectively teach the user about the available information. While system influence may be interpreted as a measure of retrieval effectiveness, system sensitivity could measure lack of privacy. 


In our short paper, we formalize the proposed theoretical model and discuss the challenges involved in instantiating it in a practical scenario as well as implications for evaluating and optimizing DIR systems. 