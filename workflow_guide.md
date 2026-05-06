# Workflow Implementation Guide

This guide details how to replicate the dual-layer architecture for career data management.

## Step 1: Data Synthesis (NotebookLM)
- Create a notebook and upload your source truth: technical syllabi, raw project logs, and CV history.
- Generate a "Technical Milestone" summary. This cleaning layer reduces noise and ensures a verified foundation.

## Step 2: Strategic Execution (Claude)
- Upload the synthesized summary to a Claude Project.
- Provide the target Job Description.
- Apply the rules from `agent_instructions.md`.
- Use Claude's reasoning to map verified data to the vacancy requirements.

## Step 3: Human Audit
- Manually audit every output. Despite AI efficiency, this step ensures 100% accuracy and professional integrity.
- Verify that technical nuances and keywords reflect actual experience.
