---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}
I conduct research in three streams. The first stream centers around understanding the dynamic evolution of online open collaborations. I apply advanced research methods such as time-series clustering and simultaneous equations to study temporal patterns and recursive relationships between articles and editors in the development of Wikipedia articles. The second stream focuses on developing a computational theory of online open collaboration using agent-based modeling. The model is grounded in a comprehensive review of Wikipedia collaboration research and will be used to simulate editing dynamics and examine the impact of anti-vandalism tools in Wikipedia collaboration. The third stream is my Ph.D. dissertation research, which involved modeling and predicting technology diffusion through a novel machine learning approach and algorithmically optimizing related marketing strategies in the solar panel industry.

## Stream 1: Unpacking the Dynamic Evolution of Wikipedia Collaboration
Online open collaboration systems like Wikipedia are complex socio-technical systems, where editors and artifacts interact and coevolve. In order to fully understanding the processes and mechanisms behind the successes and failures of Wikipedia collaboration, we need to go beyond static, cross-sectional studies and examine dynamic, recursive relationships.  

**Mining and predicting dynamic evolution of Wikipedia articles**
 
This work examines the dynamic change in the quality of Wikipedia articles to answer two research questions: 1) What are the common trajectories through which article quality grows over time and 2) What factors determine an article's trajectory? We downloaded archival data of 6,057 Wikipedia articles in the domains of roads, films, and battles. We then utilized an advanced time-series clustering method called Dynamic Time Warping to identify common patterns in the quality trajectories and ran multinomial logistic regression to predict articles' trajectories. Our results show three distinctive clusters of quality growth, which we named as stalled, plateaued, and sustained growth. The regression results suggest that the path an article follows is determined by both inherent attributes of the article, such as topic importance, and attributes of contribution and coordination among editors of the article. Our results also show different factors matter at different stages of article development.   

**Recursive relationships between Wikipedia article quality and editor crowds**

Prior studies have often examined the impact of editors on article quality or vice versa. In this paper, we argue that the recursive relationship between the two, i.e., between article quality and the number of active editors, needs to be accounted for, in order to fully understand the dynamics and co-evolution between the two. We sampled 2,466 Wikipedia articles that were Good Article nominees and extracted monthly observations of quality and editor activities. We run simultaneous equations to model the reciprocal effects between quality and editors and included instrumental variables to address endogeneity. This study has three takeaways: 1) consistent with prior literature, high article quality attracted more active editors; 2) additional factors such as nomination events and search interests also attracted more editors to contribute to articles; 3) contrary to prior beliefs, being affiliated with WikiProjects reduced, instead of increased, the number of editors, and  increases in the number of editors decreased, rather than increased, article quality. 

## Stream 2: Developing a Computational Theory of Online Open Collaboration
In a complex socio-technical system like Wikipedia, editor behaviors are influenced by many factors such as article artifacts, other editors, tools, and governing policies. The design and management of such systems are often challenging, with small changes made to parts of the system can interact with other factors and cause unintended consequences. In this project, our goal is to develop a computational theory of online collaboration by integrating various theories and empirical findings into an agent-based model. 

**A comprehensive review of Wikipedia collaboration research**

To ground our model, we first conducted a comprehensive review of empirical research on how Wikipedia editors collaborate to create the articles. Although several reviews of Wikipedia research exist, most are summaries of individual papers with little integration to show the big picture of what has been learned across studies. We searched and found approximately 1600 papers from the ACM digital library in March 2017. We chose 244 articles to review, which examine various aspects and processes of how Wikipedia editors collaborate with one another. Some popular themes include article quality (28 articles), conflict (14 articles), and tools (13 articles). Preliminary analyses show several common themes around quality such as the definition and measurements of article definition, antecedents of quality, and methods of article quality prediction. Research on conflict center around the sources and consequences of conflict, conflict management, and detection. 

**Agent-based modeling to study the impact of Wikipedia vandal-fighting tools**

Wikipedia has experienced a slow but steady decline in editor contribution since 2007. One speculated the reason for the decline is the unfriendly environment for newcomers who are more likely to be reverted, particularly due to the use of semi-automated tools to fight vandalism. While the impact of these semi-automated tools remains an open question, their design requires careful consideration of some critical trade-offs. For example, how should the task of vandal fighting be divided between human editors and tools? What criteria should be built into vandal detection algorithms to balance between type I and type II errors? How should the algorithms be customized to learn and adapt to individual editor behaviors? To answer these questions, we are building an agent-based model to simulate editors' activities and the process of article creation and maintenance.

## Stream 3: Modeling Innovation Diffusion and Algorithmic Marketing
Agent-based modeling has become the new paradigm to model innovation diffusion. A review of agent-based models (ABMs) of innovation diffusion revealed that few ABMs were calibrated properly, validated rigorously, and developed for prediction purpose. In my Ph.D. dissertation, I explored the use of machine learning techniques to harvest insights from large-scale data to ground an agent-based model to study the diffusion of residential solar panels. Computational diffusion models also make it possible that marketing decisions can be augmented or even automated by intelligent algorithms. My thesis also contributed a number of optimization algorithms in various marketing settings.

**A Review of Empirically-Grounded ABMs of Innovation Diffusion**

Agent-based modeling has become a popular approach to model innovation diffusion in many domains, such as sociology, economics, marketing, ecology, and computer science. We conducted a critical review of empirically grounded agent-based models of innovation diffusion and presented an overarching framework to categorize the research based on types of adoption decision models. Our review also showed great variance and the common absence of rigorous validation of the models. We proposed a relatively novel approach of using statistical inference methods such as maximum likelihood estimation for model calibration and validation purposes. __[[AI Review 2017](http://haifeng-zhang.github.io/files/abmsurvey.pdf)]__

**Agent-based modeling of solar adoption and diffusion**

In this work, we proposed a novel data-driven agent-based modeling framework, in which assumptions about individual behaviors were rooted in and parameterized by machine learning techniques, and validated using a holdout sample of collective adoption decisions. The model was successfully deployed to forecast residential rooftop solar adoption in San Diego County. We then ran counterfactual experiments with the model to evaluate the efficacy of a government incentive program, and virtual experimental results suggest potentially effective incentive structures and seeding strategies to promote higher solar adoption. __[[JAAMAS 2016](http://haifeng-zhang.github.io/files/ddabm.pdf)]__

**Optimizing Marketing Operations with intelligent algorithms**

Marketing operations to some extent can be treated as mathematical optimization problems with the goals to maximize influence, adoption or revenue. For example, product seeding is aimed to maximize the word-of-mouth effects by giving away free samples to potential influencers in social networks. The optimization of seeding strategies can be formulated as a maximization problem with an objective function that follows decreasing returns or submodularity, where a greedy algorithm is proven to have a good approximation of the optimal solution. 

The influence of new users on future adoptions may vary depending on the stages of innovations. For instance, a new adoption in the early stage of technology diffusion may have a greater marginal impact on others' likelihood of adoption than in the later stage. We refer to this property as increasing returns. How can one optimize seeding strategies in such a market? We formulated this question as a dynamic influence maximization problem and presented a simple but optimal strategy to optimize the marketing budget to various stages of the diffusion cycle. We experimentally verified the performance of the algorithm and also identified conditions under which its optimality guarantee does not hold but a more effective and general algorithm was proposed. __[[AAMAS 2015](http://haifeng-zhang.github.io/files/influmax.pdf)]__ 

Marketing, in reality, can face complex constraints. For example, in door-to-door marketing, salesmen often face routing constraints. Unfortunately, the classic mathematical framework, like submodular optimization only deals with cardinality or cost constraints. We therefore investigated the problems of maximizing a submodular function subject to routing cost constraints and proposed a generalized cost-benefit greedy algorithm with proven approximation guarantees. Experiments on both real networks from mobile sensing and door-to-door marketing and simulated networks demonstrated the efficiency of our algorithm. __[[AAAI 2016](http://haifeng-zhang.github.io/files/submax.pdf)]__  

In contemporary marketing, increased availability of data and computing resources has advanced the development of sophisticated computational models to estimate and optimize advertising outcome (i.e., sales or revenues) in different marketing channels. High-fidelity simulations and accurate predictive models can reduce decision uncertainty and risk greatly, but querying outcomes from these systems can be time-consuming. In addition, the fact that non-negligible budget increments are required for noticeable marginal impact also introduces intractable combinatorial structure to the decision space. This work was aimed to address the two computational challenges by solving a multi-choice knapsack problem, where the weights are not known but can be approximated by sending queries to outcome estimators. We developed an approximation algorithm that has proven optimality guarantee as well as several query strategies to achieve the approximation ratio in an online fashion. __[[AAMAS 2017](http://haifeng-zhang.github.io/files/multichan.pdf)]__