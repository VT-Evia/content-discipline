# Content Creation (and Management) Activities

Activities in this stage focus on content creation and not necessarily the production of user-facing deliverables. Topic-based content creation is built on a foundation of separating content from presentation, and in some cases the presentation is not in the hands of a content author. 

## Creating a Structured Website

Following the **Creating a Content Model** activity from [Stage 2](../stage2/contentstrategyactivities.md), students can create an HTML-based project to be managed in a GitHub repository and hosted as a website on GitHub Pages. The goal of this activity is not to create the kinds of reusable topics (content chunks) required in structured authoring workflows but rather to gain familiarity with applying a content model to content creation, using a code editor, and assembling a website.

A consistent format for every entry/page in this website activity is key to maintaining the content model. This is not an assignment for individual formatting across pages or entries. For topics, students can continue with the project that they started in Stage 2 (using this activity as an opportunity to create content in accordance with their content model), or they can select a topic that interests them. We have used topics ranging from the top 10 songs on the hit parade, to a collection of favorite books or movies, to a catalog of the courses a student is taking in a given term. 

Audience considerations will drive the content, so it is important to specify who the intended reader of the website deliverable is. If students are building on the activities that they completed in Stage 2 when developing a content strategy plan, their audience should already be well defined. If students are selecting topics of interest to them, they might build their website for family members and friends.

The project includes three main tasks: planning the content model, creating content, and assembling the website.

### Planning the Content Model

Each page on the planned website must follow the same structure and contain one topic. For example, a website with the top 10 songs of the summer might be based on a content model like the following:

- Song title  
- Performer  
- Single cover image  
- Personal review  
- Rating on a scale of 1 to 5 stars  

When we practice this activity, we allow students to use generative AI tools to generate the skeleton HTML, CSS, and JS files for the project, but their prompts must not ask for sample content. Students' prompts must emphasize functionality and user experience. We recommend having students use [Visual Studio Code](https://code.visualstudio.com/) to develop the code structure for their website pages. Most LLM chat agents can generate the HTML code for the pages following the content model that students will need to describe in a prompt. Visual Studio Code also integrates with GitHub, allowing students to push their HTML, CSS, and JS files to their GitHub repository. There is both a desktop and browser-based version of Visual Studio Code. We recommend using the [github.dev web-based editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor), which provides many of the benefits of Visual Studio Code without additional downloads.

#### Sample Prompt

> You are a coding assistant. Create a small, static website scaffold (HTML/CSS/JS) suitable for hosting on GitHub Pages. The site will implement a single, consistent content model for multiple entries/pages. Do not generate any sample content, filler text, or “lorem ipsum.” Use clearly marked placeholders and empty elements where students will author their own content.

> ##### Audience

> Primary audience: Classmates, friends/family.
>> The design should prioritize readability, simple navigation, and accessibility for this audience.

> Topic & Content Model
>> Topic domain: "Top 10 songs of the summer,” “My current semester courses,” “Favorite books,” etc.
>> Each page shows one entry that follows this exact content model (keep labels visible in the code as data-field attributes and comments):
```
title (short title for the entry)
creator (e.g., performer/author/instructor)
image (single representative image)
description (student-authored review/summary/notes)
rating (1–5 stars)
```
> Ensure the HTML includes empty elements / placeholders for each field. Students will author content later—do not include any example values.

> ####Technical Requirements
>> Files & Structure
```
/ (project root)
├─ index.html                    # Lists all entries with consistent cards (no sample data)
├─ entry.html                    # Template page showing one entry/topic (no sample data)
├─ assets/
│  ├─ css/
│  │  └─ styles.css
│  ├─ js/
│  │  └─ main.js
│  └─ images/                    # empty folder; do not add images
└─ README.md                     # brief usage notes for students (no content examples)

>> HTML & Accessibility
>>>- Use semantic HTML5 with header, nav, main, footer.
- Include a skip-to-content link and sensible heading hierarchy.
- Provide an accessible nav with links to Home (index.html) and a generic All Entries anchor.
- Image wrapper with empty src and placeholder alt that says: <!-- STUDENT: write meaningful alt text -->
- Do not include any example text; instead, include comments like <!-- STUDENT: write your own [field] here -->.

>>CSS
>>>- Create a clean, responsive layout using CSS Grid/Flexbox.
- No frameworks. Keep the palette neutral and minimal.
Include a prominent comment block at the top of index.html and entry.html:
<!--
  CONTENT POLICY FOR THIS ASSIGNMENT:
  - Students must author all entry content themselves.
  - Do NOT paste or generate content from AI systems.
  - This scaffold provides structure only (HTML/CSS/JS).
  - Replace placeholders with your own writing and media.
-->
Quality & Consistency Guards
Ensure the same field order and labels appear across index.html cards and entry.html detail view.
Provide a small “Model Inspector” section (collapsed <details> in the footer) that shows the current schema.json keys (fetched and listed). No sample data.
Output Format
Provide all files in one response, each preceded by a clear filename line like:
--- index.html ---
[file contents]
--- assets/css/styles.css ---
[file contents]
...
Keep comments concise and instructional. No example content values anywhere.
Do not include images or external libraries. Everything must be self-contained.
Generate the code now.

### Creating Content

Once the students have the code structure for each entry in their project, they need to conduct research for the actual content. Then, they will use the HTML template files to create consistent entries with effective content that satisfies their users' information needs.

### Assembling the website

Students should use GitHub (we recommend using the github.dev editor inside GitHub) to customize their websites by creating a GitHub repository named in a way relevant to their site’s topic. The [resources](resources.md) page for this stage includes tutorials for GitHub and GitHub Pages that will be essential for this assignment.

---

## Creating a Structured Collection of Topics

Depending on the scope and needs of a specific course, this assignment can be created in Markdown or DITA XML. The focus at this stage is on content creation and not necessarily on the production of deliverables. Whereas the HTML-based website from the previous assignment can easily produce a user-facing website with GitHub Pages, this assignment is more about the tasks associated with topic creation for later (in [Stage 4](../stage4/overview.md)) production of deliverables.

If this assignment is based on DITA, we recommend using only the basic DITA topic type and saving the specialized technical content types (concept, task, reference, and troubleshooting) for a more advanced assignment.

This assignment can use the same topic as the previous one, with an intended audience of family members, friends, or peers. The content for this assignment should be based on something that the author collects or is a fan of. It could be a collection of PS5 games or a Harry Potter series of topics with detailed entries in which the student reviews the books, movies, or characters.

### Creating content

Students should plan and create DITA topics (and a map) or Markdown files for entries in a collection. We recommend using the [github.dev web-based editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor), which provides many of the benefits of Visual Studio Code without additional downloads.If students or instructors do not want to interact directly with DITA code, they can use the demo version of [Oxygen Web Author](https://www.oxygenxml.com/xml_web_author.html), which integrates with GitHub and is functional for lightweght projects. For more advanced, semester-long projects, instructors should consider a downloadable DITA editor like [Oxygen Editor](https://www.oxygenxml.com/), which is relatively affordable in its academic license and also offers a free trail, or [XMLMind](https://www.xmlmind.com/xmleditor/), which offers an open source personal edition.

The assignment must require one topic or file per entry, following a content model in a detailed but concise tone. Images must include alt text content and, if included in DITA topics, be embedded in `<fig>` environments.

Consult the resources page for this stage, which includes readings about Lightweight DITA (LwDITA). In LwDITA environments, a collection can include both DITA and Markdown topics.

Students should upload their collections of topics to a GitHub repository. Evaluation criteria can include the following:

#### Structure and Organization

- Clear and logical organization of topics  
- Effective use of a DITA map to link topics (if using DITA)  

#### Content Clarity and Depth

- Clear and concise writing suitable for the intended audience  
- Quality and quantity of content appropriate for the course  
- Depth of information and appropriate level of detail  

#### Technical Implementation

- Correct use of DITA or Markdown syntax  
- Clean and well-organized code  
