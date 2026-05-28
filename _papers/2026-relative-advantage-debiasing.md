---
title: "Relative Advantage Debiasing for Watch-Time Prediction in Short-Video Recommendation"
collection: papers
# category: manuscripts
permalink: /_papers/2026-relative-advantage-debiasing
excerpt: 'This work tackles the challenge of using watch time as a signal for user preference in video recommendation systems. Raw watch time is heavily influenced by factors like video length, popularity, and individual user habits, which can distort what users actually enjoy. We introduce a relative-advantage debiasing framework that compares a user’s watch time to reference distributions conditioned on similar users and items, producing a quantile-based, more reliable measure of preference. Our two-stage architecture cleanly separates the tasks of distribution estimation and preference learning, and we further develop distributional embeddings that make quantile prediction efficient without storing historical data. Both offline and live experiments show substantial gains in accuracy and robustness over existing approaches.'
date: '2026-01-20'
venue: 'AAAI 2026'
# slidesurl: 'http://academicpages.github.io/files/slides1.pdf'
paperurl: 'https://arxiv.org/pdf/2508.11086'
citation: 'Relative Advantage Debiasing for Watch-Time Prediction in Short-Video Recommendation. Emily Liu, Kuan Han, Minfeng Zhan, Bocheng Zhao, Guanyu Mu, Yang Song. Association for the Advancement of Artificial Intelligence (AAAI) Conference 2026.'
---

Watch time is widely used as a proxy for user satisfaction in video recommendation platforms. However, raw watch times
are influenced by confounding factors such as video duration, popularity, and individual user behaviors, potentially
distorting preference signals and resulting in biased recommendation models. We propose a novel relative advantage
debiasing framework that corrects watch time by comparing it to empirically derived reference distributions conditioned
on user and item groups. This approach yields a quantilebased preference signal and introduces a two-stage architecture that 
explicitly separates distribution estimation from preference learning. Additionally, we present distributional embeddings to 
efficiently parameterize watch-time quantiles without requiring online sampling or storage of historical data. 
Both offline and online experiments demonstrate significant improvements in recommendation accuracy and robustness compared to existing baseline methods.