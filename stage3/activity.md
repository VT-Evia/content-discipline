# Content Creation (and Management) Activities

Activities in this stage focus on content creation and not necessarily the production of user-facing deliverables. Topic-based content creation is built on a foundation of separating content from presentation, and in some cases the presentation is not in the hands of a content author. 

## Creating a Structured Website

Following the **Creating a Content Model** activity from [Stage 2](../stage2/contentstrategyactivities.md), students can create an HTML-based project to be managed in a GitHub repository and hosted as a website on GitHub Pages. The goal of this activity is not to create the kinds of reusable topics (content chunks) required in structured authoring workflows but rather to gain familiarity with applying a content model to content creation, using a code editor, and assembling a website.

A consistent format for every entry/page in this website activity is key to maintaining the content model. This is not an assignment for individual formatting across pages or entries. For topics, students can continue with the project that they started in Stage 2 (using this activity as an opportunity to create content in accordance with their content model), or they can select a topic that interests them. We have used topics ranging from the top 10 songs on the hit parade, to a collection of favorite books or movies, to a catalog of the courses a student is taking in a given term. 

Audience considerations will drive the content, so it is important to specify who the intended reader of the website deliverable is. If students are building on the activities that they completed in Stage 2 when developing a content strategy plan, their audience should already be well defined. If students are selecting topics of interest to them, they might build their website for family members and friends.

The project includes three main tasks: planning the content model, setting up the GitHub infrastructure, and creating content.

---

### Planning the Content Model

Each page on the planned website must follow the same structure and contain one topic. For example, a website with the top 10 songs of the summer might be based on a content model like the following:

- Song title  
- Performer  
- Single cover image  
- Personal review  
- Rating on a scale of 1 to 5 stars  

When we practice this activity, we allow students to use generative AI tools to generate the skeleton HTML, CSS, and JS files for the project, but their prompts must not ask for sample content. Students' prompts must emphasize functionality and user experience. We recommend having students use an LLM chat agent such as ChatGPT or Copilot to generate the code for their HTML, CSS, and JS files. Students can prompt the chat agent to develop a consistent structure for each web page in accordance with their content model. Students should save their files to a local folder on their machine (they will then upload their files to a GitHub repository that they will create as their next main task). 

Two alterative ways to generate the skeleton HTML, CSS, and JS files are as follows: 
- Use GitHub Copilot (via the "Chat with Copilot" icon in Github next to the search box). This approach allows for pushing the files directly to a GitHub repository - Copilot can be prompted to do this.
- Use the desktop version of [Visual Studio Code](https://code.visualstudio.com/). Visual Studio Code integrates with GitHub. Students who do not have a subscription to GitHub Copilot can sign up for a 30-day free trial directly from the downloaded version of Visual Studio Code. Using GitHub Copilot in Visual Studio Code, students can generate the HTML, CSS, and JS files for their website. They can also push these files directly to a GitHub repository.  

#### Sample Prompt

We have included a [sample, detailed prompt](sample-prompt.md) related to this assignment for an LLM chat agent. This prompt asks the chat agent to create the HTML, CSS, and JS files for a website. Students will need to customize the audience, topic domain, and content model in the prompt before asking the chat agent to generate the code. 

---

### Setting Up the GitHub Infrastructure

Students can follow these steps to create a repository, add their project files, and publish the site on GitHub Pages. This section focuses only on **infrastructure**—file organization, commits, and publishing. Students will author **all of their content** in later steps.

> **Prerequisites**
> - A GitHub account and the ability to sign in.
> - The HTML, CSS, and JS files generated **without** any sample content.
> - Recommended editor: the **github.dev** web editor (press `.` while viewing your repo on github.com).


### 1) Create a new repository

1. Go to <https://github.com/new>.
2. **Repository name**: choose something relevant to your topic (e.g., `summer-top-10`, `course-catalog`, `favorite-books`).
3. **Visibility**: select **Public** (recommended for GitHub Pages).
4. Check **Add a README file** (optional but helpful).
5. Click **Create repository**.

### 2) Open the repo in the github.dev editor (recommended)

- On your new repository’s main page, press the `.` (period) key to open the **github.dev** editor in your browser. 
- This gives you a full editor experience without installing anything locally. Learn more about the [github.dev web-based editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor).

### 3) Upload your files

1. From your repository page, click **Add file → Upload files**.
2. Drag-and-drop your local files/folders into the upload area.
3. Scroll down, enter a commit message, and click **Commit changes**.

> **Commit message guidance:** Write short, descriptive messages (e.g., “Create data folder and empty entries.json”). Small, frequent commits make it easier to review and troubleshoot.


### 4) Verify required files

- Confirm `index.html` exists at the root; this is the default entry point for GitHub Pages.
- Confirm `assets/css/styles.css` and `assets/js/main.js` are referenced correctly from your HTML.


### 5) Enable GitHub Pages to publish your site

1. Go to **Settings → Pages** in your repository.
2. Under **Build and deployment**, select:
   - **Source**: *Deploy from a branch*
   - **Branch**: `main` (or your default branch) and **/ (root)** as the folder
3. Click **Save**.
4. After a moment, GitHub will provide a public URL of the form:
https://<your-username>.github.io/<your-repo-name>/
5. Visit the URL to confirm the site loads. If you see a 404, wait a minute and refresh, or re-check that `index.html` is at the root.

----

### Creating Content

Once the students have their HTML, CSS, and JS files in their repository, they need to conduct research for the actual content that they need to write. Then, they will open each HTML file in the **github.dev** web editor (press `.` while viewing your repo on github.com) and create consistently structured, effective content that satisfies their users' information needs. To save changes to a file, students can click the **Source Control** icon on the leftside menu (it should indicate pending changes), enter a message in the commit message field that describes the changes, and click **Commit & Push**. The file will be updated in the repository and the change will be reflected when viewing the website hosted on GitHub Pages. If students created their files using the desktop version of Visual Studio Code, they can alternatively edit their files in Visual Studio Code and commit and push them to their repository.    

---

## Creating a Structured Collection of Topics

Depending on the scope and needs of a specific course, this activity can be created in Markdown or DITA XML. The focus at this stage is on content creation and not necessarily on the production of deliverables. Whereas the HTML-based website from the previous activity can easily produce a user-facing website with GitHub Pages, this activity is more about the tasks associated with topic creation for later (in [Stage 3](../stage4/overview.md)) production of deliverables.

If this activity is based on DITA, we recommend using only the basic DITA topic type and saving the specialized technical content types (concept, task, reference, and troubleshooting) for a more advanced project. The basic DITA topic is a good fit for topics based on something that the author collects or is a fan of (e.g., a collection of PS5 games or a Harry Potter series of topics with detailed entries in which the student reviews the books, movies, or characters). The audience for this kind of project might be family members, friends, or peers. 

However, if students are continuing the content strategy project that they started in [Stage 2](../stage2/contentstrategyactivities.md), particularly if they are documenting a product or suite of products, they will likely need to use the specialized content types. If they used the structured website activity above as an opportunity to create HTML files that followed their content model developed in Stage 2, they can use this activity to practice adapting their content model and the content that they authored for their HTML files to the basic DITA topic type or to the specialized technical content types. 

### Creating Content

Students should plan and create DITA topics (and a map) or Markdown files for entries in a collection. We recommend using the [github.dev web-based editor](https://docs.github.com/en/codespaces/the-githubdev-web-based-editor) for Markdown files (the desktop version of Visual Studio Code is also a good option but must be downloaded). A great option for creating DITA topics is the demo version of [Oxygen Web Author](https://www.oxygenxml.com/xml_web_author.html), which integrates with GitHub and is functional for lightweight projects. For more advanced, term-long projects, instructors should consider a downloadable DITA editor like [Oxygen Editor](https://www.oxygenxml.com/), which is relatively affordable in its academic license and also offers a free trial, or [XMLMind](https://www.xmlmind.com/xmleditor/), which offers an open source personal edition.

LIST SUGGESTED TUTORIALS FOR OXYGEN AND XMLMIND HERE

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
