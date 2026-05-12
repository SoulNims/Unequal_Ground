# CLAUDE.md

Context file for my HIST 160 unessay project. Use this to understand the course, the assignment, and what I am trying to build.

## Who I am

Nima, undergraduate student at Knox College. I am working on the final unessay project for HIST 160.

## The Course

**HIST 160: Power and Inequity in America to 1865**
- Instructor: Cate Denial (cdenial@knox.edu, also referenced as njsherpa@knox.edu for reflections)
- Term: Spring 2026
- Focus: early American history through primary sources, with attention to who held power, who was excluded, and how systems of inequality were built and justified.

### Course themes
The course centers on the question of what power means in U.S. history, what it means to be just and free, and who got (and gets) to decide. It pushes back on the simplified K through 12 narrative that often erases Indigenous people, Black people, Latinx people, Asian people, people with disabilities, and women, trans, and non binary individuals.

### Learning goals
1. Explain the significance of individual and structural histories to a chosen audience.
2. Synthesize and interpret historical structures of the place we now call the U.S. for peers (this is the unessay).
3. Analyze primary sources.
4. Reflect on the learning process.

### Assignments in the course
1. Letter to Someone (done, due April 27)
2. **Unessay project (due Thursday, May 21)** — what this file is about
3. Final reflection (during finals)

## The Unessay Assignment

From the syllabus, verbatim spirit:

> Toward the end of term you will choose any subject related to the early history of North America and/or the United States and create something of your choosing that communicates what you know about the subject. You might make a zine, create art, cook food, make a film, draw a map. The possibilities are endless.

So: open ended creative or scholarly project demonstrating what I have learned. No essay format required. The point is to *communicate knowledge* in a form I choose.

## My Proposal (already submitted)

**Topic:** Power and inequity in early America, explored through technology, data visualization, and historical mapping.

**Core tension I want to surface:** the contradictions between the ideals of freedom and equality in early American political thought and the realities lived by Indigenous peoples and enslaved Africans.

**Subtopics I want to cover:**
- Settler colonialism
- Slavery
- Epidemic disease after European contact
- Unequal systems of political and economic power (land, labor, political rights)

**Form:** a digital visualization project or dashboard. Interactive maps, timelines, and graphs. Almost an interactive historical exhibit.

**Tools I plan to use:** Python (likely pandas, matplotlib/plotly, possibly folium or kepler.gl for maps, maybe streamlit or a static site for the dashboard shell).

**Why this form:** I am interested in data science and visualization. Historical systems can be clearer visually than in prose. I want patterns of inequality, land ownership, disease spread, labor, and political rights to be *seen*, not just described.

**Supplies:** all digital, no physical materials needed.

## Key Readings That Inform the Project

These are the assigned course readings I have explicitly tied to the project. Anything outside this list is outside exploration, not the assigned curriculum, and should be flagged as such.

1. **Nahuatl Census from the Cuernavaca Region, c. 1540** (trans. Lisa Sousa). Calpulli structure, tribute system, household composition, baptized vs unbaptized residents, irrigated vs hill maize fields measured in brazas, the obligations owed to Martín Molotecatl teuctli. Great source for visualizing colonial labor and tribute extraction at household scale.

2. **Book XII of the Florentine Codex** (Sahagún, compiled 1540 to 1570, trans. James Lockhart). Nahuatl account of the smallpox epidemic of the 1520s, the "great rash," that swept through Mexico before and during Spanish military campaigns. Useful for the epidemic disease piece.

3. **John Locke, Second Treatise of Government** (Week 6). Equality, the state of nature, civil society, consent, the limits of legitimate political power. The ideological side of the contradiction I am tracking.

4. **Other course readings already covered:** Powhatan/Jamestown primary sources, Mary Rowlandson's captivity narrative with Carla Cevasco's secondary analysis, the South Carolina Slave Code of 1740, Adams correspondence, the Mum Bett / Elizabeth Freeman freedom suit, Frederick Douglass's Fourth of July speech.

5. **Settler Colonialism Primer (Unsettling America)** — framing reading from early in the term. Useful conceptual scaffolding.

6. **"Ultra Processed Minds" by Carl Hendrick** — Week 2 reading on deep reading vs scanning. Not directly about colonial history but part of the course's framing about how we engage with sources.

## SOCC Method (how this course reads primary sources)

When I analyze a primary source in the project, the course framework is:
- **Source:** when, who, what kind of document, audience, significance
- **Observe:** summarize, identify supporting text, what it tells us about the time
- **Contextualize:** connect to broader era
- **Corroborate:** what questions remain, what evidence would answer them

If I am writing captions, labels, or interpretive text in the dashboard, this framework is the spine.

## How I Want Claude to Help

### My working style
- I read primary sources closely and catch inaccuracies. Ground claims in the actual text. If you are unsure, say so rather than guessing.
- Distinguish between assigned course readings and outside material (Wikipedia, web research, etc.). Preserve that distinction.
- Casual, natural, first person student voice. Not formal academic prose unless I ask.
- Concise. No over explanation, no repeating content across sections.
- Specific textual references when relevant, but they should feel natural.
- Do not use em dashes in writing for me.

### What I want help with on the unessay
- Brainstorming what to visualize and what data sources to pull from (historical demographic data, Trans Atlantic Slave Trade Database, colonial census data, land records, disease mortality estimates, etc.)
- Python code for data cleaning, mapping, and dashboard building
- Designing how the visualizations connect to the primary sources I have read
- Writing short interpretive captions or exhibit text in my voice
- Honest feedback on whether a chart or map actually communicates the historical point or just looks cool
- Catching when I am drifting outside what the course actually covered

### What I do not want
- Generic AI sounding prose
- Big walls of caveats
- Padding or restating the prompt back at me
- Treating this like a normal essay when it is explicitly not one

## Deadline

Thursday, May 21 (due in class).

## Technical Notes (what has been built)

**File:** `index.html` — single static file, open in any browser, no server needed.

**Libraries:** Plotly.js 2.26.0 (CDN). No other dependencies. No Python runtime required to view.

**Charts included:**
1. Bar chart — 1790 U.S. population by legal/political status (Census data)
2. Scattergeo map — epidemic contact points across North America and Mesoamerica (Florentine Codex anchor + outside sources)
3. Line chart — enslaved population 1650–1860, estimated then Census-sourced, annotated at key legislative moments
4. Scattergeo map — key colonial, Indigenous, slavery, and resistance sites (course readings + outside sources)

**Source tagging:** every chart caption marks content as `[Course Reading]` or `[Outside]`. Primary source quotes are cited; paraphrases are marked as paraphrases.

**Sections:** Hero, The Promise (Locke), Epidemic (Florentine Codex), Enslaved (SC Slave Code), The Land (Nahuatl Census), Resistance (Freeman / Douglass), Sources.

**To open:** double-click `index.html` or drag it into a browser window. Works offline once the Plotly CDN loads once.
