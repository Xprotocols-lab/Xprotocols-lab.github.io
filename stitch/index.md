---
layout: stitch
title: "Stitch: Assertion-Guided Patching of On-Chip Protocol Implementations using LLMs"
content_type: abstract
permalink: /stitch/
---

## Abstract

Verification flows use Verification IPs to identify assertion violations in on-chip protocol implementations, but patching those violations still requires manual effort. A good patch must not only fix the violation but also preserve functionality without introducing new violations. We propose Stitch, based on the intuition that given an implementation, a violated assertion and a counterexample, an LLM can synthesize patches. To evaluate Stitch, we built a dataset of 100 violations across 11 implementations of 5 protocols (AXI, AHB, APB, Wishbone, TileLink). Our first experiment reports a 19% success rate across four LLMs (GPT-4, GPT-5, Gemini, Claude). By analyzing the failed cases, we devised three improvement strategies — patch localization, violation-specific context (cone of influence, counterexample), and iterative feedback from model-checker outputs — that raise Stitch's success rate to 61%, with GPT-5 dominating at 56%. We validate Stitch's patches through simulation and on real hardware, and compare Stitch to three state-of-the-art non-LLM tools and existing patches.

## Contributions

<div class="pics">
  <figure class="pic">
    <img src="{{ '/assets/implementation_logo.png' | relative_url }}" alt="Stitch">
    <figcaption><strong>Stitch</strong><br>Automated patching of on-chip protocol implementations</figcaption>
  </figure>
  <figure class="pic">
    <img src="{{ '/assets/icon-implementations-checklist.png' | relative_url }}" alt="Implementations">
    <figcaption>Patched 11 implementations across 5 protocols</figcaption>
  </figure>
  <figure class="pic">
    <img src="{{ '/assets/icon-dataset-database.png' | relative_url }}" alt="Dataset">
    <figcaption>Dataset of 100 violations of on-chip communication protocols</figcaption>
  </figure>
</div>
