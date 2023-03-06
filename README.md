# Hosting a Resume on Github Pages

## PURPOSE

- Describing the practical steps to host and format a resume using the software stack on `GitHub`. 
- Using lightweight markup languages such as `Markdown` to create technical documentation that is easy to read, write, and maintain.
- Using version control systems such as `git` to keep track of changes made to the documentation.

### PREREQUISITES

Before following the instructions in this README, you will need the following:

- `Web Browser.`
- `A Resume in Markdown Format`.

### INTRODUCTION

#### STEP 1: Create a Github Account
If you have a GitHub account already, you can skip to step 2. 
1. Go to the GitHub homepage at <https://github.com/>.
2. Click on the `Sign up` button in the top right corner of this page.
3. Enter your preferred username, email address, and strong password.
4. Click the `Create account` button.
5. Choose a plan. You can choose the free plan for now.
6. Follow the on-screen steps to complete filling out your personal information and selecting your preferences.
7. A link has been sent to you to verify at the email address you have provided. Verify your email address by clicking the link.

#### STEP 2: Create a New Repository
The Second step in hosting your resume on GitHub Pages is to create a new repository on GitHub. You can do this by following these steps:

1. Log in to your GitHub account if you are already not logged in.
2. Click on the `+` icon in the top right corner of the screen. Then select `New repository`.
3. Give your repository a name, For example, `online-resume`, and select `Public`.
4. Check the box that says, `Initialize this repository with a README`.
5. Click the `Create repository` button.

#### STEP 3: Rename the Resume File.
This step will cover creating the resume in markdown format. 

1. Rename the resume filename as `index.md`.
2. Remember the location where you saved this file.

#### STEP 4: Uploading the Resume
In this step, we will upload our markdown formatted resume to our GitHub resume. You can do this by following these steps: 

2. Go to the repository on GitHub from your browser.
3. Click on the "Add file" dropdown button and select "Upload files".
4. Drag and drop the resume file, namely `index.md` from your computer.
5. Click on the "Commit changes" button at the bottom to upload the files to the repository.

#### STEP 5: Creating the Configuration File for Jekyll
To generate a static site and add a theme to your resume, we will be using Jekyll. Jekyll is a static site generator that allows you to create websites and blogs by writing content in Markdown or HTML and using templates to generate the pages. To generate a static site using Jekyll and add a theme, we need to create a `_config.yml` file. From the repository, 
1. Click on the `"Add file"` dropdown button and select `"Create new file"`.
2. A text editor will appear. At the top of it, there is an empty field. Write the name your file here. The name must be exactly `_config.yml`
3. In the text editor, copy this code below.

```
remote_theme: pages-themes/slate@v0.2.0 # this line adds the slate theme of Jekyll. You can replace "slate@v0.2.0" with your preferred theme.

plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one

title: "RESUME OF [Your Name]" 
```
4. Click on the "Commit changes" button at the bottom.

#### STEP 6: Set up GitHub Pages
To activate the Github site hosting feature, follow the steps below.
1. In the repository, navigate to the "Settings" tab.
2. Scroll down to the "GitHub Pages" section on the left side of the page.
3. Select the branch you want to use as the source. In this case, select the main branch.
4. Click "Save."


#### STEP 7: Check your GitHub Pages site

1. Please wait up to 10 minutes for Github to build your site. However, the usual time is around 2 minutes.
2. go to `https://username.github.io/repository_name/`, where username is your GitHub username and repository_name is the name of the repository where you uploaded your resume.
3. You should see your resume displayed on the site.

#### Visual Representation Example
<img src="/assets/images/resume.gif" alt="resume_example" width="500" height="300" />

### More Resources: 

- [Markdown Tutorial](https://www.markdownguide.org/basic-syntax/) 
- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

### Authors and Acknowledgments
This README was created by Saif Mahmud and reviewed by Martin Popper, Aditya Kashyap, and Akashkumar Ghelani.

### FAQs
Q. Can I edit my resume after I have hosted it on GitHub Pages?

Yes, you can edit your resume after you have hosted it on GitHub Pages. Simply make the necessary changes to your Markdown file and save the changes. Then, upload the updated file to your GitHub repository using the same steps outlined in Step 4. Your changes should be reflected on your hosted resume shortly after GitHub rebuilds your site.

Q. Can I use a different theme for my GitHub Pages site?

Yes, you can use a different Jekyll theme by changing the remote_theme field in the _config.yml file to the theme you prefer. A list of Jekyll themes is available [here](https://pages.github.com/themes/). Once you update the _config.yml file, commit the changes and your GitHub Pages site will automatically update with the new theme.


<br>
<br>
<br>

# Relating to Andrew Etter's Principles

## Purpose 

Relate the practical steps described above to the general principles of current technical writing, as explained in Andrew Etter's book Modern Technical Writing.

## Prerequisite

- A general understanding of Andrew Etter's book, Modern Technical Writing.

## Correlation

1. Purpose: This section is an example of providing the audience with a clear objective of the document. This is one of the key principles of technical writing. It helps the readers understand the context and what they can expect from this document.

2. Prerequisite: To prevent frustration and failures later on, this section helps by identifying the necessary skills, knowledge, and resources needed for this particular task. One can focus on acquiring or improving them before moving on to the next step. This step also helps to identify who the audience should be for this document.

3. Step 1: Create a Github Account: This step is an example of breaking down the content into smaller, manageable chunks. It helps the readers focus on each step and reduces confusion or error.

4. Step 2: Create a New Repository: This step is an example of using descriptive headings to select the appropriate medium to communicate with the audience. By reading this heading, the audience will know the goal of this step.

5. Step 3: Creating the Resume in Markdown Format: In this step, the instructions are clear and concise, which is another principle of technical writing. It helps the readers follow the steps without getting overwhelmed by unnecessary information.

6. Step 4: Uploading the Resume: This step is an example of using an easy-to-follow manner. This step also uses the version control `git`` system to keep track of changes made to the document. 

7. Step 5: Creating the Configuration File for Jekyll: This step's process can be new and overwhelming to the audiences. Thus, a short description was added to provide a clear understanding and goal of this step.

8. Step 6: Set up GitHub Pages: This step is an example of using appropriate formatting and layout, such as using bullet points to make the content more understandable and scannable for the audience.

9. Step 7: Check your GitHub Pages site: This step is an example of providing a conclusion of the instructions, which is another principle of technical writing. It helps the readers understand the outcomes of following the instructions.

10. Visual Representation Example: This step is an example of using visual aids, such as images or videos to enhance the readers' understanding, which is another principle of technical writing.