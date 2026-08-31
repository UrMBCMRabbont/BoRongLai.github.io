---
title: "ACT with a DINO Backbone for Bimanual Imitation Learning"
excerpt: "Swapping ACT's ResNet-18 vision encoder for DINO, raising cube-grasping success by 20% on an SO-101 arm."
collection: portfolio
---

Extended **ACT** (Action Chunking with Transformers) for bimanual imitation learning on an **SO-101** arm.

**What I changed**
* Replaced the stock **ResNet-18** vision encoder with a **DINO** backbone, raising task success rate by **20%** on a cube-grasping task
* Refactored temporal ensembling to expose action-chunk size and inference stride as configuration, so both could be varied for controlled ablation instead of being baked into the policy

*Dimeidos, Kaohsiung — 2026*
