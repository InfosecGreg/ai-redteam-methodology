# AI Red Team Methodology

## Overview

This repository contains the framework for a comprehensive, phased AI Red Teaming methodology. The core of this project is the `methodology.md` file, which outlines a structured approach to testing and evaluating the security, safety, and ethical boundaries of AI systems, particularly Large Language Models (LLMs).

The goal is to create a living document and a series of detailed articles that can be used by security professionals, AI developers, and researchers to conduct effective AI red teaming engagements.

## The Methodology

The official methodology is maintained in the following file:

- **[/methodology.md](./methodology.md)**

This document outlines the six phases of an engagement, from initial reconnaissance to final reporting.

## Article Generation

This project uses a generative AI (you!) to create detailed articles for each point in the methodology. Two instruction files govern this process:

- `article_generation_prompt.md`: A template for creating a full article for a methodology point.
- `example_explanation_prompt.md`: A template for creating a detailed sub-article for a specific example within an article.

### Usage

To generate content, use the following instructions in your prompts.

#### To Generate a Main Article:

Use the following prompt structure, replacing `X.Y.Z` with the desired section number from `methodology.md`.

> "Using `article_generation_prompt.md`, write the article for section `X.Y.Z` from `methodology.md`."

**Example:**
> "Using `article_generation_prompt.md`, write the article for section `3.1.1` from `methodology.md`."

#### To Generate an Example Explanation:

After an article is generated, its examples will have reference IDs (e.g., `3.1.1.E1`). To create a detailed sub-article for a specific example, use the following prompt structure.

> "Using `example_explanation_prompt.md`, write the sub-article for example `X.Y.Z.E1`."

**Example:**
> "Using `example_explanation_prompt.md`, write the sub-article for example `3.1.1.E1`."

## Contributing

Contributions to the methodology and the generation prompts are welcome. Please feel free to suggest improvements by opening an issue or a merge request.
