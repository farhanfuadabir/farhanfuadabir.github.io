---
layout: page
title: PCovNet+
description: Smartwatch-powered anomaly detection for presymptomatic COVID-19 monitoring.
img: assets/img/8.jpg
importance: 3
category: health-tech
related_publications: true
---

PCovNet+ is a CNN-VAE framework augmented with LSTM embeddings that I co-developed at Qatar University to detect the earliest physiological signatures of COVID-19.

Highlights:

- Processes raw PPG, accelerometer, and heart-rate traces from commodity smartwatches and learns per-user baselines.
- Hybrid reconstruction + prediction losses capture both patterned deviations and sudden spikes.
- LSTM embeddings retain circadian rhythms, reducing false alarms from schedule or workout changes.
- Lightweight enough to run on mobile gateways with federated fine-tuning.

In longitudinal field trials the model flagged presymptomatic cases up to 36 hours before PCR confirmation, offering a pragmatic blueprint for future wearable epidemiology platforms.
