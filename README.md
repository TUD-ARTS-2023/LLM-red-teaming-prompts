# Red teaming prompts for LLMs

⚠️ **WARNING: Sensitive Content** ⚠️

This repository contains prompts that may include content related to hate speech, racism, and other harmful themes. This material is **strictly for research purposes** to evaluate the guardrails of LLMs. It is not intended to harm, offend, or promote harmful behavior. Use this material with caution and be aware of its potentially offensive nature.

## Overview

This repository contains three datasets of prompts created for a research study aimed at assessing the guardrails of LLMs, with the Vicuna 13B model serving as an example.

- **Dataset 1: Baseline Prompts** | "baseline_prompts.csv"
  - Compromises 100 red-teaming prompts across 10 harm categories to assess the default guardrails of the LLM.

- **Dataset 2: Harmful LLM Conversations** | "conversations"
  - Features 180 conversations with the Vicuna 13B LLM with red-teaming prompts that successfully provoked harmful responses. The conversations are stored in .yaml files for each red-teaming technique.

- **Dataset 3: Teaching Prompts** | "teaching_prompts.csv"
  - Contains various teaching prompts (one generalized, 10 harm-specific, and 6 red-teaming technique-specific teaching) aimed at preventing the LLM from generating harmful output. Each teaching prompt serves as an initial primer before introducing a red-teaming trigger prompt. The goal is to evaluate whether the LLM can assimilate knowledge from the initial teaching prompt and thus avoid responding harmfully to the subsequent red teaming prompt.