---
layout: post
title: "My First International Conference Presentation: EASIAM 2025 (De La Salle University)"
date: 2025-07-03
categories: [conference, talks]
---

## Event details
- **Conference:** Mathematical and Computational Approaches to Modeling, Data, and Optimization in Complex Systems  
- **Organized under:** East Asia Section of the Society for Industrial & Applied Mathematics (EASIAM) Conference  
- **Presentation type:** Contributed Talk  
- **Venue:** De La Salle University, Manila, Philippines  
- **Date:** July 3, 2025  

## A personal milestone
This was my first international conference presentation. Walking into the venue and seeing faculty and researchers from East Asia, including Japan, China, South Korea, Taiwan, Singapore, Thailand, and the Philippines, made the experience both exciting and humbling. It reminded me that my work, even if grounded in Philippine data, participates in a wider research conversation.

## Photo from the presentation
<img src="/assets/blog/easiam-2025-presenting.jpg" alt="Me presenting at EASIAM 2025" style="width: 420px; max-width: 75%; height: auto;">

*Presenting my MS thesis work on persistent homology-based early warning signals.*

## What I presented
I presented my MS thesis titled:

**A Persistent Homology Approach to Early Warning Signals in Philippine Epidemiological Data**

The core problem I addressed is practical and urgent: early detection of epidemic upswings remains difficult when surveillance time series are noisy, irregular, or affected by reporting artifacts. In many real settings, clean signals are rare, and standard indicators can trigger late or produce false alarms.

## The idea in plain terms
My approach builds an early-warning pipeline that tracks **changes in the “shape” of the data** over time.

Using weekly national case counts for **dengue, measles, and COVID-19** in the Philippines, I applied a unified workflow:

1. **Convert time series windows into geometric objects.**  
   I used delay embedding to transform sliding-window segments into low-dimensional point clouds.

2. **Summarize structure using persistent homology.**  
   For each window, I constructed a Vietoris–Rips filtration and computed persistent homology to capture evolving topological features.

3. **Compress topological summaries into a single monitoring signal.**  
   I derived persistence landscapes and reduced them into a nonnegative L1-based measure per window, producing a topology-driven time series.

4. **Monitor early-warning indicators on the derived series.**  
   I tracked lag-1 autocorrelation, variance, and low-frequency spectral power using rolling windows, then tested trends with a rank-based approach.

5. **Reduce false alarms using a voting rule.**  
   A warning is issued only when at least two indicators are significant.

6. **Quantify lead time with automated truncation.**  
   I used an automated truncation procedure to determine how far before the peak the warning pattern remains detectable.

## Key result
The method produced early warning lead times of:
- **10 weeks** for dengue  
- **27 weeks** for measles  
- **22 weeks** for COVID-19  

These results suggest that persistent homology can provide robust early warning information that complements standard surveillance analytics.

## Why this matters beyond academia
I shared possible operational directions, including:
- integration into public health decision-support dashboards,
- automated outbreak monitoring services,
- analytics pipelines for hospitals and local health units to guide targeted preparedness and resource allocation.

## What I’m taking forward
This experience strengthened my motivation to keep building tools that are mathematically sound and operationally realistic. It also reminded me that communicating clearly matters. A method is only useful if it can be understood, trusted, and implemented by people who make real decisions.

---

**Keywords:** Persistent homology, early warning, epidemics, surveillance, Philippines