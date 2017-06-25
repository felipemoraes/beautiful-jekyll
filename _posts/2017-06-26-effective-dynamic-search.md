---
layout: post
title: ' Effectiveness of Dynamic Search Systems'
published: true
---

Research on exploratory search has been supported by several initiatives. The **T**ext **RE**trieval **C**onference (TREC) have hosted related research tracks on [interactive](http://trec.nist.gov/data/interactive.html) search, search within [sessions](http://trec.nist.gov/data/session.html), search for [task completion](http://trec.nist.gov/data/tasks.html) and, more recently, dynamic search in specialized domains organized mainly by [Grace Hui Yang](http://infosense.cs.georgetown.edu/grace/) and [Ian Soboroff](https://www.nist.gov/people/ian-soboroff).  The latter problem, embodied by the [TREC Dynamic Domain (DD)](http://trec-dd.org/) track, was the focus of my Master supervised by [Rodrygo Santos](http://homepages.dcc.ufmg.br/~rodrygo/). As a result of this work, we had a full paper accepted at ICTIR 2017.

```bibtex
@inproceedings{moraes2017ictir-a,
  author = {Felipe Moraes and Rodrygo L. T. Santos and Nivio Ziviani},
  title = {On effective dynamic search in specialized domains},
  booktitle = {Proceedings of the 3rd ACM International Conference on the Theory of Information Retrieval},
  year = {2017},
  address = {Amsterdam, The Netherlands},
  publisher = {ACM},
}
```

The TREC DD problem can be sumarized as follows: 
> Given an initial query, a dynamic search system must improve its understanding of the user’s information need through a series of interactions. In each interaction, the user may provide the system with feedback on the relevance of specific passages of the retrieved documents with respect to one or more aspects underlying his or her information need. The system must then choose to either provide the user with further documents or end the interactive process. An effective system should be able to satisfy as many query aspects as possible (to maximize user satisfaction) with as few interactions as possible (to minimize user effort). 

In the very beggining, we faced this problem as group participant of the TREC DD 2016. In total, we submitted five runs with different approaches, and in our paper report [UFMG at the TREC 2016 Dynamic Domain track](http://trec.nist.gov/pubs/trec25/papers/ufmg-DD.pdf), we presented results for additional unofficial runs.



![ds_framework.png]({{site.baseurl}}/img/ds_framework.png)

## 
