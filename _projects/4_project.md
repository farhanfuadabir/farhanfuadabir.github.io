---
layout: page
title: ASL Dataglove
description: Low-cost wearable that recognizes 40 American Sign Language gestures in real time.
img: assets/img/2.jpg
importance: 4
category: hardware
related_publications: true
---

The ASL Dataglove started as my undergraduate capstone project and now powers outreach demos for inclusive communication.

- **Custom hardware.** Designed a light, fabric-friendly glove with flex sensors on each finger, a 9-DOF IMU, and haptic feedback for bidirectional cues. The board can be fabricated locally for <$35.
- **Datasets.** Collected two datasets covering 14 static and 3 dynamic ASL gestures from 35 participants, capturing inter-user variance that most public sets miss.
- **Modeling.** Created a domain-transformation pipeline (time–frequency embeddings + CNN) and a temporal CNN-LSTM hybrid that runs on-device using TensorFlow Lite.

The system recognizes gestures in under 40 ms with >92% accuracy and has been open-sourced for community labs. It also inspired our Scientific Reports paper on low-cost gesture recognition.
