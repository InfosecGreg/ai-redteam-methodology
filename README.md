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

### Usage (Slash Commands)

The most efficient way to generate content is using the following agent workflows.

#### To Generate a Main Article:

Use the `/generate-article` command followed by the section reference.

> `/generate-article 1.2.1`

This will automatically read the requirements and create the article in the `techniques/` folder.

#### To Generate an Example Explanation:

Use the `/generate-example` command followed by the example reference ID.

> `/generate-example 1.2.1.E1`

This will create a detailed deep-dive for that specific example in the `techniques/examples/` folder.

### Manual Usage

If you prefer to trigger generation manually, use the following prompt structures.

#### To Generate a Main Article:

Use the following prompt structure, replacing `X.Y.Z` with the desired section number from `methodology.md`.

> "Using `article_generation_prompt.md`, write the article for section `X.Y.Z` from `methodology.md`."

#### To Generate an Example Explanation:

Use the following prompt structure, replacing `X.Y.Z.E1` with the desired example ID.

> "Using `example_explanation_prompt.md`, write the sub-article for example `X.Y.Z.E1`."

## Contributing

Contributions to the methodology and the generation prompts are welcome. Please feel free to suggest improvements by opening an issue or a merge request.
