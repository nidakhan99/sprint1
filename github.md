# GITHUB <img src="https://cdn-icons-png.flaticon.com/512/25/25231.png" width="8%" height="8%">   


| Author | Created on | Version | Last updated by | Last edited on |
| ------ | ---------- | ------- | --------------- | -------------- |
| Nida Khan    | 19-03-24   | version 1.3 | Nida Khan         | 19-03-24       |




## Introduction 

GitHub is as a platform for hosting code, facilitating version control and collaborative efforts. It enables seamless project collaboration regardless of location. This guide instructs you in fundamental GitHub concepts such as repositories, branches, commits, and pull requests, offering a comprehensive understanding of these essential elements.

Programmers can pick source codes in many different languages and use Git, the command-line interface, to make and keep track of any changes. As a result, every team member receives help to work together on multiple projects from any location, thanks to top-notch collaboration. As a token of its flexibility, GitHub lets users review previous projects created at an earlier point in time.


## Purpose
GitHub serves several purposes, acting as a platform for collaboration, version control, and software development. Here are some of the key purposes of GitHub:

1. **Version Control**: GitHub provides a distributed version control system (VCS) based on Git. It allows developers to track changes to their code, collaborate with others, and manage different versions of their projects effectively.

2. **Collaboration**: GitHub facilitates collaboration among developers by providing tools for code review, issue tracking, and project management. Multiple developers can work on the same project simultaneously, contributing changes, suggesting improvements, and resolving issues.

3. **Code Hosting**: GitHub hosts millions of open-source projects, making it a central hub for developers to share their code with the community. It allows developers to publish their projects publicly or privately, making it accessible to collaborators and users.

4. **Community Engagement**: GitHub fosters a vibrant developer community where individuals and teams can connect, share knowledge, and learn from each other. Developers can follow projects, participate in discussions, and contribute to open-source projects, thereby building their reputation and expanding their network.

5. **Documentation**: GitHub provides features for documenting projects, including wikis and README files. Developers can create comprehensive documentation to guide users and contributors on how to use, contribute to, and extend their projects.

6. **Continuous Integration and Deployment (CI/CD)**: GitHub integrates with CI/CD tools like GitHub Actions and third-party services, enabling developers to automate build, test, and deployment processes. This ensures code quality, reduces manual effort, and accelerates the delivery of software updates.


7. Project Management: GitHub offers project management tools such as project boards, milestones, and issue trackers to help teams organize and prioritize their work. These tools facilitate task tracking, bug fixing, and feature implementation throughout the software development lifecycle.


## Key feature & functionality
1. **Smooth project management**:
GitHub project management features are vast. It provides a place where project managers and developers can collaborate to coordinate, track, and update their work. With this, projects are fast, timely, and transparent. 

2. **Safe packages**:
Thanks to the GitHub introduction, you can publish packages privately, within the team, or publicly to the open-source community. You can then use or reuse the packages by downloading them from GitHub.

3. **Improved code writing**:
GitHub enables team members to review, develop, and propose new codes. They can also discuss any implementation and proposals before changing the source code. 

4. **Unique code safety**:
GitHub is packed with dedicated tools to help individuals and teams identify and analyze vulnerabilities in the code that other tools tend to miss. Development teams everywhere can collaborate to secure the software supply chain from beginning to end.

5. **Effective team management**:
With GitHub, teams carry the same mindset, which makes them organized. Also, moderation tools, such as Issue and Pull Request Locking, help the team to focus on the code.

6. **Code hosting is easy**:
Code hosting is another area that shows how functional GitHub is. You have all the code and documentation in one place. With the millions of repositories on GitHub, you have various tools to help you host and release code.

8. **GitHub Actions**:
GitHub Actions is a versatile and powerful tool that allows developers to automate their workflows directly within GitHub repositories. It provides a wide range of functionalities, such as building, testing, and deploying code, making it an important part of any development process.

7. You can improve your team's productivity and efficiency by creating custom workflows and automating repetitive tasks with GitHub Actions. It supports a variety of programming languages and platforms, allowing you to seamlessly integrate your tech stack.

8. Create a new workflow file in your repository's ".github/workflows" directory to get started with GitHub Actions. In this file, you define the event that will initiate the workflow, the actions to be performed, and any necessary inputs and outputs.

Here are some workflow examples that show the power and versatility of GitHub Actions:

- **Build and Test Workflow**: When a new pull request is created, this workflow is triggered. It validates the code, installs dependencies, builds the code, runs unit tests, and generates a test report.
- **Deployment Workflow**: When a new release is published, this workflow is triggered. It validates the code, builds it, packages it into a Docker container, and deploys it to a cloud platform like AWS or Google Cloud.
- **Notification Workflow**: When a new issue is created, this workflow is triggered. It notifies the relevant team members of the new issue by sending a notification to a Slack channel or an email address.
  
These workflows are just a few examples of what GitHub Actions can do. You can create workflows that are tailored to your specific project and team needs thanks to its flexibility and customization options.

9. **GitHub Copilot**:
- GitHub Copilot is an artificial intelligence (AI) tool created by GitHub in collaboration with OpenAI, with the goal of revolutionizing the way developers write code. As you type, it uses machine learning algorithms to provide suggestions and auto-complete code.

- This new tool has the potential to change the way developers work by making high-quality code easier and faster to write. GitHub Copilot analyses your code and then uses machine learning models to predict and recommend code snippets that match your intent.

- Developers can save time and increase productivity by spending less time writing boilerplate code and more time focusing on the important aspects of their projects with GitHub Copilot. GitHub Copilot can also assist developers in learning new programming languages and libraries by making suggestions and providing examples based on existing code.

- However, as with any AI tool, there are privacy and security concerns. GitHub Copilot analyses code uploaded to GitHub, which raises concerns about the potential exposure of sensitive information. Furthermore, there are concerns about the potential for bias in GitHub Copilot's suggestions, as the machine learning models used to generate them are only as unbiased as the data used to train them.

10. **GitHub Pages** :
GitHub Pages is a free web hosting service that enables users to host static websites directly from their GitHub repositories. Developers can use GitHub Pages to create and publish websites without the need for a separate hosting service or domain name.

- To begin using GitHub Pages, you must first create a GitHub account and repository. Then, go to the repository settings, select the "Pages" tab, and select a source for your site to enable GitHub Pages on your repository (either the main branch or a specific folder).

- After you've enabled GitHub Pages, you can begin creating your website with HTML, CSS, and JavaScript. Static site generators, such as Jekyll, can also be used to speed up the website creation process.

- One of the most important advantages of GitHub Pages is its simplicity and ease of use. Developers can use GitHub Pages to create and host a website in minutes, without having to worry about the complexities of setting up a separate hosting service or domain name.

- It is important to note, however, that GitHub Pages is only intended for hosting static websites. You will need to use a different hosting service if your website requires dynamic content or server-side processing.

11. **GitHub CLI**:
GitHub CLI is a command-line interface tool that allows developers to interact with GitHub directly from the terminal. It provides a powerful set of features that can assist developers in more efficiently managing their GitHub repositories and workflows.

- GitHub CLI allows developers to create and clone repositories, create pull requests and issues, and merge changes from the command line. This can save time and increase productivity by allowing developers to complete tasks without switching between the terminal and the GitHub web interface.

- One of the most important advantages of GitHub CLI is its ability to help automate common tasks. GitHub CLI allows developers to create aliases for common commands, allowing them to complete tasks more quickly and efficiently.

The following are some examples of how to use GitHub CLI:

Creating a new repository:
<tab><tab><pre><code>gh repo create my-new-repo/repo</code></pre>

Cloning a repository:
##  
<tab><tab><pre><code>gh repo clone owner/repo</code></pre>

Creating a new issue:
<tab><tab><pre><code>gh issue create -t "Title of the issue" -b "Body of the issue"</code></pre>

Creating a new pull request:
tab><tab><pre><code>gh pr create -t "Title of the pull request" -b "Body of the pull request" -B main -H feature-branch</code></pre>

Merging a pull request:
<tab><tab><pre><code>gh pr merge 123 --merge</code></pre>


These are just a few examples of what GitHub CLI can do. With its powerful set of features and ability to automate common tasks, GitHub CLI can be a valuable tool for developers who want to manage their GitHub workflows more efficiently.

12. **GitHub Codespaces**:
GitHub Codespaces is a new cloud-based development environment that enables developers to write, review, and collaborate on code directly from their browsers. Developers can use GitHub Codespaces to create a fully functional development environment that is hosted in the cloud and accessible from anywhere, at any time.

With features like live sharing, real-time code editing, and integrated debugging, the platform is intended to make it easier for developers to collaborate on projects. Codespaces also integrate with other popular tools such as Visual Studio Code, Git, and GitHub Actions, making it easier for developers to continue working with their existing workflows.

One of the primary benefits of using GitHub Codespaces is the ability to quickly create a new development environment with a few clicks. Developers can use pre-configured environments or create their own custom environments based on their specific requirements. This allows them to concentrate on writing code rather than configuring development environments.

Developers can also collaborate on code in real-time using GitHub Codespaces. Developers can use the live sharing feature to invite others to join their Codespace and collaborate on code in real-time. This is especially useful when working on complex problems that require input from multiple developers.



## Getting Started
### Pre-requisites

| License Type | Description | Commercial use| Open Source|
| ---------- | ------- | --------- |------------|
| General Public License version 2.0   | Free and open for public use and modification. |  Yes|      Yes| 


## Software Overview

| Software | Version |
| --------------- | -------------- |
| github | 2.25.1 |


## System Requirement

| Requirement |	Minimum Recommendation |
| --------------- | -------------- |
| Processor/Instance Type |	One-Core/T2.micro instance |
|RAM|	1 Gigabyte |
|ROM(Disk Space)|	 8 Gigabyte or Higher|
|OS| Required	Linux(Ubuntu, CentOS, Red Hat Enterprise Linux (RHEL), and Debian)|


## Important Ports
| Ports|	Description|
| --------------- | -------------- |
|22	|Port 22 is used to establish an SSH connection to an EC2 instance and access a shell.
|443	|It is a standard port for secure communication over the internet between client and server.
| 80	|It is a standard port for  not secure communication over the internet between client and server.



## Installation

1. First, use the apt package management tools to update your local package index.

##  
<tab><tab><pre><code>sudo apt update</code></pre>

2. With the update complete, you can install Git:

##  
<tab><tab><pre><code>sudo apt install git</code></pre>

3. You can confirm that you have installed Git correctly by running the following command and checking that you receive relevant output.

##  
<tab><tab><pre><code>git --version</code></pre>

Output: `Output
git version 2.25.1`


## Contact Information
|Name	|Email address 📧|
| --------------- | -------------- |
|Nida khan|	[nida.khan.snaatak@mygurukulam.co](https://www.gmail.com/)|




## Reference
|Links	|Description|
| --------------- | -------------- |
|https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-20-04| github installation link |
|https://www.knowledgehut.com/blog/web-development/what-is-markdown| markdown reference points |

