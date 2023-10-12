# Red teaming prompts for LLMs

⚠️ **WARNING: Sensitive Content** ⚠️

This repository contains prompts that may include content related to hate speech, racism, and other harmful themes. This material is **strictly for research purposes** to evaluate the guardrails of LLMs. It is not intended to harm, offend, or promote harmful behavior. Please use this material with caution and be aware of its potentially offensive nature.

## Overview

This repository contains three datasets of prompts created for a research study aimed at assessing the guardrails of LLMs, with the Vicuna 13B model serving as an example.

- **Dataset 1: Initial Assessment** | "initial_assessment_prompts.csv"
  - Comprises 100 red-teaming prompts across 10 harm categories to assess the default guardrails of the LLM, without using any red-teaming technique or deceptive tactics.

- **Dataset 2: Red-Teaming Prompts** | "red-teaming-prompts"
  - "red_teaming_prompts.csv": Features 180 prompts that successfully provoked harmful responses when tested with the Vicuna-13B LLM. These prompts are model-specific and might not yield the same results when tested with other LLMs.
  - "conversations": Provides records of the full conversations in .yaml and .md files for each red-teaming technique.

- **Dataset 3: Teaching Prompts** | "teaching_prompts.csv"
  - Contains various teaching prompts (one generalized, 10 harm-specific, and 6 red-teaming technique-specific teaching) aimed at preventing the LLM from generating harmful output. Each teaching prompt serves as an initial primer at the beginning of a conversation, before the model is triggered by a red-teaming prompt. The goal is to evaluate whether the LLM can assimilate knowledge from the initial teaching prompt and thus avoid responding harmfully to the subsequent red teaming prompt.