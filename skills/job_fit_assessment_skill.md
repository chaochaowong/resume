# Job Fit Assessment Skill

## Purpose

Assess how well a candidate's background aligns with a specific job posting and produce a concise, evidence-based fit assessment similar to a hiring-manager review.

The assessment should answer:
1. What is the role?
2. How well does the candidate align?
3. What are the strongest matches?
4. What are the most important gaps?
5. How should the candidate position their experience?
6. Is the role worth pursuing?

## Inputs

Required:
- Job posting URL or pasted job description
- Candidate resume, CV, or established career profile

Optional:
- Candidate's current goals
- Preferred industry or role direction
- Interview stage
- Location / remote preferences
- Compensation constraints

When a resume is supplied, use it as the primary source for the candidate's experience. Do not invent experience that is not supported by the resume or conversation.

## Workflow

### Step 1: Retrieve and understand the job

If a URL is provided, retrieve the current job description.

Identify:
- Company
- Job title and level
- Core responsibilities
- Required qualifications
- Preferred qualifications
- Domain expertise
- Technical skills
- Leadership / collaboration expectations
- Regulatory or clinical requirements
- Location / work arrangement
- Compensation, if available

Do not infer requirements from the job title alone.

### Step 2: Build the candidate profile

Extract the candidate's strongest relevant experience from the resume and conversation.

Group experience into:
- Scientific/domain expertise
- Bioinformatics/computational methods
- Software and pipeline engineering
- Statistics / machine learning / AI
- Translational or clinical experience
- Leadership / ownership
- Cross-functional collaboration
- Product or production experience
- Regulatory experience

### Step 3: Score alignment

Calculate an estimated alignment score from 0-10 using this weighted rubric:

| Category | Weight |
|---|---:|
| Core scientific/domain match | 20% |
| Required technical skills | 25% |
| Relevant project experience | 20% |
| Execution / software / production capability | 15% |
| Seniority / ownership / collaboration | 10% |
| Preferred qualifications / special requirements | 10% |

Rate each category from 0-10, multiply by its weight, and sum.

Interpretation:
- **9.0-10.0:** Exceptional fit
- **8.0-8.9:** Strong fit
- **7.0-7.9:** Good fit; worth applying
- **6.0-6.9:** Moderate fit; meaningful gaps
- **5.0-5.9:** Stretch role
- **Below 5.0:** Weak alignment unless there is a strategic reason to apply

Always label the score as an **estimated qualification alignment**, not a prediction of hiring success.

### Step 4: Separate direct matches from transferable skills

Use these labels:
- **Direct match:** candidate has clearly done the requested work
- **Transferable:** closely related experience, but not the exact requested application
- **Gap:** important requirement not demonstrated
- **Unknown:** cannot be established from available information

Do not turn transferable experience into direct experience.

Examples:
- Long-read WGS experience can transfer to WES, but is not direct WES experience.
- Research pipeline validation is relevant to clinical pipelines, but does not equal CLIA/CAP experience.
- Using AI tools to assist development does not equal building production agentic AI systems.

### Step 5: Identify the three strongest selling points

Select the candidate's three experiences that best map to the job.

For each, explain:
- What the candidate did
- Which job requirement it maps to
- Why it matters for this role

### Step 6: Identify meaningful gaps

Focus only on gaps that could influence hiring.

For each gap:
- State it directly
- Explain whether it is a major or minor concern
- Explain what transferable experience helps compensate
- Suggest what the candidate should learn or prepare before an interview

Never hide a significant gap just to make the candidate sound stronger.

### Step 7: Recommend positioning

Provide a short positioning statement tailored to the role.

It should connect the candidate's strongest background to the employer's actual needs.

### Step 8: Give a recommendation

Use one of:
- Strongly pursue
- Pursue
- Worth applying, but tailor carefully
- Stretch role
- Low priority

Explain the recommendation in 1-2 paragraphs.

## Output Format

### [Company] — [Job Title]

**Estimated qualification alignment: X/10 — [Exceptional / Strong / Good / Moderate / Stretch]**

One short paragraph summarizing the overall fit.

| Job requirement | Candidate evidence | Alignment |
|---|---|---|
| Requirement 1 | Relevant experience | Strong / Moderate / Gap |
| Requirement 2 | Relevant experience | Strong / Moderate / Gap |
| Requirement 3 | Relevant experience | Strong / Moderate / Gap |

### Strongest alignment

Discuss the 2-3 strongest areas.

### Main gaps

Discuss only the meaningful gaps.

### How I would position you

Provide a 3-5 sentence interview or application positioning statement.

### Recommendation

State whether the user should pursue the role and why.

If useful, finish with one specific interview question or preparation topic that addresses the biggest gap.

## Candidate-specific guidance for CJ Wong

When assessing roles for this candidate, consider these established strengths when relevant:
- 15+ years in bioinformatics and computational biology
- PhD-level quantitative / mathematical background
- Early-career software development and Bioconductor infrastructure experience
- Long-read genomics and PacBio HiFi WGS
- Nextflow / nf-core pipeline engineering
- Major contribution to `nf-core/pacvar`
- SNV/indel, SV, CNV, STR, phasing, methylation, and annotation workflows
- Cancer genomics, especially AML and sarcoma
- Rare disease genomics
- Chromatin biology and epigenomics
- CUT&RUN, CUT&Tag, CUTAC, Fiber-seq
- Transcriptomics, proteomics, drug-screen and multi-omics integration
- Translational research and mechanism-of-action studies
- Biomarker and therapeutic-target discovery
- Cross-functional work with wet-lab scientists
- Open-source collaboration and technical ownership
- Interest in clinical genomics, public-health impact, and product-oriented industry work
- Emerging experience with AI-assisted genomic interpretation

Do not assume the following unless explicitly supported by the resume or current conversation:
- CLIA/CAP laboratory experience
- FDA-regulated software development
- Production clinical pipeline ownership
- Extensive WES-specific experience
- Liquid biopsy / cfDNA expertise
- Production LLM / RAG / agent orchestration expertise
- Direct deployment of AI systems in clinical care

## Style

- Be concise and analytical.
- Avoid generic encouragement.
- Do not inflate the score to be supportive.
- Explain why a role fits or does not fit.
- Distinguish research experience from clinical production experience.
- Distinguish using AI from engineering AI systems.
- Prefer concrete evidence from the job description and resume.
- If the job description is unavailable or incomplete, say so explicitly rather than guessing.
