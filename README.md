Pre-submission Manuscript Check
An AI-assisted Skill for checking research manuscripts before journal submission.

This Skill helps researchers identify common problems in their manuscripts before submission, including internal inconsistencies, author and contribution mismatches, declarations, ethics and consent issues, figure and table cross-checks, reference consistency, citation appropriateness, and writing conventions.

Key features
- Journal-independent — does not impose a specific journal's template or formatting style.
- Two-track workflow — automatically distinguishes medical/life-science manuscripts from non-medical manuscripts.
- General manuscript checks — authorship, consistency, declarations, figures, tables, references, and writing conventions.
- Medical-specific checks — ethics, informed consent, registration timelines, reporting-guideline items, and biological materials when applicable.
- Citation appropriateness review — helps authors examine whether references are appropriate for the statements they support.
- Evidence-based reporting — reports observed differences and potential issues without inventing information.
  
What does this Skill check?
General checks
Category	Checks
Authors & contributions	Author list, Author Contributions, corresponding authors, affiliations
Internal consistency	Numbers, groups, terminology, statistics, figures, tables, conclusions
Declarations	Contributions, COI, funding, data availability, AI disclosure
Figures & tables	Numbering, callouts, captions, labels, units and consistency
References	In-text citations ↔ reference list
Writing conventions	Italics, gene symbols, statistical symbols, superscripts/subscripts, special characters


Medical/life-science checks
Applied only when relevant:
- Ethics approval
- Informed consent
- Consent for publication
- Trial/review registration
- Registration timeline
- Clinical-data consistency
- Reporting-guideline items
- Animal ethics
- Cell-line authentication
- Human biological samples
- Public database accession numbers
  
How it works
Manuscript
    ↓
Classify manuscript
    ↓
General manuscript check
    ↓
Medical/life-science check
    │   (if applicable)
    ↓
Figures / Tables / References
    ↓
Citation appropriateness review
    ↓
Self-check reports

Core principle
Classify first. Check only what applies. Report differences, not guesses.

The Skill does not automatically apply medical ethics or registration requirements to non-medical manuscripts.
Installation / Use
This repository contains the complete Skill package, including the Skill instructions, scripts, references, and reporting-guideline resources.

The main Skill definition is:
SKILL.md

Supporting resources are located in:
scripts/
references/
guidelines/

Use the repository according to the Skill/AI-agent environment you are working with.
For compatible Skill environments, install or copy the Skill package into the environment's Skill directory and invoke it when performing a pre-submission manuscript check.
Then provide the manuscript and ask the AI assistant to perform a pre-submission manuscript check.

What this Skill does NOT do
This Skill does not:
- enforce a specific journal's formatting requirements;
- decide whether a manuscript is scientifically novel or valid;
- replace peer review;
- verify author identities or affiliations;
- determine whether an author qualifies for authorship;
- guarantee compliance with a particular journal;
- guarantee acceptance or successful editorial screening.
  
If you want to check a specific journal's requirements, provide its current Author Guidelines separately. The Skill can use user-provided journal requirements as additional parameters.
Output

A complete check is designed to produce:

1. Manuscript self-check report
A structured report covering:
- manuscript classification;
- author and contribution consistency;
- internal consistency;
- declarations;
- medical-specific checks when applicable;
- figures and tables;
- writing conventions;
- citation-related findings;
- limitations.
  
2. Citation appropriateness assessment
A separate spreadsheet containing citation-level assessment and supporting rationale.
Privacy
Manuscripts may contain unpublished research, confidential information, or personal data.

Please review the privacy and data-handling policies of the AI platform you use before uploading a manuscript.

The supporting scripts are designed for local document processing, but this does not mean that every AI environment using the Skill processes uploaded manuscripts locally.

Do not include unnecessary patient identifiers, contact information, or other sensitive personal information.
Limitations
This is an AI-assisted pre-submission checking tool, not a substitute for author review, editorial assessment, or peer review.

Automated checks may produce false positives or miss problems. Authors should verify all flagged issues against the original manuscript before submission.
Repository structure.

├── README.md
├── SKILL.md
├── scripts/
├── references/
└── guidelines/

Version
Current version: v2.2
