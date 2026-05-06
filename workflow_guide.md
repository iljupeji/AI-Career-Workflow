# Workflow Implementation Guide

This guide details how to replicate the dual-layer architecture for career data management using engineering principles.

## Step 1: Data Structuring (Base Architecture)

Before uploading to any AI platform, you must organize your professional history into a structured format. Use the following templates provided in the repository:

1. **Header**: Define a single-line contact block.
2. **XYZ Experience Repository**: Format your achievements as: "Accomplished [X] as measured by [Y], by doing [Z]".
3. **Skills Matrix**: Categorize competencies with predefined levels (Skill | Level).
4. **Academic Block**: Standardize education dates, GPA, and relevant keywords.
5. **Complementary Training**: Organize certifications by category with specific syntax rules.
6. **Portfolio Projects**: Structure independent work for quick insertion.

## Step 2: Data Synthesis (NotebookLM)

The objective is to create a "source of truth" by cleaning raw data.

1. Create a new notebook in NotebookLM.
2. Upload your structured data from Step 1, along with technical syllabi and raw project notes.
3. Generate a "Technical Milestone" summary. This synthesis layer reduces noise and ensures every claim is anchored in verifiable facts.

## Step 3: Strategic Execution (Claude)

The objective is to adapt the synthesized data to a specific job requirement.

1. Create a new Project in Claude.
2. Upload the summary generated in Step 2.
3. Provide the target Job Description.
4. Apply the logic from `agent_instructions.md`. Claude will identify gaps, calculate affinity, and optimize keywords based on the structured XYZ data.

## Step 4: Human-in-the-Loop Audit

Implementation is only half of the work. The final layer is a mandatory manual review.

1. Cross-reference the final CV against your NotebookLM source truth.
2. Verify that technical nuances and XYZ metrics are 100 percent accurate.
3. Finalize formatting (0.49 cm margins, single-page limit) before submission.

---
*Note: This workflow transforms a 5-hour manual process into a 20-minute high-precision system.*
