# Deliver and Maintain Activities

In this stage, activities focus on processing content topics to produce user-facing deliverables. Students can take topic collections created in Markdown or DITA from the [Stage 3 activities](../stage3/activities.md) and put them into production mode using the [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) or the [Markdown/Pandoc GitHub Actions template](https://github.com/VT-Evia/pandocactions) recommended for this stage.

## Advanced Technical Content DITA Activity

For this activity, we recommend using the [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository in combination with a DITA-aware editor such as Oxygen XML (standalone editor or demo web author) or XMLMind. See the [Stage 3 resources](../stage3/resources.md) page for links and tutorials related to these tools. For years, we have used a version of the following activity to introduce students to more advanced technical content topic types and workflows using DITA XML.

### Overview

One of the benefits of using DITA is its ability to support single-sourcing and content reuse across multiple publication platforms and audiences. A single topic written in a structured authoring environment could appear in hundreds of different documents across a variety of media, and one change to the source file will automatically update all those documents. This assignment gives students the opportunity to practice single-sourcing and reuse on a small scale.

For this assignment, students will write a collection of DITA topics (we recommend at least 12) and a DITA map for those topics. Then, they will produce two final deliverables in different media for different audiences.

The scenario for this assignment is based on two personas: a fictional roommate named Armando and a relative visiting the student (e.g., a mom). The goal is to create detailed topics explaining to these audiences (Armando and the mom) how to prepare breakfast, lunch, and dinner using available ingredients and tools. Armando follows a strict vegan diet, so students must adapt and customize their recipes accordingly. The activity requires real recipes with pictures, citing sources from websites or cookbooks. Recipes must be fully adapted to the DITA standard.

For the topics, students should use a combination of concepts and tasks. Concepts can serve as customized introductions for each section, tailored to the audience. Tasks should explain the steps involved in each recipe. Reference and troubleshooting topics are welcome but not required.

The DITA map should include at least 10 different recipes, organized by breakfast, lunch, and dinner. Since the goal is reuse, some overlap is expected—and, in this case, required. For example, several recipes should include a conditional ingredient (or ingredients) that can be adapted for vegan and non-vegan users (e.g., replacing bacon with tofu).

The [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository will automatically produce both PDF and website deliverables for the project.
