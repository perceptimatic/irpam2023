**Pre-trained acoustic models** learned in an unsupervised fashion have exploded in the domain of speech. The representations discovered by CPC, wav2vec 2.0, HuBERT, WavLM, and others, can be used to massively reduce the amount of labelled data to train speech recognizers; they also produce excellent speech resynthesis.

However, while pre-trained acoustic representations seem to be nicely isomorphic with phones or phone states under optimal listening conditions (see, for example, [here](https://proceedings.neurips.cc/paper/2020/hash/92d1e1eb1cd6f9fba3227870bb6d7f07-Abstract.html), [here](https://ieeexplore.ieee.org/abstract/document/9414776/?casa_token=odmFOIWEJoAAAAAA:LNdam3N45ZkSWPKGokHWJN71qJd_kgII8LM0L4tqvt2hKEOa5VgUC_DZRf2XIpZpGc-Zp6M)), very little work has addressed **invariances.** Do the representations remain consistent across instances of the same phoneme in **different phonetic contexts** (i.e., are they *phonemic* or merely *allophone* representations)? Do they hold up under **noise and distortions**? Are they invariant to different **talkers and/or accents**?



The limited research that has addressed these questions directly suggests:
- that state-of-the-art models [have some degree of robustness to talker change](https://ieeexplore.ieee.org/abstract/document/9888095?casa_token=q5yNt_-Ax6UAAAAA:ZTb5yGkCyUMxhwKXtKx-yWggIhofX0f-9LwHIh-DQCzjso5zONobs5s_ld07Rfb-oxtaUVQ)
- that they [are fragile when surrounding phonetic context changes](https://arxiv.org/abs/2210.15775)
- and that they [are highly sensitive to noise and distortions, including time-dilation](https://arxiv.org/abs/2209.15483)
However, this research remains extremely limited: evaluation is limited to a few models, and the two standard benchmarks ([**ZeroSpeech:**](https://zerospeech.com/) intrinsic representation quality; **[SUPERB](https://superbbenchmark.org/), [SUPERB-SG](https://arxiv.org/abs/2203.06849):** downstream tasks) only assess talker invariance, and only in a superficial way. There is no standard evaluation for invariance to context, noise, and other distortions, and only limited evaluation of talker-/accent-invariance.

Progress on these issues could unlock new levels of performance on higher-level tasks such as word segmentation, named entity recognition, and language modelling, where using the discretized “units” discovered by pre-trained acoustic models still lag behind state-of-the-art text-based models. Importantly, progress on talker and accent robustness would contribute to the serious fairness problem that current ASR models have (including those using pre-trained acoustic models as features) whereby [lower socioeconomic status is highly correlated with higher word error rate](https://arxiv.org/abs/2110.08583).

This special session aims to address both the **evaluation problem**and the **problem of invariance** in pretrained acoustic models.

We invite researchers to submit papers in one of two tracks.

1. The **evaluation track** will accept proposed systematic **evaluation measures, test sets,** or **benchmarks** for pre-trained acoustic models, including but not limited to context-invariance, talker-invariance, accent-invariance, or robustness to noise and distortions. In the interest of in-depth validation of the proposed evaluations in the  limited Interspeech page limit, such papers should *not* propose new models.
2. The **model track** will propose new models or techniques and demonstrate empirically that they improve the invariance or robustness properties of pre-trained speech representations, evaluating using existing approaches or variants on existing benchmarks/measures. This could also include techniques for disentanglement in pre-trained acoustic models. Models submitted to this track must *not* propose new evaluation measures, and must use standard, existing evaluations.

Suggested evaluations for the model track include:
- [ZeroSpeech](https://zerospeech.com) Task 1 (acoustic) evaluations, focusing on **within versus across-speaker** measures as well as the brand new **within versus across-context** measures of context invariance, based on this [recent paper](https://arxiv.org/abs/2210.15775)
-


### Organizers
- Ewan Dunbar, University of Toronto
- Emmanuel Dupoux, École des Hautes Études en Sciences Sociales / École Normale Supérieure / Meta
- Hung-yi Lee, XXX
- Abdelrahman Mohamed

### Call for papers
Submissions for IRPAM will follow the same schedule and procedure as the main conference. More details to come.

### Important Dates
- Paper submission deadline: XXX, 23:59, Anywhere on Earth.
- Paper update deadline: XXX, 23:59, Anywhere on Earth.
- Author notification: XXX
- Interspeech conference dates: XXX

### Contact
If you have any questions, please contact us at XXX@gmail.com.

