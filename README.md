# Hosting a Resume on GitHub Pages

## PURPOSE

- Describing the practical steps to host and format a resume using the software stack on `GitHub`. 
- Using lightweight markup languages such as `Markdown` to create technical documentation that is easy to read, write, and maintain.
- Using version control systems such as `git` to keep track of changes made to the documentation.

### PREREQUISITES

Before following the instructions in this README, you will need the following:

- `Web Browser.`
- `A Resume in Markdown Format`.

## INTRODUCTION

### STEP 1: Create a Github Account

If you have a GitHub account already, you can skip to step 2. 

1. Go to the GitHub homepage at <https://github.com/>.
2. Click on the `Sign up` button in the top right corner of this page.
3. Enter your preferred username, email address, and strong password.
4. Click the `Create account` button.
5. Choose a plan. You can choose the free plan for now.
6. Follow the on-screen steps to complete filling out your personal information and selecting your preferences.
7. Verify your email address by clicking the link that has been sent to you at the email address you have provided.

### STEP 2: Create a New Repository

The Second step in hosting your resume on GitHub Pages is to create a new repository on GitHub. You can do this by following these steps:

1. Log in to your GitHub account if you are already not logged in.
2. Click on the `+` icon in the top right corner of the screen. Then select `New repository`.
3. Give your repository a name, For example, `online-resume`, and select `Public`.
4. Check the box that says, `Initialize this repository with a README`.
5. Click the `Create repository` button.

### STEP 3: Rename the Resume File.

This step will cover preparing the resume for the static website. 

1. Rename the resume filename as `index.md`.
2. Remember the location where you saved this file.

### STEP 4: Uploading the Resume
In this step, we will upload our markdown formatted resume to our GitHub resume. You can do this by following these steps: 

2. Go to the repository on GitHub from your browser.
3. Click on the "Add file" dropdown button and select "Upload files".
4. Drag and drop the resume file, namely `index.md` from your computer.
5. Click on the "Commit changes" button at the bottom to upload the files to the repository.

### STEP 5: Creating the Configuration File for Jekyll

To generate a static site and add a theme to your resume, we will be using Jekyll. Jekyll is a static site generator that allows you to create websites and blogs by writing content in Markdown or HTML and using templates to generate the pages. To generate a static site using Jekyll and add a theme, we need to create a `_config.yml` file. From the repository, 

1. Click on the `"Add file"` dropdown button and select `"Create new file"`.
2. Write the name your file at the top of the text editor. The name must be exactly `_config.yml`
3. Copy this code below in the text editor.

```
remote_theme: pages-themes/slate@v0.2.0 # this line adds the slate theme of Jekyll. You can replace "slate@v0.2.0" with your preferred theme.

plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one

title: "RESUME OF [Your Name]" # Replace "[Your Name]" with your first and last name.
```

4. Click on the `Commit changes` button at the bottom.

### STEP 6: Set up GitHub Pages

To activate the Github site hosting feature, follow the steps below.

1. In the repository, navigate to the `Settings` tab.
2. Scroll down to the `GitHub Pages` section on the left side of the page.
3. Select the branch you want to use as the source. For now, select the `main` branch.
4. Click `Save.`


### STEP 7: Check your GitHub Pages site

1. Wait up to 10 minutes for Github to build your site. However, the usual time is around 2 minutes.
2. Go to `https://username.github.io/repository_name/`, where username is your GitHub username and repository_name is the name of the repository where you uploaded your resume.
3. You should see your resume displayed on the site.

### Visual Representation Example

<img src="/assets/images/resume.gif" alt="resume_example" width="500" height="300" />

## More Resources: 

- [Markdown Tutorial](https://www.markdownguide.org/basic-syntax/) 
- [Modern Technical Writing: An Introduction to Software Documentation](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## Authors and Acknowledgments
This README was created by Saif Mahmud and peer reviewed by Aditya Kashyap. 
The theme used in the resume is Jekyll `slate@v0.2.0` found [here](https://github.com/pages-themes/slate).

## FAQs
Q. Can I edit my resume after I have hosted it on GitHub Pages?

Yes, you can edit your resume after you have hosted it on GitHub Pages. Simply make the necessary changes to your Markdown file and save the changes. Then, upload the updated file to your GitHub repository using the same steps outlined in Step 4. Your changes should be reflected on your hosted resume shortly after GitHub rebuilds your site.

Q. Can I use a different theme for my GitHub Pages site?

Yes, you can use a different Jekyll theme by changing the remote_theme field in the _config.yml file to the theme you prefer. A list of Jekyll themes is available [here](https://pages.github.com/themes/). Once you update the _config.yml file, commit the changes and your GitHub Pages site will automatically update with the new theme.


<br>
<br>

# Relating to Andrew Etter's Principles

## Purpose 

Relate the practical steps described above to the general principles of current technical writing, as explained in Andrew Etter's book Modern Technical Writing.

## Prerequisite

- A general understanding of Andrew Etter's book, Modern Technical Writing.

## Correlation

### 1. Using a lightweight markup language.
In Etter's book, "Modern Technical Writing," he discusses the importance of using lightweight markup languages. A lightweight markup language such as Markdown makes it easy to create technical documentation that is easy to read, write, and maintain. This readme document and the resume we have made were in markdown format. From a markdown format, one can easily convert it into an HTML document without worrying about the complexities of HTML markup.

### 2. Format a document with a static site generator.
The book also emphasizes using a static site generator such as Jekyll. Jekyll is a static site generator that allows the creation of websites by writing content in Markdown or HTML and using templates to generate the pages. In the instructions above, we have used Jekyll to generate a static site and add a theme to our resume. By creating a _config.yml file and specifying a theme, we were able to generate a professional-looking resume with minimal effort.

### 3. Share/host documents on a distributed version control system.
Etter highly encouraged the advantages of utilizing version control systems like Git to track modifications made to the documents. In this README, we have used a version control system called GitHub as a platform to host our resume. With Git, we can effectively track and revert any modifications made to our documents. Moreover, by hosting our resume on GitHub, we can seamlessly share it with others and engage in collaborative work on the same document for free.

In conclusion, by following the practical steps outlined in this README, we have demonstrated the key principles of using lightweight markup languages, formatting a document with a static site generator, and sharing/hosting documents on a distributed version control system. As outlined in Etter's book, these principles, are very effective for creating and maintaining technical documentation.
