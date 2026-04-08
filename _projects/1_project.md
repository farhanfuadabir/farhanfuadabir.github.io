---
layout: page
title: Multimodal Ultrasound Intelligence
description: Fusing ultrasound imagery with lean clinical biomarkers for rare tumor diagnosis.
img: assets/img/4.jpg
importance: 1
category: research
related_publications: true
---

I am building a multimodal pipeline that pairs B-mode ultrasound imagery with minimally invasive clinical features to assist radiologists diagnosing Phyllodes tumors and pleural effusions. The system features:

- **Feature-level fusion:** Dual-branch encoders that learn complementary representations from ultrasound sweeps and structured vitals, followed by cross-attention to emphasize mutually supportive cues.
- **Trust layer:** CAM- and Grad-CAM++-based saliency overlays tuned for sonographers, plus lightweight textual rationales distilled from the structured branch.
- **Data realism:** A diffusion-driven augmentation module that synthesizes high-fidelity B-mode variants for the minority tumor classes, easing class imbalance without overfitting.

The model is deployed in a prototype review studio built with Gradio, enabling physicians to scrub frames, toggle saliency layers, and audit the minimal clinical context that informed every prediction. This work was recently accepted at IEEE BSN'25.
