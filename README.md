# SCMRE DATASET

# Original Dataset
The SCMRE corpus is organized by incorporating each generated event, including actions and referring expressions, as a distinct sample. 
The elicitation process resulted in a total of 10,408 events, including 7,681 pointing-only references, 551 transitive attributive events, 641 attributive events, 369 relational events, 27 historical events, 453 non-executed events, 
and 686 non-referencing events, which include 428 undoing events, 118 refusal events, and 117 affirmative events. 
In terms of modalities used by humans, 575 events were generated multimodally by mixing deixis and language, 7,681 events were generated using pointing-only, and 2,152 events were generated using speech-only.

| Events                                          | Modalities            | Quantity | Total        |
|------------------------------------------------------------------|--------------------------------|-------------------|------------------------|
| Attributive Multimodal Events                                    | Multimodal   | 186               | 575   |
| Transitive Attributive Multimodal Events  |                                | 302               |                        |
| Relational Multimodal Events              |                                | 48                |                        |
| Historical Multimodal Events              |                                | 3                 |                        |
| Not executed multimodal events            |                                | 36                |                        |
| Focus and target pointing                                 | Pointing-Only                  | 7,681             | 7,681                  |
| Attributive Speech Only Events                            | Speech-Only | 455               | 2,152 |
| Transitive attributive speech only events |                                | 249               |                        |
| Relational speech-only events             |                                | 321               |                        |
| Historical speech-only events             |                                | 24                |                        |
| Non-referencing speech-only               |                                | 686               |                        |
| Not executed speech-only events           |                                | 416               |                        |
| Total                                     | 10,408                         |

# Augmented Dataset

A data augmentation method was utilized to increase both
the size and diversity of SCMRE. Specifically, we employed the Synonym Aug-
mentation technique from the NLPAug library to expand the range of mul-
timodal and speech-only referring expressions. Each original expression was aug-
mented to produce three similar expressions.

# Synthesized Dataset

Despite the expansions resulting from augmentation, the dataset
remained imbalanced, particularly in multimodal REs, potentially affecting the
robustness of MRE generative model training. To augment the dataset with di-
verse multimodal samples, we synthesized individual pointing-only and speech-
only samples to create new multimodal RE samples. 

| Dataset             | Speech-Only REs | Multimodal REs | Pointing-Only REs | Total           |
|----------------------------|-----------------|----------------|-------------------|-----------------|
| Original Dataset    | 2,152           | 575            | 7,681             | **10,408** |
| Augmented Dataset   | **6,550**  | **2,296** | 7,681             | **16,527** |
| Synthesized Dataset | 6,550           | **7,928** | 7,681             | **22,159** |

