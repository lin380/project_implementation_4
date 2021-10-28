# README

<!-- REMEMBER: 
You can preview a formatted version of this README.md document by clicking the 'Preview' button in the RStudio toolbar.
-->

## Preparation

- Reflect on your interests in language and linguistics
- Review the concepts on identifying a research problem and developing a research statement in [TAD Chapter 4 "Framing research"](https://lin380.github.io/coursebook/framing-research.html)
- Review the concepts on curating corpus data in [TAD Chapter 2 "Understanding data"](https://lin380.github.io/coursebook/understanding-data.html) and implementing curation steps in [TAD Chapter 7 "Transform data"](https://lin380.github.io/coursebook/transform-data.html)
- Continue to refine your project statements and data acquisition implementation.
- Review the steps for working with RStudio, Git, and GitHub in [Recipe #5](https://lin380.github.io/tadr/articles/recipe_5.html) and Lab #5. 

## Objectives

- Continue to refine your text analysis project
- Add your data transformation implementation strategy to your project
- Apply the edit, add, commit, push workflow to update your GitHub page
- Continue to apply your growing knowledge of R

## Instructions

### Setup

1. Open your research project (`project_<your_last_name>`) on RStudio Cloud. 
2. Open the `3_transform_dataset.Rmd` file in the `analysis/` directory. 

### Project

In this project implementation step you will be working to refine the process by which you will transform the dataset(s) you will use in your text analysis project. You will build on the curated dataset you have created and documented and move to create a transformed dataset that is more in line with your analysis approach yet reflects the structural characteristics to maintain a tidy dataset.

The `3_transform_dataset.Rmd` file has a similar template structure (to the previous analysis files) in the prose section of the .Rmd document. This includes 'About' , 'Setup', 'Run', and 'Finalize' sections with some relevant subsections. This structure is not set in stone and merely helps you start to think about the steps that your processing and documentation should most likely include. Each of the (sub)sections has a comment (`<!-- ... -->`) to guide you as to what you might expect to add in these sections.

**Tasks**

1. Provide a description that overviews the aim of this script (.Rmd). 
2. Include any information necessary for someone to know to be able to reproduce this script. 
3. Load the appropriate packages that you will need. 
4. Include the relevant code to transform, store, and document the data on your disk.
5. Make sure that your data is stored on disk in a plain-text format (most likely `.csv`) inside the `data/derived/` directory. 
6. Source the `_pipeline.R` file. Either through: 
  - opening the `_pipeline.R` file and clicking the 'Source' button.
  - or, in the R Console running `source("_pipeline.R")`

Each step of your project should be seen as modular --that is, that one script should not directly depend on the next in the sequence. By storing the relevant data necessary for the next step in the `data/derived/` directory you are ensuring that no object(s) from the `3_transform_dataset.Rmd` R session is required for the next step `4_analyze_dataset.Rmd`.

*Note: The exact data transformation steps likely change in the coming weeks, but it is important to make a concerted effort to develop the scaffolding (even if only [psuedocode](https://codinghero.ai/what-is-pseudocode/)). We will workshop the ideas that surface from the work on this project orientation step and discuss collective and individual questions to continue to develop and hone our projects so that they show the most promise for being viable.*

### Update GitHub

1. Now run the Git commands in the Terminal to add, commit, and push your updates to your GitHub repository/ website. 

- `git status`
- `git add -A`
- `git commit -m '<briefly describe what you've done>'`
- `git push`

**Remember:** your PAT has probably expired (it only lasts 12 hours in RStudio Cloud) so you will need to run `gitcreds::gitcreds_set()` in the R Console and paste in your PAT before you run `git push` (otherwise you will get cryptic error). 

## Submission

1. Navigate to your GitHub website (where the web page shows) and copy the link to the main page where you have added your changes. 
3. Go to the Canvas submission page for "Project implementation #3" and paste this URL link into the 'website url' submission field. In the 'Text Entry' field add your self-assessment comments.

**IMPORTANT NOTE:**

We will continue using GitHub to post our work. In addition to saving our project work and hosting a website for our projects, GitHub also has a robust set of features for commenting and collaborating on code. We will use these features to receive and ask for feedback on our code and ideas.
