# ab-testing-social-contract
A/B test examining how reflecting on broken vs. kept institutional promises affects political discontent.

**Read the analysis report**
<a href="https://deanbaltiansky.github.io/ab-testing-social-contract/" target="_blank">
https://deanbaltiansky.github.io/ab-testing-social-contract/
</a>

# Overview

This repository contains the design and analysis of a **randomized A/B experiment** testing whether reflecting on a broken social contract causally increases political discontent.

Participants were randomly assigned to reflect on a core institutional promise as either being kept, broken, or simply defined (active control). The experiment evaluates whether a short, targeted writing prompt can shift attitudes that are typically stable, allowing for clear interpretation of directionality and causal effects.

The study was conducted as part of a Time-sharing Experiments for the Social Sciences (TESS) project and fielded on NORC’s AmeriSpeak panel, a nationally representative U.S. probability sample. The design was competitively peer-reviewed and supported by federal funding prior to data collection.

The repo demonstrates an experimentation workflow using attitudinal outcomes, randomized treatment, and baseline comparisons.

# Experimental design

A nationally representative U.S. sample was first situated in the context of the Constitution as a set of promises to American citizens.

The experiment proceeded in three steps:

  1. **Value identification**
     Participants listed several values they believed the U.S. stands for *on paper* and selected the single value they believed was most central to the U.S.'s promise. This value was then embedded in the second step of the experiment.
  2. **Randomized writing prompt**
     Participants were randomly assigned to one of three conditions:
     - **Promise Kept**: reflected on how the U.S. *IS* living up to its promise of that value
     - **Promise Broken**: reflected on how the U.S. *IS NOT* living up to its promise of that value
     - **Control**: defined that value
  3. **Outcome measurement**
     Participants then completed three randomly-ordered validated measures of three consequential aspects of political discontent:
     - **Anti-establishment sentiment**
     - **Trust in government**
     - **Support for radical change**

# Analysis approach

  - **Primary effects**: For each outcome, the report estimates differences between the two experimental conditions (*Broken* vs. *Kept*) to assess whether a reflecting on a broken social contract leads to higher political discontent than reflecting on a social contract being upheld.
  - **Direction of the effects**: For each outcome, the report then compares the two experimental conditions to the control condition, adjusting for multiple comparisons with Tukey-HSD p-value corrections. This establishes whether a broken social contract *increases* political discontent, compared to baseline, or whether an in tact social contract *decreases* political discontent, compared to baseline.

# Why this matters

Many explanations of political discontent rely on correlational evidence or stable individual differences. This experiment shows that brief, targeted framing of institutional performance can causally shift otherwise stable political attitudes, highlighting the role of the **subjective experience of a broken social contract**.

# What this repo shows

  - Designing and analyzing a multi-condition A/B experiment
  - Working with attitudinal outcome measures
  - Using active control conditions to establish directionality
  - Communicating causal results clearly for non-academic audiences
