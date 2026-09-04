## Goal
Update the profile website (`index.html`) with updated **About** and **Background** section content provided by the user.

## Assumptions
1. Target website file is located at `c:\Users\cyber\Downloads\website\adamsayyed.github.io\index.html`.
2. Existing section IDs `#about` and `#background` in `index.html` should retain their structural wrapper elements (`<section>`, `<h2>`) while replacing paragraph contents.
3. Content should be properly formatted into semantic HTML `<p>` tags matching the user's structured paragraphs.

## Plan

### Step 1: Update the About Section
- **Files**: `adamsayyed.github.io/index.html`
- **Change**: Update `<section id="about" class="content-section">` with the 2 new paragraphs:
  1. Senior student status, B.S. in CS (ML/AI focus) at UMBC, Meyerhoff Scholar, AI & Software Engineer focused on end-to-end intelligent systems.
  2. Intersection of software engineering, ML, data-intensive systems, internal APIs, ML pipelines, LLMs, and HPC workloads.
- **Verify**: Perform a view/grep on `index.html` around line 83 to ensure correct HTML structure and updated text.

### Step 2: Update the Background Section
- **Files**: `adamsayyed.github.io/index.html`
- **Change**: Update `<section id="background" class="content-section">` with the 6 new paragraphs covering:
  1. Overall summary as senior CS student with internships/research at JHU APL, Sandia, UMBC.
  2. JHU APL Software Engineering Intern experience (FastAPI service, 65% reduction in manual data prep, passive radar pipelines speedup/failure reduction).
  3. Sandia National Laboratories experience (geospatial ML, error-analysis pipelines, MCP LLM integration).
  4. UMBC multimodal machine learning research for financial forecasting (time-series + FinBERT/RoBERTa embeddings).
  5. University of Iowa research (seq2seq Transformers) and foundational software dev experience.
  6. Core interest summary (AI engineering, ML systems, AI infrastructure, HPC, scalable deployment).
- **Verify**: Perform a view/grep on `index.html` around line 101 to verify text and formatting.

### Step 3: Validate Layout and HTML Markup
- **Files**: `adamsayyed.github.io/index.html`
- **Change**: Verify clean HTML structure and section tags.
- **Verify**: Check file content and tag balance across `#about` and `#background` sections.

## Risks & mitigations
- **Risk**: Loss of styling or breaking section tags during edit.
- **Mitigation**: Retain existing `<section>` and `<h2>` elements, updating only inner `<p>` nodes.

## Rollback plan
Run `git checkout -- index.html` inside `c:\Users\cyber\Downloads\website\adamsayyed.github.io` to restore original file.
