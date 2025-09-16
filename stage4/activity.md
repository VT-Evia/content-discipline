# Deliver and Maintain Activities

In this stage, activities focus on processing content topics to produce user-facing deliverables.

## Multichannel Publishing with Markdown Activity

For this activity, we recommend using the [Markdown/Pandoc GitHub Actions template](https://github.com/VT-Evia/pandocactions) repository in combination with a Markdown editor such as Visual Studio Code. See the [Stage 3 resources](../stage3/resources.md) page. The template will take Markdown topics as input and process them via the document converter [Pandoc](https://pandoc.org/) to create deliverables in HTML, PDF, and EPUB formats.

### Overview

Students can take topic collections created in Markdown for the [Stage 3 activities](../stage3/activities.md) or convert to Markdown topics one of the suggested example documents to examine from the [Identifying Content Types and Relationships](../stage1/activity-identifyingcontenttypes.md) in Stage 1.

Each Markdown file should contain a single topic representing an item in a collection or a section in one of the example documents to examine. Follow the formatting requirements in the template's README file. For a hypothetical collection of songs of the summer (2025 version), each file could have a fixed structure as follows:

``` markdown
---
navtitle: "Song Title"
---

# Song title

## Performer

## Personal review

## Ranking
```

Then, students will develop content to populate each entry of the collection. Example:

``` markdown
---
navtitle: "Ordinary"
---

# Ordinary

## Alex Warren

## Personal review

This song is representative of the screaming is singing movement of 2024-2025 mainly performed by male singers. It also belongs to a category of semi-religious pop songs. I think it was particularly popular this summer because its tenure on the hit parade coincided with wedding season in the United States.

## Ranking

3 out of 5 stars.
```

The `navtitle` element in the metadata preface will be used by the template to generate a table of contents or navigation menu for the deliverables.

The naming of files in the collection should look as follows to create a hierarchy:

```
index.md
01-ordinary.md
02-what-i-want.md
03-just-in-case.md
04-im-the-problem.md
05-luther.md
06-die-with-a-smile.md
07-golden.md
08-pink-pony-club.md
09-manchild.md
10-love-me-not.md
```

In this example, `index.md` would be an introductory topic that would become the home page of a website deliverable or the introduction of a PDF or EPUB deliverable. 

Follow the placement of files steps in the template repository's README file.

## Advanced Technical Content DITA Activity

For this activity, we recommend using the [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository in combination with a DITA-aware editor such as Oxygen XML (standalone editor or demo web author) or XMLMind. See the [Stage 3 resources](../stage3/resources.md) page for links and tutorials related to these tools. For years, we have used a version of the following activity to introduce students to more advanced technical content topic types and workflows using DITA XML. Particularly, the following resources should help with this activity:

- Evia, C., Sharp, M., & Pérez-Quiñones, A. (2015). Teaching structured authoring and DITA through rhetorical and computational thinking. *IEEE Transactions on Professional Communication*, 58(3), 328–343.
- Evia, C. (2018). *Creating intelligent content with Lightweight DITA*. New York: Routledge (mainly Chapter 8).

### Overview

One of the benefits of using DITA is its ability to support single-sourcing and content reuse across multiple publication platforms and audiences. A single topic written in a structured authoring environment could appear in hundreds of different documents across a variety of media, and one change to the source file will automatically update all those documents. This assignment gives students the opportunity to practice single-sourcing and reuse on a small scale.

For this assignment, students will write a collection of DITA topics (we recommend at least 12) and a DITA map for those topics. Then, they will produce two final deliverables in different media for different audiences.

The scenario for this assignment is based on two personas: a fictional roommate named Armando and a relative visiting the student (e.g., a mom). The goal is to create detailed topics explaining to these audiences (Armando and the mom) how to prepare breakfast, lunch, and dinner using available ingredients and tools. Armando follows a strict vegan diet, so students must adapt and customize their recipes accordingly. The activity requires real recipes with pictures, citing sources from websites or cookbooks. Recipes must be fully adapted to the DITA standard.

For the topics, students should use a combination of concepts and tasks. Concepts can serve as customized introductions for each section, tailored to the audience. Tasks should explain the steps involved in each recipe. Reference and troubleshooting topics are welcome but not required.

The DITA map should include at least 10 different recipes, organized by breakfast, lunch, and dinner. Since the goal is reuse, some overlap is expected—and, in this case, required. For example, several recipes should include a conditional ingredient (or ingredients) that can be adapted for vegan and non-vegan users (e.g., replacing bacon with tofu).

As an alterative to the recipe scenario, students can continue the content strategy project that they started in [Stage 2](../stage2/contentstrategyactivities.md) and/or further develop the collection of topics that they created in [Stage 3](../stage3/activity.md). 

The [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository will automatically produce both PDF and website deliverables for the project. As we discussed in the section Stage 4 in Chapter 7 of our book *Technical Communication and the Discipline of Content*, the DITA Open Toolkit is the primary engine for transforming DITA content assets into a variety of user deliverables. GitHub Actions enable processing inside repositories, and a workflow can invoke the DITA Open Toolkit automatically in a process of continuous integration and development to build and serve website and PDF deliverables. This template enables DITA Open Toolkit GitHub Actions. 
