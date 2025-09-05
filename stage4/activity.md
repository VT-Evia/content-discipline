# Deliver and Maintain Activities

In this stage, activities are related to the processing of content topics to produce user-facing deliverables. Students can bring topic collections created in Markdown or DITA from the [Stage 3 activities](../stage3/activities.md) and put them in production mode using the [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) or the [Markdown/Pandoc GitHub Actions template](https://github.com/VT-Evia/pandocactions) recommended for this stage.

## Advanced technical content DITA activity

For this activity, we recommend using the [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository in combination with a DITA-aware editor like Oxygen XML (standalone editor or demo web author) or XMLMind. See the [Stage 3 resources](../stage3/resources.md) page for links and tutorials related to these tools. For years, we have used a version of the following activity to introduce students to more advanced technical content topic types and workflows using DITA XML.

### Overview

One of the benefits of using DITA is its ability to serve projects that single-source and reuse content across a number of publication platforms and across a number of audiences. One single topic written in a structured authoring environment could show up in hundreds of different documents across a variety of media, and one single change to the source file will automatically update all those documents. This assignment will give students the opportunity to practice single-sourcing and reuse on a small scale

For this assignment, students will write a collection of DITA topics (we recommend at least 12) and a DITA maps for those topics. Then, students will produce two final deliverables in different media for different audiences.

The scenario for this assignment is based on the persona of a fictional roommate named Armando and the persona of a relative visiting the student (e.g. a  mom). The goal is to create very detailed topics telling your audiences (Armando and mom) how to make breakfast, lunch, and dinner with available ingredients and tools. Armando is on a strict vegan diet, so students need to adapt and customize their recipes. The actvity needd real recipes with pictures, citing sources from websites or cookbooks. The recipes will need to be fully adapted to the DITA standard.

For the topics, students should use a combination of concepts and tasks. Concepts, for instance, could be used as unique introduction for each section, customized for that audience. Tasks, of course, explain the steps involved in a recipe. Reference and troubleshooting topics are welcome, but not required.

The DITA map should include at least 10 different recipes (organized by breakfast, lunch, and dinner). Remember that the point of reuse is that some overlap is expected, or in this case, required: we will need several recipes with a conditional ingredient (or ingredients) that could be adapted for vegan and non-vegan users (example: replace tofu for bacon).

The [DITA Open Toolkit GitHub Actions template](https://github.com/VT-Evia/dita-ot-actions) repository will automatically produce PDF and website deliverables for the project.
