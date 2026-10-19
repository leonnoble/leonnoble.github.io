---
layout: page
title: research
permalink: /research/
description:
nav: true
nav_order: 3
---

<style>
  .rs-fig { margin: 0.4rem 0 1rem; }
  .rs-fig img { width: 100%; height: auto; background: #fff; border-radius: 4px; }
  .rs-fig figcaption { font-size: 0.85rem; margin-top: 0.4rem; color: var(--global-text-color-light); }
  @media (min-width: 768px) {
    .rs-float { float: left; width: 46%; margin: 0.3rem 1.4rem 0.6rem 0; }
  }
  .rs-clear { clear: both; }
  .rs-summary { margin: 1.5rem 0; }
  .rs-summary svg { width: 100%; height: auto; display: block; }
  .rs-summary svg text { fill: var(--global-text-color); font-family: inherit; }
  .rs-summary .on-fill { fill: #000; }
  .rs-summary .on-dark { fill: #fff; }
  .rs-cards { display: grid; grid-template-columns: repeat(auto-fit, minmax(170px, 1fr)); gap: 0.6rem; margin-top: 0.8rem; }
  .rs-card { border: 1.5px solid; border-radius: 5px; padding: 0.55rem 0.65rem; font-size: 0.8rem; line-height: 1.35;
             display: flex; flex-direction: column; justify-content: space-between; background: var(--global-card-bg-color); }
  .rs-card.eor { border-color: #E69F00; }
  .rs-card.post { border-color: #CC79A7; }
  .rs-card .ref { margin-top: 0.5rem; font-weight: 600; }
  .rs-card .ref a { font-weight: 700; }
</style>

I am a cosmologist working at the intersection of theory and observations to understand the Epoch of Reionization (EoR) and how neutral hydrogen traces large-scale structure afterward. The timing of the EoR, the sources that drove it, and the physical state of the intergalactic medium (IGM) remain uncertain. Line intensity mapping (LIM) of the 21-cm signal, together with other lines such as [CII] and CO, can map this epoch in three dimensions and address these questions. After reionization, in the post-EoR era, the same technique maps large-scale structure over cosmological volumes, acting as a probe of fundamental physics.

The SKA Observatory (SKAO) will provide unprecedented access to both eras, and its overlap with [CII] experiments such as FYST and with galaxy surveys such as *Euclid* enables multi-probe analyses. Because these signals are highly non-Gaussian, extracting their full information requires statistics beyond the power spectrum and robust inference methods. ***My research focuses on how much more we can learn about the EoR and post-EoR Universe by looking beyond the 21-cm power spectrum with SKAO, through the bispectrum, LIM--LIM cross-correlations and LIM--galaxy cross-correlations.*** I showed that the 21-cm bispectrum distinguishes reionization morphologies better than the power spectrum ([Noble et al. 2024](https://doi.org/10.1088/1475-7516/2024/10/003)), and I carried out the first study of the 21-cm--galaxy cross-bispectrum, forecasting a $>100\sigma$ detection with SKA-Mid and a *Euclid*-like survey ([Noble et al. 2026](https://arxiv.org/abs/2604.15440)); I now lead its first measurement in real data, from MeerKLASS. To make this possible, I developed estimators of higher-order statistics, GPU-accelerated multi-line LIM simulations, and a simulation-based inference pipeline for multi-line LIM and its cross-correlations.

<div class="rs-summary">
<svg viewBox="0 0 760 330" role="img" aria-label="Timeline of the EoR and post-EoR eras with the surveys and results of this research">
  <rect x="251" y="22" width="197" height="240" rx="3" fill="none" stroke="#E69F00" stroke-width="3"/>
  <rect x="251" y="2" width="197" height="20" fill="#E69F00"/>
  <text x="349.5" y="16" text-anchor="middle" font-size="13" font-weight="700" class="on-fill">Epoch of Reionization</text>
  <rect x="460" y="22" width="270" height="240" rx="3" fill="none" stroke="#CC79A7" stroke-width="3"/>
  <rect x="460" y="2" width="270" height="20" fill="#CC79A7"/>
  <text x="595" y="16" text-anchor="middle" font-size="13" font-weight="700" class="on-fill">post-EoR</text>

  <g stroke-width="5" stroke-linecap="round">
    <line x1="637" y1="52" x2="747" y2="52" stroke="#56B4E9"/>
    <line x1="625" y1="85" x2="755" y2="85" stroke="#56B4E9"/>
    <line x1="629" y1="118" x2="751" y2="118" stroke="#56B4E9"/>
    <line x1="364" y1="154" x2="629" y2="154" stroke="#F0E442"/>
    <line x1="357" y1="203" x2="616" y2="203" stroke="#009E73"/>
    <line x1="272" y1="245" x2="739" y2="245" stroke="#0072B2"/>
  </g>
  <g font-size="11" font-weight="700" text-anchor="middle">
    <rect x="652" y="43" width="60" height="18" rx="3" fill="#56B4E9"/><text x="682" y="56" class="on-fill">Euclid</text>
    <rect x="652" y="76" width="60" height="18" rx="3" fill="#56B4E9"/><text x="682" y="89" class="on-fill">LSST</text>
    <rect x="648" y="109" width="60" height="18" rx="3" fill="#56B4E9"/><text x="678" y="122" class="on-fill">Roman</text>
    <rect x="400" y="145" width="60" height="18" rx="3" fill="#F0E442"/><text x="430" y="158" class="on-fill">COMAP</text>
    <rect x="400" y="194" width="60" height="18" rx="3" fill="#009E73"/><text x="430" y="207" class="on-dark">CCAT</text>
    <rect x="445" y="236" width="60" height="18" rx="3" fill="#0072B2"/><text x="475" y="249" class="on-dark">SKAO</text>
  </g>
  <line x1="10" y1="290" x2="745" y2="290" stroke="currentColor" stroke-width="1.5" style="color: var(--global-text-color-light)"/>
  <path d="M745 290 l-8 -4 v8z" style="fill: var(--global-text-color-light)"/>
  <text x="10" y="316" font-size="12" style="fill: var(--global-text-color-light)">early Universe</text>
  <text x="745" y="316" font-size="12" text-anchor="end" style="fill: var(--global-text-color-light)">today</text>
  <text x="378" y="316" font-size="12" text-anchor="middle" style="fill: var(--global-text-color-light)">cosmic time</text>
</svg>
<div class="rs-cards">
  <div class="rs-card eor"><span>SKA-Low observations of the 21-cm bispectrum can distinguish between different reionization morphologies better than the 21-cm power spectrum.</span><span class="ref">Noble et al. 2024<br><a href="https://arxiv.org/abs/2406.03118">arXiv:2406.03118</a></span></div>
  <div class="rs-card eor"><span>The 21-cm marked power spectrum yields tighter constraints on EoR model parameters than the 21-cm power spectrum.</span><span class="ref">Pandya, Noble et al. 2026<br><a href="https://arxiv.org/abs/2605.18301">arXiv:2605.18301</a></span></div>
  <div class="rs-card eor"><span>Jointly inferring the SKA-Low 21-cm signal with [CII] LIM from CCAT yields tighter constraints on reionization source parameters than the 21-cm auto-correlation alone.</span><span class="ref">Noble et al.<br><em>in prep.</em></span></div>
  <div class="rs-card post"><span>The 21-cm--galaxy cross-bispectrum shows enhanced detectability compared to the 21-cm auto-bispectrum for all unique triangles with SKAO and Euclid.</span><span class="ref">Noble et al. 2026<br><a href="https://arxiv.org/abs/2604.15440">arXiv:2604.15440</a></span></div>
  <div class="rs-card post"><span>Impact of foreground contamination on the cross-bispectrum, and recovering the information lost in foreground-dominated Fourier modes with the 21-cm--galaxy cross-bispectrum.</span><span class="ref">Noble et al.<br><em>in prep.</em></span></div>
</div>
<p class="rs-fig" style="margin-bottom:0"><small style="color: var(--global-text-color-light)"><strong>Summary of my past and current research</strong> on how much more we can learn about the EoR and post-EoR Universe by looking beyond the 21-cm power spectrum with SKAO, through the bispectrum, LIM--LIM cross-correlations, and LIM--galaxy cross-correlations.</small></p>
</div>

## Probing the EoR with higher-order statistics of the 21-cm maps and 21-cm--[CII] cross-correlations

<figure class="rs-fig rs-float">
  <img src="{{ '/assets/img/research/bispectrum_xhi.png' | relative_url }}" alt="Evolution of the 21-cm bispectrum for different reionization scenarios" data-zoomable>
  <figcaption><em>Evolution of the 21-cm bispectrum for squeezed-limit $k$-triangles for different reionization scenarios with global neutral fraction (redshift). The 21-cm bispectrum can distinguish different reionization scenarios with 1000 hours of SKA-Low observations.</em></figcaption>
</figure>

The 21-cm signal from the EoR is highly non-Gaussian, and higher-order statistics, such as the bispectrum, are required to quantify it. Inference with the bispectrum can provide tighter constraints on reionization model parameters than the power spectrum alone. However, ***it remained unknown whether the bispectrum can distinguish different reionization morphologies, and thereby reveal which sources drove reionization***. In [Noble et al. (2024)](https://doi.org/10.1088/1475-7516/2024/10/003), I answered this using a suite of simulations with different reionization scenarios, which show inside-out, outside-in, and a combination of inside-out and outside-in reionization morphologies. ***I demonstrated that SKA-Low observations of the 21-cm bispectrum can quantify the time-evolving non-Gaussianity of these models across all triangle shapes and sizes and distinguish among these reionization morphologies***. I further showed that using the sign and magnitude of the bispectrum, and the sequence of its sign changes across redshift, can distinguish different reionization scenarios better than the 21-cm power spectrum.

In addition to the bispectrum, various other statistics, including the marked power spectrum, can quantify non-Gaussianity in the signal and be incorporated into a Bayesian inference framework. The marked power spectrum is computationally cheaper than the bispectrum. However, ***its constraining power depends heavily on the choice of mark, and no prescription exists for EoR 21-cm maps***. In [Pandya & Noble et al. (2026)](https://arxiv.org/abs/2605.18301), we introduced a set of EoR-tailored mark functions and investigated both the power spectrum of the mark and that of the marked fields. We established which marks one should choose for the EoR 21-cm maps, and showed that ***the marked power spectrum yields tighter constraints on EoR model parameters than the power spectrum***.

Synergies between the 21-cm signal and other EoR probes, including [CII] and CO LIM, offer a promising path to validate the first 21-cm signal detection, enhance the signal-to-noise ratio (SNR), and provide complementary physical insights into the galaxy--IGM connection. However, ***the information content of such cross-correlations and whether they improve constraints on the properties of the sources of reionization remain unknown***. To answer this, I developed a new suite of GPU-accelerated multi-line intensity mapping simulations and a simulation-based inference (SBI) framework. In Noble et al. (in prep; to be submitted to ApJ), ***I demonstrated that jointly inferring the SKA-Low 21-cm signal with [CII] LIM delivered by CCAT will yield tighter constraints on reionization source parameters than the auto-correlation of the 21-cm signal alone***. This framework is directly extensible to CO LIM, galaxy surveys, and higher-order statistics.

<div class="rs-clear"></div>

## Road toward detecting the post-EoR 21-cm signal bispectrum in cross-correlation with galaxy surveys

<figure class="rs-fig rs-float">
  <img src="{{ '/assets/img/research/snr_all_bispectra_500hrs.png' | relative_url }}" alt="SNR for the 21-cm auto-bispectrum and 21-cm-galaxy cross-bispectrum" data-zoomable>
  <figcaption><em>The SNR for detecting the 21-cm auto-bispectrum and the 21-cm--galaxy cross-bispectrum for all unique triangles at $z = 0.99$ with SKA-Mid (interferometric mode) and a <em>Euclid</em>-like galaxy survey. The 21-cm--galaxy cross-bispectrum shows enhanced detectability compared to the 21-cm auto-bispectrum for all unique triangles.</em></figcaption>
</figure>

Post-reionization 21-cm intensity mapping has now entered the era of detections. The first detections came in cross-correlation with galaxy surveys, and only recently has the 21-cm auto-power spectrum been detected by MeerKAT and CHIME. The post-EoR 21-cm signal is non-Gaussian, owing to non-linear clustering, complex astrophysics, and primordial non-Gaussianity, and higher-order statistics such as the bispectrum are required to quantify it. Cross-correlation with galaxies was the route to the first 21-cm power spectrum detections, because it suppresses foregrounds and systematics that are uncorrelated between the two tracers. The natural next step, the cross-bispectrum between the 21-cm signal and galaxies, has not yet been explored in detail. This raises a key question: ***can the 21-cm--galaxy cross-bispectrum, measured with SKAO and galaxy surveys, deliver a high-significance detection of the non-Gaussian 21-cm signal and open a new window for cosmological inference beyond the power spectrum?*** In [Noble et al. (2026)](https://arxiv.org/abs/2604.15440), we modeled the 21-cm--galaxy cross-bispectrum for all unique triangles across different cross-combinations using predictions from the theoretical galaxy evolution model GAEA, defined on a large cosmological volume. ***I demonstrated that the 21-cm--galaxy cross-bispectrum shows enhanced detectability, by more than a factor of two, compared to the 21-cm auto-bispectrum for all unique triangles for the future SKAO and Euclid synergies***. In our follow-up work, Noble et al. (in prep), we are examining the impact of foreground contamination on the cross-bispectrum and investigating the idea of ***recovering the information lost in foreground-contamination-dominated Fourier modes using the 21-cm--galaxy cross-bispectrum***.



