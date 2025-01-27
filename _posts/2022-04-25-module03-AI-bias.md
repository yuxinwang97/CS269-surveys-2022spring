---
layout: post
comments: true
title: "Module 3 Survey: On the Emergence and Elimination of Biases in Artificial Intelligence"
author: Sidi Lu and Yufeng Li and Yuxin Huang and Rakesh Bal
date: 2021-04-25
---


> While being applied to a wider and wider range of scenarios, artificial intelligence algorithms can still be less helpful or even potentially harmful in many aspects, like social equity or the reliability of fundamental services in our society. We hereby conduct a broad-ranged survey of existing analysis of such, and try to compile the underlying ideas into a systematic understanding of the problem to facilitate the future research.

<!--more-->
{: class="table-of-content"}
* TOC
{:toc}

## How AI Biases Emerge from Mis-estimating the correlations of factors.
In the classical understanding, people use the term "AI bias" to describe two major classes of existing problems: dataset bias and the algorithmic bias (sometimes as the consequence of the former one)

For dataset bias, the most worrisome (and common) case is that the model over-constructs the logical correlations between different factors in the data based purely on the observed co-occurences. For example, some recent reports show an overly-constructed racial bias in superresolution models [2] <span style="color:red">[Sidi: Please help add in figures and expand the description]</span>, which could indicate a bigger, under-explored problem. While we can tell and probably name some of such overly-constructed correlation, another important class of problems are even more of a hot potato: for example, the lack of diversity in how each dataset respectively presents the world. Datasets with such problems hinder effective cross-dataset generalization and introduce irrelevant, anonymous factors that affect models' compositional generalizabilitys[3] <span style="color:red">[Sidi: Please help add in figures and expand the description]</span>.

But still, algorithm-wise, regardless of all these concerns, ever after connectionism methods re-conquered the mainstream of AI, data-driven methods with connectionism philosophy have been producing impressive milestone-level results, refreshing people's understanding and expectations of which. There's no doubt that data-driven methods do have their merits, and are ususally the ones with the best practical rationality [4]. <span style="color:red">[Sidi: Please help expand the description]</span> This is understandable under necessary assumptions, as such methods try to honestly reflect what the data indicate. When the test cases are similar, such reflection of data directly contributes to model performance. However, without proper inductive bias, the usage of highly data-driven logic is doomed to limit models' general ability to transfer. Unlike in cases where typical mispredictions come from mis-constructed belief between **almost identical factors**, tranferrabilities to new domains set up a higher standard for models as the actual situation could be testing how belief is well-constructed also for **varied group of factors** (depending on the relative complexity of the source/target domains).

Long story short, as part of the results of our compromise between effective practice and well-estabilished theory, AI Bias is a real, inevitable problem in most data-driven models that we can think of. It is not something we can easily locate within how we design the methodology and eliminate from the root trivially. A better pracitice would definitely be to admit them and to resolve the emerging ones in response.

## Existing Efforts in AI De-biasing
Based on our previous discussion, a natural thought would be to blame all the things on the problematic data. Some would argue that data could be nothing but a sincere reflection of the world, and that the AI bias, at the end of day, is essentially _**OUR**_ bias.

While this could be arguably correct in philosophy, in practice, recent discussions gradually lead to a more practical conclusion that, we need to move beyond the idea of "algorithmic bias is a data problem" due to multiple reasons[5]. <span style="color:red">[Sidi: Please help expand the description]</span>

Some well-founded approaches have been achieved following this way of thinking in the past few years. For example, one work [6] discussed in detail how such de-biasing can be achieved (at least by a large margin) in caption generation models. <span style="color:red">[Sidi: Please help expand the description]</span>

Some of those attempts for commercial purposes[7], however, still rely on data pre/post-processing to mitigate the data-related bias in their business models that could have negative impacts on their profit statistics. <span style="color:red">[Sidi: Please help expand the description]</span>

In general, mitigating the AI bias in multiple levels has been granted more and more attention. As the solutions stabilize and fushion, it's definitely more than just a hope to solve the problem.

## Essentially addressing the AI Bias problem?
Unfortunately, up to now, addressing the AI Bias problem is still beyond the best of our ability. However, more and more studies, with relaxed assumption of training/inference data beyond the classicial _i.i.d._ assumption, have been conducted [8,9,10]. While they are no essential solutions, step by step, they still shed light on how we can improve the model robustness towards (harmful) biases, and possibly defend the AI Bias-related consequences as a dynamic solution (rather than a static, ideal, essential solution).  
## Reference

[1] Redmon, Joseph, et al. "You only look once: Unified, real-time object detection." *Proceedings of the IEEE conference on computer vision and pattern recognition*. 2016.

[2] Vincent, James. "What a machine learning tool that turns Obama white can (and can’t) tell us about AI bias." Retrieved October 28 (2020): 2021.

[3] Torralba, Antonio, and Alexei A. Efros. "Unbiased look at dataset bias." CVPR 2011. IEEE, 2011.

[4] Sutton R. The bitter lesson[J]. Incomplete Ideas (blog), 2019, 13: 12.

[5] Hooker, Sara. "Moving beyond “algorithmic bias is a data problem”." Patterns 2.4 (2021): 100241.

[6] Hendricks, Lisa Anne, et al. "Women also snowboard: Overcoming bias in captioning models." Proceedings of the European Conference on Computer Vision (ECCV). 2018.

[7] Lee, Nicol Turner, Paul Resnick, and Genie Barton. "Algorithmic bias detection and mitigation: Best practices and policies to reduce consumer harms." Brookings Institute: Washington, DC, USA (2019).

[8] Mao, Jiayuan, et al. "The neuro-symbolic concept learner: Interpreting scenes, words, and sentences from natural supervision." arXiv preprint arXiv:1904.12584 (2019).

[9] Johnson, Justin, et al. "Clevr: A diagnostic dataset for compositional language and elementary visual reasoning." Proceedings of the IEEE conference on computer vision and pattern recognition. 2017.

[10] Lu, Sidi, et al. "Neurally-guided structure inference." International Conference on Machine Learning. PMLR, 2019.

---
