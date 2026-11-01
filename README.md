# K2IA

**Knowledge-Informed Imagination Augmentation for Voltage Stability Emergency Control**

K2IA is a reusable mechanism that enhances existing control policies **without retraining their policy networks**. It coordinates load-shedding timing, location, and magnitude to improve voltage recovery while limiting unnecessary supply interruption.

## Method

The mechanism combines three components:

1. **Dynamic surrogate construction:** Learn voltage responses from recorded trajectories to rapidly evaluate candidate control actions.
2. **Knowledge-informed action candidates:** Retain engineering choices alongside the base-policy action, including waiting, alternative shedding magnitudes, different control locations, and no further shedding.
3. **Multi-step imagination:** Compare predicted recovery and shedding consequences along independent candidate trajectories, execute the selected first action, and update decisions using measured feedback.

The study evaluates augmentation of SAC, PPO, DDPG, and a distilled student policy.

## Manuscript and Code Availability

The accompanying manuscript is being prepared for submission to the **IEEE Power & Energy Society General Meeting (PESGM)**.

This repository currently provides a project overview. **Source code and reproducibility materials will be released here after the manuscript has been submitted to PESGM.**

## Authors

Dingyang Suo, Yu Zhao, and Jun Liu  
Xi'an Jiaotong University, China
