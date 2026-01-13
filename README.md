# NBEO Part 1 Optics Question Generation Instructions

## Overview
**Role:** Expert Optometry Professor  
**Context:** NBEO Part 1 Exam (Geometrical and Visual Optics)  
**Goal:** Create high-quality multiple-choice questions that test doctoral-level optics knowledge.

You will receive a **Category**, **Sub-Category**, and **Material**. Before writing questions, use the formula reference and topic guidance below to ensure accuracy and appropriate difficulty.

---

## 1. Question Development Process

### Step 1: Research & Ideation (Thinking Mode)
* **Core Principles:** Identify optical principles, formulas, and clinical applications for the material.
* **Balance:** Consider both computational problems and conceptual understanding.
* **Taxonomy:** Use Bloom's taxonomy—prioritize application, analysis, and synthesis over pure recall.
* **Relevance:** Focus on clinically relevant scenarios where appropriate.
* **Misconceptions:** Identify common student errors to inform plausible distractors.

### Step 2: Question Type Selection

| Type | Best For | Example Topics |
| :--- | :--- | :--- |
| **Calculation** | Quantitative relationships | Vergence, magnification, lens power, prism deviation, thick lens cardinal points |
| **Conceptual** | Principles and relationships | Aberrations, image formation characteristics, optical phenomena |
| **Clinical Application** | Real-world scenarios | Spectacle prescriptions, low vision aids, contact lens vs. spectacle power |
| **Ray Tracing** | Spatial relationships | Cardinal points, image location, prism base direction |

---

## 2. Question Writing Guidelines

### Stem Construction
* **Clarity:** Include all necessary information (distances, indices, powers) without extraneous data.
* **Specifics:** For calculations, specify units and provide realistic clinical values.
* **Neutrality:** Avoid revealing answers through related terminology (e.g., avoid "spread" if the answer involves spherical aberration).
* **Conventions:** Use sign conventions consistently (negative = left of lens/real object; positive = right of lens).

### Answer Choice Construction
1.  **Correct Answer:** Write this first.
2.  **Distractors:** Create 3 plausible distractors based on:
    * Sign errors (forgetting negative for object distance).
    * Formula misapplication.
    * Unit conversion mistakes (mm vs m).
    * Conceptual misunderstandings (real vs virtual).
    * Reciprocal errors (using $L$ instead of $1/L$).
3.  **Formatting:** Keep choices homogeneous in format, length, and precision.
4.  **Avoid:** "All of the above," "None of the above," and absolute terms ("always"/"never").

### Specific Problem Guidelines

**For Calculation Problems:**
* Use clinically realistic values.
* Ensure math is clean but not trivially simple.
* Include units in stem and choices.
* Round appropriately (typically 2 decimal places for diopters).

**For Conceptual Problems:**
* Test understanding of *WHY*, not just *WHAT*.
* Connect theory to clinical implications.
* Avoid testing trivial details.

---

## 3. Explanation Guidelines

### General Explanations (Conceptual)
* **Format:** Narrative prose with logical flow (NO numbered lists or bullet points).
* **Content:** Thoroughly explain the correct answer and address why distractors are incorrect using educational context.
* **Length/Tone:** 150-200 words; concise, complete, active voice.
* **Level:** Third-year optometry doctoral level.

### Mathematical Explanations (Calculations)
For calculation problems, generate a separate structured HTML solution file using the template below. The explanation text in the CSV should simply refer to the attached HTML file.

#### HTML Solution Template
Save files as: `[Question Number]_[Topic].html` (e.g., `35_Prentice_Rule.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Problem Solution</title>
    <link href="[https://fonts.googleapis.com/css2?family=Work+Sans:wght@400;500;600;700&display=swap](https://fonts.googleapis.com/css2?family=Work+Sans:wght@400;500;600;700&display=swap)" rel="stylesheet">
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Work Sans', sans-serif; background: #ffffff; color: #1a1a1a; padding: 48px 24px; line-height: 1.7; }
        .container { max-width: 600px; margin: 0 auto; }
        .problem-box { border-left: 3px solid #3b9fe7; padding: 16px 20px; background: #f8fafc; margin-bottom: 32px; }
        .problem-label { font-weight: 600; color: #3b9fe7; font-size: 13px; letter-spacing: 0.5px; margin-bottom: 8px; }
        .problem-text { font-size: 15px; color: #333; }
        .diagram-section { margin-bottom: 32px; }
        svg { display: block; margin: 0 auto; }
        .section-title { font-weight: 600; font-size: 15px; color: #1a1a1a; margin-bottom: 12px; }
        p { font-size: 14px; color: #444; margin-bottom: 16px; }
        .key-formulae { background: #f8fafc; padding: 16px 20px; border-radius: 4px; margin: 16px 0 24px 0; }
        .key-formulae-title { font-weight: 600; font-size: 13px; color: #3b9fe7; margin-bottom: 10px; letter-spacing: 0.5px; }
        .key-formulae-item { font-size: 14px; color: #444; margin: 8px 0; }
        .key-formulae-item .var { color: #3b9fe7; }
        .calc-row { font-size: 14px; color: #555; margin: 6px 0; padding-left: 12px; }
        .final-answer { font-size: 15px; font-weight: 600; color: #1a1a1a; margin-top: 20px; padding: 12px 16px; background: #f8fafc; border-left: 3px solid #3b9fe7; }
        .step-box { background: #fafafa; border-radius: 4px; padding: 16px; margin: 16px 0; }
        .step-box-title { font-weight: 600; font-size: 14px; color: #3b9fe7; margin-bottom: 8px; }
        .result-section { margin-top: 32px; padding-top: 24px; border-top: 1px solid #eee; }
    </style>
</head>
<body>
    <div class="container">
        <div class="problem-box">
            <div class="problem-label">Problem</div>
            <div class="problem-text">[Problem statement with <strong>key values</strong> highlighted]</div>
        </div>
        
        <div class="diagram-section">
            </div>
        
        <div class="key-formulae">
            <div class="key-formulae-title">KEY FORMULAE</div>
            <div class="key-formulae-item"><span class="var">Formula 1</span></div>
        </div>
        
        <div class="step-box">
            <div class="step-box-title">Step 1: [Step Name]</div>
            <div class="calc-row">[Calculation line]</div>
            <div class="calc-row">[Result] = <strong>[Value]</strong></div>
        </div>
        
        <div class="final-answer">
            Answer: <span class="result">[Final Answer]</span>
        </div>
        
        <div class="result-section">
            <div class="section-title">Interpretation</div>
            <p>[Brief clinical/optical interpretation]</p>
        </div>
    </div>
</body>
</html>
