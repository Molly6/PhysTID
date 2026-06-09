# PhysTID

**Physics-Inspired Spatio-Temporal Infrastructure Damage Assessment from Multi-Temporal Remote Sensing Imagery**

Reliable damage assessment of diverse infrastructures via remote sensing is paramount amidst frequent global disasters and conflicts.

However, unlike instantaneous failure scenarios, damage from multi-wave aftershocks or prolonged conflicts often exhibits progressive and cumulative characteristics.

Existing works predominantly focus on single post-disaster phases and are largely limited to individual object categories with binary damage detection, failing to characterize complex dynamic evolution patterns.

To bridge this gap, we introduce the first large-scale Disaster Dynamic Damage Dataset (D^3-Dataset), which provides long-term sequential observations with up to 17 temporal phases per event. Covering 15 functional sub-categories across airports, ports, and industrial parks, the D^3-Dataset introduces four-level damage annotations, supporting the requirements for fine-grained dynamic monitoring.

This task involves two critical challenges:

(i) spatial localization uncertainty, where post-disaster infrastructure fragmentation and displacement lead to the loss of geometric features, making precise boundary determination difficult; and

(ii) temporal state reversion, where interference from sensor discrepancies, smoke, or shadows causes the model to suddenly produce physically inconsistent "pseudo-self-healing" predictions at a certain observation phase.

To address these issues, we propose the Physics-inspired Spatio-Temporal Infrastructure Damage Assessment Network (PhysTID).

Specifically, in the spatial dimension, we introduce pre-disaster imagery as a physical geometric reference and design a Physics-inspired Spatio-temporal Deformable Mamba (PI-SDM) architecture to enhance localization accuracy.

In the temporal dimension, we incorporate the physical principle of short-term damage irreversibility into the training objective via a proposed Physics-inspired Soft-margin Monotonicity Loss (PISM-Loss), effectively suppressing unrealistic damage-level predictions.

Extensive experiments on the D^3 and other two related datasets demonstrate that PhysTID achieves state-of-the-art performance.

**After the paper is accepted, we will release the code and data.**
<img width="2458" height="800" alt="image" src="https://github.com/user-attachments/assets/30caccef-d216-44ca-9ce3-0efdffc09f6d" />

