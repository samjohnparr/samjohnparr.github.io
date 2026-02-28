---
layout: post
title: "My First International Conference Presentation: EASIAM 2025 (De La Salle University)"
date: 2025-07-03
categories: [conference, talks]
---

On **July 3, 2025**, I gave my first-ever paper presentation at **De La Salle University** in Manila during the **EASIAM Conference**, under the session theme *Mathematical and Computational Approaches to Modeling, Data, and Optimization in Complex Systems*. It was a **contributed talk**, and it honestly felt surreal to say that this was my first international presentation.

## A personal milestone
Walking into the venue, I felt that mix of excitement and nerves you get when you know you are stepping into something new. Seeing faculty and researchers from across East Asia, including Japan, China, South Korea, Taiwan, Singapore, Thailand, and the Philippines, reminded me that research can feel both big and small at the same time. Big, because the room is full of people doing serious work. Small, because you still start with one simple question and the courage to share what you found.

<p style="text-align:center;">
  <img src="/assets/blog/easiam-2025-presenting.jpg" alt="Me presenting at EASIAM 2025" style="width: 420px; max-width: 75%; height: auto;">
</p>

<p style="text-align:center;"><em>Presenting my MS thesis work on persistent homology-based early warning signals</em></p>


One thing I was really thankful for was being reunited with my MS classmate, Gio, who is now taking his PhD in Applied Mathematics at the **University of the Philippines Los Baños**. I was glad to have someone to talk to in my own language, **Bisaya**, especially in a setting where everything can feel formal and overwhelming. He has always been one of the smartest people I know, and catching up with him gave me confidence and comfort in the middle of a busy conference day.

<p style="text-align:center;">
  <img src="/assets/blog/me_and_gio.jpg" alt="Me and Gio" style="width: 420px; max-width: 75%; height: auto;">
</p>

<p style="text-align:center;"><em>Me, Gio, and THE LEGENDARY Dr. Jomar F. Rabajante</em></p>

## What I presented
I presented my MS thesis titled:

**A Persistent Homology Approach to Early Warning Signals in Philippine Epidemiological Data**

At the heart of the work is a practical problem: early detection of epidemic upswings remains difficult when surveillance time series are noisy, irregular, or affected by reporting artifacts. In real public health data, signals are rarely clean, and standard indicators can sometimes trigger late or raise false alarms.

## The idea in plain terms
The main idea is to track changes in the **shape** or **structure** of the data over time and use that as a foundation for early warning.

Using weekly national case counts for **dengue, measles, and COVID-19** in the Philippines, I followed a workflow like this:

1. **Turn time series segments into point clouds.**  
   I used delay embedding to represent sliding-window segments as low-dimensional point clouds.

2. **Summarize structure using persistent homology.**  
   For each window, I built a Vietoris–Rips filtration and computed persistent homology to capture how topological features evolve.

3. **Compress those summaries into a single monitoring signal.**  
   I derived persistence landscapes and reduced each window into a nonnegative L1-based measure, producing a topology-driven time series.

4. **Monitor early-warning indicators on the derived series.**  
   I tracked lag-1 autocorrelation, variance, and low-frequency spectral power using rolling windows, and assessed trends using a rank-based approach.

5. **Use a voting rule to reduce false alarms.**  
   A warning is issued only when at least two indicators are significant.

6. **Measure lead time using automated truncation.**  
   I used an automated truncation procedure to determine how far before the peak the warning pattern remains detectable.

## Key result
The method produced early warning lead times of:
- **10 weeks** for dengue  
- **27 weeks** for measles  
- **22 weeks** for COVID-19  

These results suggest that persistent homology can provide early warning information that complements standard surveillance analytics, especially when data are messy.

## Why this matters beyond academia
When I shared the work, I also pointed to potential practical directions, such as:
- integration into public health decision-support dashboards,
- automated outbreak monitoring services,
- analytics pipelines for hospitals and local health units to guide preparedness and resource allocation.

## What I’m taking forward
This experience reminded me how important it is to communicate clearly. A method is only useful if people can understand it, trust it, and see how it fits into real decision-making. More personally, it encouraged me to keep showing up in rooms like this, even when it is uncomfortable at first. That is where growth happens.