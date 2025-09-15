# Prompt to Generate the HTML/CSS/JS Structure (No Sample Content)

You are a coding assistant. Generate only code and minimal code comments—no prose explanations. Create a small, static website scaffold (HTML/CSS/JS) suitable for hosting on GitHub Pages. The site will implement a **single, consistent content model** for multiple entries/pages. **Do not generate any sample content, filler text, or “lorem ipsum.”** Use clearly marked placeholders and empty elements where students will author their own content.

## Audience
- Primary audience: Classmates, friends/family, prospective students, etc.
- The design should prioritize readability, simple navigation, and accessibility for this audience.

## Topic & Content Model
- Topic domain: “Top 10 songs of the summer,” “My current semester courses,” “Favorite books,” etc.)
- Each page shows **one entry** that follows this **exact content model** (keep labels visible in the code as `data-field` attributes and comments):
  - `title` (short title for the entry)
  - `creator` (e.g., performer/author/instructor)
  - `image` (single representative image)
  - `description` (student-authored review/summary/notes)
  - `rating` (1–5 stars)
- Ensure the HTML includes **empty elements / placeholders** for each field. **Students will author content later**—do not include any example values.

## Technical Requirements
1. **Files & Structure**
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
   ```
  
2. **HTML & Accessibility**
   - Use semantic HTML5 with `header`, `nav`, `main`, `footer`.
   - Include a skip-to-content link and sensible heading hierarchy.
   - Provide an accessible **nav** with links to **Home (index.html)** and a generic **All Entries** anchor.
   - In `entry.html`, include an ARIA-labeled section for the entry and `data-field` attributes for each field:
     - Title element: `<h1 data-field="title"></h1>`
     - Creator: `<p data-field="creator"></p>`
     - Image wrapper with **empty** `src` and **placeholder** `alt` that says: `<!-- STUDENT: write meaningful alt text -->`
     - Description: `<section data-field="description"></section>`
     - Rating: an empty container with 5 star outlines and an ARIA label; **no preselected value**.
   - Do not include any example text; instead, include comments like `<!-- STUDENT: write your own [field] here -->`.

3. **Index Page (Card List)**
   - `index.html` shows a grid/list of entry **cards** with:
     - a title placeholder
     - a thumbnail image placeholder
     - a short teaser area (empty)
     - a “View entry” link to `entry.html?slug=PLACEHOLDER`
  
4. **CSS**
   - Create a clean, responsive layout using CSS Grid/Flexbox.
   - No frameworks. Keep the palette neutral and minimal.
  
5. **JavaScript**
   - `main.js` should:
     - Fetch `data/entries.json` on `index.html` and render cards. If empty, show a no-entries state.
     - On `entry.html`, read a `?slug=` query param, look up the matching entry (once students add data), and populate fields. Until data exists, show placeholder states and **do not** inject any sample values.
  
6. **README.md**
   - Explain:
     - The purpose of the scaffold.
     - Where students should write their own content.
   - Explicitly state: **“Students must author all page content themselves. Do not use AI to generate the content of entries.”**

7. **Content Policy (Critical)**
   - Include a prominent comment block at the top of `index.html` and `entry.html`:
     ```
     <!--
       CONTENT POLICY FOR THIS ASSIGNMENT:
       - Students must author all entry content themselves.
       - Do NOT paste or generate content from AI systems.
       - This scaffold provides structure only (HTML/CSS/JS).
       - Replace placeholders with your own writing and media.
     -->
     ```

8. **Quality & Consistency Guards**
   - Ensure the same field order and labels appear across `index.html` cards and `entry.html` detail view.
 
**Generate the code now.**
