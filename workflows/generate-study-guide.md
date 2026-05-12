# Workflow: Generate Module Study Guide

## Overview
This workflow automates the creation of a structured study guide and self-assessment quiz for any specific module in the course.

## Trigger
User says: "Generate a study guide for [Module Number/Name]" or uses a slash command (if implemented).

## Step-by-Step Instructions

### Step 1: Research
Identify the correct HTML file in `slides/` corresponding to the requested module. Read the first 200 lines to identify the Module Title and Learning Objectives.

### Step 2: Content Extraction
Search the file for key themes:
*   Identify the **"Problem"** being addressed (e.g., The Cold Start Problem).
*   Identify the **"Solution"** or "Goal" presented in the slides.
*   Extract 3-5 key "Takeaway" points.

### Step 3: Quiz Generation
Generate 3 multiple-choice questions based *strictly* on the content extracted in Step 2.
*   Each question must have 4 options (A, B, C, D).
*   Provide the correct answer in a hidden or bottom section.

### Step 4: Final Output Formatting
Present the study guide using this exact Markdown structure:

# Study Guide: [Module Title]

## 🎯 Core Objective
[Brief summary of what this module teaches]

## 💡 Key Takeaways
* [Takeaway 1]
* [Takeaway 2]
* [Takeaway 3]

## 🧩 The Problem & Solution
* **The Problem:** [Describe the core challenge]
* **The Solution:** [Describe the proposed system/method]

## 📝 Self-Assessment Quiz
[3 Questions here]

---
**Answer Key:** [Answers hidden below]
