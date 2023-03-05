# Hosting a Resume on Github Pages

## PURPOSE

- Describing the practical steps to host and format a resume using the software stack on `GitHub`. 
- Using lightweight markup languages such as `Markdown` to create technical documentation that is easy to read, write, and maintain.
- Using version control systems such as `git` to keep track of changes made to the documentation.

### PREREQUISITES

Before following the instructions in this README, you will need the following:

- `VSCode.`
- `Web Browser.`

### INTRODUCTION

#### STEP 1: Create a Github Account
If you have a github account already, you can skip to step 2. 
1. Go to the GitHub homepage at <https://github.com/>.
2. Click on the `Sign up` button in the top right corner of this page.
3. Enter your preferred username, email address, and a strong password.
4. Click the `Create account` button.
5. Choose a plan. You can choose the free plan for now.
6. Follow the on-screen steps to complete filling out your personal information and selecting your preferences.
7. A link has been sent to you to verify at the email address you have provided. Verify your email address by clicking the link.

#### STEP 2: Create a New Repository
The Second step in hosting your resume on GitHub Pages is to create a new repository on GitHub. You can do this by following these steps:

1. Log in to your GitHub account if you are already not logged in.
2. Click on the `+` icon in the top right corner of the screen. Then select `New repository`.
3. Give your repository a name, For example, `online-resume`, and select `Public`.
4. Check the box that says `Initialize this repository with a README`.
5. Click the `Create repository` button.

#### STEP 3: Creating the Resume in Markdown Format
This step will cover creating the resume in markdown format. 

1. If you are not familiar with `Markdown`, please refer to this [link](https://www.markdownguide.org/basic-syntax/) for a quick introduction. 
2. Open VSCode.
3. Click on `New file`.
4. Write the filename as `index.md`. Then press the `enter` button on your keyboard.
5. Select the location where you want to save this file.
6. Start writing your resume in markdown format. You can press `ctrl + k` then `v` to open a preview window at the side. This is a default feature in VSCode for a live preview of your markdown file.
7. When the writing is done, save the file by pressing `ctrl + s`.

#### STEP 4: Uploading the Resume
In this step, we will upload our markdown formatted resume to our github resume. You can do this by following these steps: 

2. Go to the repository on Github from your browser.
3. Click on the "Add file" dropdown button and select "Upload files".
4. Drag and drop the resume from your computer.
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
2. go to `https://username.github.io/repository_name/`, where username is your Github username and repository_name is the name of the repository where you uploaded your resume.
3. You should see your resume displayed on the site.

#### Visual Representation Example
<img src="/assets/images/resume.gif" alt="resume_example" width="500" height="300" />


# Relating to Andrew Etter's Principles