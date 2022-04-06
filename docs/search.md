---
layout: default
title: Creating and Pushing a Project to a GitHub Repository 
nav_order: 4
has_children: false
permalink: /docs/navigating
---

{: .fs-6 .fw-300 }

# Creating and Pushing a Project to a GitHub Repository 
{: .no_toc }

---

A GitHub repository is a powerful tool to host your projects in a stable environment. It allows authorized users to collaborate on the project and takes snapshots so you can return to the last stable version of your project in case bugs arise. In this section, we will guide you through the necessary steps to create and publish your project to a GitHub repository.

---

### Table of contents
{: .no_toc .text-delta }
* TOC
{:toc}

---

## Committing and Pushing a Project

A commit, or "revision", is an individual change to a file (or set of files). When you make a commit to save your work, Git creates a unique ID (a.k.a. the "SHA" or "hash") that allows you to keep record of the specific changes committed along with who made them and when. The git push command is used to upload local repository content to a remote repository. Pushing is how you transfer commits from your local repository to a remote repo. These are both necessary to add your files to a GitHub repository.

---

**1.** Go to the VCS panel which is present at the top of the PyCharm main menu bar and click on it.

![1](https://user-images.githubusercontent.com/18428358/161925375-8f748453-3ccf-4ca6-8cf9-5580b129b6cf.png?raw=true)

<br />
<br />

**2.** After clicking “Enable Version Control Integration…” a pop up window will appear. Select Git from the drop-down menu and click OK. This will initialize the project for GitHub.

![2](https://user-images.githubusercontent.com/18428358/161925623-91d629fc-f983-48c1-b17e-6197cb2dd5e2.png?raw=true)

<br />
<br />

**3.** The next step is to click on the green check mark present in the upper part of the PyCharm. This symbol refers to Commit and its purpose is to collect all unversioned files and make them ready to update on GitHub.

![3](https://user-images.githubusercontent.com/18428358/161925791-ab49ef5f-2793-471b-9ea6-bd0e18e66923.png?raw=true)

<br />
<br />

**4.** After clicking this a new screen will pop up like the following. First, click the arrow next to “Unversioned Files”.

![4](https://user-images.githubusercontent.com/18428358/161926246-77167470-2592-48d2-b564-3d041e285643.png?raw=true)

<br />
<br />

**5.** Next, select the files to commit and push to the GitHub repository by clicking the boxes next to the file names.

![5](https://user-images.githubusercontent.com/18428358/161926429-330f5ad2-92fd-434e-9b37-6e8adb88d980.png?raw=true)

<br />
<br />

**6.** After selecting the files to publish to our GitHub repository, include a commit message to give context about a change to the repository for fellow developers.

![6](https://user-images.githubusercontent.com/18428358/161926562-2727f9ad-6037-4f2d-a6d1-2f251e67eb29.png?raw=true)

Click the text field to type your commit message.

<br />
<br />

**7.** After providing a commit message, click the “Commit and Push…” button to commit your changes to the GitHub repository.

![7](https://user-images.githubusercontent.com/18428358/161926852-6ad97f97-0936-4615-baaa-4f729ef03925.png?raw=true)

<br />
Now that the project files have been committed and pushed, you will need to create a GitHub repository to house the files.
<br />

## Creating a GitHub Repository

**8.** Make your way to the menu bar and click “Git”. A dropdown menu will appear, hover over “GitHub” and click “Share Project on GitHub” when it appears on the side.

![8](https://user-images.githubusercontent.com/18428358/161927434-591a32bb-9764-4b30-954c-458aaae5e1fd.png?raw=true)

<br />
A window will appear where you can give the repository a name, remote, and description.
<br />

**9.** Click the text box next to “Repository name” and set the name for this project.

![9](https://user-images.githubusercontent.com/18428358/161927676-c62bc0c7-c2e7-42fb-b52b-d05a2f235693.png?raw=true)

<br />
<br />

**Optional** You can also choose to make your GitHub repository private so only authorized users can access your project.

To do so, click the box next to “Private”.

![10](https://user-images.githubusercontent.com/18428358/161927782-d94ad57a-af3e-4d59-9826-ac8e237973db.png?raw=true)

<br />
<br />

**10.** After providing a name for the repository, we are ready to publish the project on GitHub.

Click the “Share” button when you’re ready to upload your project.

![11](https://user-images.githubusercontent.com/18428358/161928104-97d2b523-3c45-463e-9416-f71cfea15c45.png?raw=true)

<br />
<br />

Congratulations! Your project is now deployed and accessible through GitHub.









