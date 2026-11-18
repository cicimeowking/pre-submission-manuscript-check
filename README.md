
# Pre-submission Manuscript Check

**An AI-assisted Skill for checking research manuscripts before journal submission.**

Pre-submission Manuscript Check helps researchers identify common problems in their manuscripts before submission, including internal inconsistencies, author and contribution mismatches, missing declarations, ethics and consent issues, figure and table inconsistencies, reference mismatches, citation appropriateness, and writing conventions.

The Skill is designed to help authors identify potential problems before submitting their manuscripts, regardless of the target journal.

## Key Features

- **Journal-independent** — Does not impose a specific journal's template, reference style, or formatting requirements.
- **Two-track workflow** — Distinguishes medical/life-science manuscripts from non-medical manuscripts and applies the appropriate checks.
- **General manuscript checks** — Covers authorship, internal consistency, declarations, figures, tables, references, and writing conventions.
- **Medical-specific checks** — Examines ethics, informed consent, registration timelines, reporting-guideline items, and biological materials when applicable.
- **Citation appropriateness review** — Helps authors assess whether cited references are relevant to the statements they support.
- **Evidence-based reporting** — Identifies observed inconsistencies and potential issues without inventing information or making unsupported assumptions.

## What Does This Skill Check?

### 1. General Checks

Applied to all manuscripts.

| Category | Checks |
|---|---|
| Authors & Contributions | Author list, Author Contributions, corresponding authors, and affiliations |
| Internal Consistency | Numbers, sample sizes, groups, terminology, statistics, figures, tables, and conclusions |
| Declarations | Author contributions, conflicts of interest (COI), funding, data availability, and generative AI disclosure |
| Figures & Tables | Numbering, in-text callouts, captions, labels, units, and consistency with the main text |
| References | Matching in-text citations with reference-list entries; identifying missing, duplicated, or apparently uncited references |
| Writing Conventions | Italics, biological names, gene/protein symbols, statistical symbols, superscripts/subscripts, and special characters |

### 2. Medical and Life-Science Checks

Applied only when relevant to the manuscript.

- Ethics approval
- Informed consent
- Consent for publication
- Clinical trial and systematic review registration
- Registration timelines
- Clinical-data consistency
- Reporting-guideline items
- Animal ethics and welfare
- Cell-line source and authentication
- Human biological samples
- Public database accession numbers

The Skill first classifies the manuscript and then determines which additional checks are applicable. Medical ethics and registration requirements are not automatically imposed on non-medical manuscripts.

## How It Works

```text
             Manuscript
                 |
                 v
        Classify Manuscript
                 |
                 v
       General Manuscript Check
                 |
                 v
     Medical/Life-Science Check
          (if applicable)
                 |
                 v
      Figures, Tables & References
                 |
                 v
     Citation Appropriateness Review
                 |
                 v
          Generate Reports
```

### Core Principle

**Classify first. Check only what applies. Report differences, not guesses.**

The workflow is designed to identify potential issues while avoiding irrelevant requirements and unsupported conclusions.

## Installation and Use

This repository contains the complete Skill package, including:

- `SKILL.md` — Main Skill instructions and checking workflow.
- `scripts/` — Python scripts for document processing, manuscript checking, and report generation.
- `references/` — Supporting reference materials and checking criteria.
- `guidelines/` — Relevant reporting-guideline resources.

### How to Use

1. Download or clone this repository.
2. Install or copy the Skill package into the appropriate Skill directory of a compatible AI assistant or agent environment.
3. Make sure the supporting folders (`scripts/`, `references/`, and `guidelines/`) retain their original relative paths.
4. Provide your manuscript to the AI assistant.
5. Request a **pre-submission manuscript check**.
6. Review the generated reports and verify the flagged issues against the original manuscript.

The exact installation procedure depends on the AI assistant or agent environment being used. Please refer to the documentation of your chosen environment for its Skill installation requirements.

**Note:** The current workflow is designed primarily for Word (`.docx`) manuscripts. Support for other file formats depends on the capabilities of the relevant scripts and AI environment.

## Output

A complete check is designed to produce two complementary reports.

### 1. Manuscript Self-Check Report

A structured report covering:

- Manuscript classification and applicable checking workflow
- Author list and contribution consistency
- Internal consistency across the manuscript
- Declaration completeness
- Medical-specific checks, when applicable
- Figure and table consistency
- Writing conventions and typography
- Citation-related findings
- Potential issues and suggested actions

### 2. Citation Appropriateness Assessment

A separate Excel spreadsheet containing citation-level assessments and supporting explanations.

This report helps authors review whether their cited references are appropriate for the statements they are intended to support.

**Current output:** The manuscript self-check report is generated in Chinese, while the citation assessment is provided in Excel.

## What This Skill Does NOT Do

This Skill is designed for content-oriented pre-submission checking. It does not:

- Enforce a specific journal's formatting requirements or reference style.
- Determine whether a manuscript is scientifically novel or valid.
- Replace editorial assessment or peer review.
- Verify the real-world identities or affiliations of authors.
- Determine whether an individual qualifies for authorship.
- Guarantee compliance with a particular journal's submission requirements.
- Guarantee successful editorial screening or manuscript acceptance.

If you want to check a manuscript against a specific journal's requirements, provide the journal's current **Instructions for Authors** separately. These requirements can be used as additional checking parameters.

## Privacy and Responsible Use

Manuscripts may contain unpublished research, confidential information, or sensitive personal data.

Please review the privacy and data-handling policies of the AI platform you use before uploading a manuscript.

- The supporting Python scripts are designed for local document processing. However, this does not guarantee that the AI assistant or agent environment processes uploaded manuscripts locally.
- Avoid including unnecessary patient identifiers, contact details, or other sensitive personal information.
- Ensure that your use of the Skill complies with applicable research ethics requirements, institutional policies, and confidentiality obligations.

Authors are responsible for protecting unpublished research and personal information when using AI-assisted tools.

## Limitations

This is an AI-assisted pre-submission checking tool, not a substitute for author review, editorial assessment, or peer review.

Please keep the following limitations in mind:

- Manuscript classification may be uncertain for interdisciplinary research.
- Automated document extraction may not capture all content in complex Word layouts.
- AI-assisted checks may produce false positives or overlook certain issues.
- Typography and biological-name checks may require manual verification.
- Citation relevance assessments depend on the information available about the cited references.
- The absence of a flagged issue does not guarantee that the manuscript is free of errors.

Authors should verify all findings against the original manuscript before submission.

## Repository Structure

```text
pre-submission-manuscript-check/
│
├── README.md
├── SKILL.md
│
├── scripts/
│   ├── qc_extract.py
│   ├── qc_typography.py
│   └── ...
│
├── references/
│   └── ...
│
└── guidelines/
    └── ...
```

The directory structure above illustrates the main components of the Skill package. Please refer to the repository for the complete list of included resources.

## Version

**Current Version: v2.2**

---

**Pre-submission Manuscript Check**

*Helping researchers identify potential manuscript issues before submission.*
