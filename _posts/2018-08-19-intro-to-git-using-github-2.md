---
ID: 1942
post_title: Intro to Git using Github
author: CMS
post_excerpt: ""
layout: post
permalink: >
  http://creativemedia.space/intro-to-git-using-github-2/
published: true
post_date: 2018-08-19 17:25:39
---
<!-- wp:heading {"level":3} -->
<h3>A Version Control Workflow</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>In this lesson, we will learn about&nbsp;<a href="https://git-scm.com/">Git</a>&nbsp;via a hands-on exercise using&nbsp;<a href="https://github.com/">Github</a><a href="https://github.com/">.</a></p>
<!-- /wp:paragraph -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>Git</strong>&nbsp;is a version control system for tracking changes in computer files and coordinating work on those files among multiple people.<br>–&nbsp;<a href="https://en.wikipedia.org/wiki/Git">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:quote -->
<blockquote class="wp-block-quote"><p><strong>GitHub</strong>&nbsp;is a web-based Git or version control repository and Internet hosting service. It is mostly used for code. It offers all of the distributed version control and source code management (SCM) functionality of Git as well as adding its own features. It provides access control and several collaboration features such as bug tracking, feature requests, task management, and wikis for every project.<br>–&nbsp;<a href="https://en.wikipedia.org/wiki/GitHub">Wikipedia</a></p></blockquote>
<!-- /wp:quote -->

<!-- wp:paragraph -->
<p>Git is a “distributed” version control system, where you keep your code in one place and are able to manage, track, and backup your code (e.g. using GitHub, a hosting platform that uses Git). It can be complex, especially when it comes to managing large projects with large teams. In this lesson, we are going to cover the basics specifically geared toward individual web designers, front-end developers and small teams working on small projects.</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#outcomes"></a>Outcomes:</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li>Learn the basics of Git and common git commands via CLI (Command Line Interface)</li><li>Learn how to install Git locally, setup your local environment, and create a new repository from scratch.</li><li>Learn a basic daily workflow of syncing a local repository with a remote repository on GitHub, editing it locally, and updating it.</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#lesson-resources"></a>Lesson Resources:</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="https://github.com/johndoenma/hello-world">Hello World</a>&nbsp;(a first repository, for learning purposes)</li></ul>
<!-- /wp:list -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#three-parts-of-this-lesson"></a>Three Parts of this Lesson:</h4>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol><li><strong>Installing Git</strong><br><em>Make sure that you have Git installed on your local machine</em></li><li><strong>Setting up a Repo</strong><br><em>Learn how to create repositories on Github from scratch (in the browser)</em></li><li><strong>Learning About Daily Git Workflows</strong><br><em>Understand the process of cloning, pulling, editing, commiting, and pushing using git via CLI. to remotely update an existing repository on Github</em></li></ol>
<!-- /wp:list -->

<!-- wp:image {"linkDestination":"custom"} -->
<figure class="wp-block-image"><a href="https://camo.githubusercontent.com/df0be9e99363eeaa74753a676abfd7d526f9a503/68747470733a2f2f696d67732e786b63642e636f6d2f636f6d6963732f6769745f32782e706e67" target="_blank" rel="noreferrer noopener"><img src="https://camo.githubusercontent.com/df0be9e99363eeaa74753a676abfd7d526f9a503/68747470733a2f2f696d67732e786b63642e636f6d2f636f6d6963732f6769745f32782e706e67" alt="Git Comic"/></a></figure>
<!-- /wp:image -->

<!-- wp:paragraph -->
<p>Git comic from&nbsp;<a href="https://xkcd.com/1597/">xkcd</a></p>
<!-- /wp:paragraph -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:heading -->
<h2><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#install-git"></a>Install Git</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Make sure that you have Git installed on your local machine</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Before you install anything, first check to see if you have it already installed. You can confirm via the following commands (to be entered via CLI, such as Terminal on a MAC or Command Prompt on a PC)</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git --version</code></pre>
<!-- /wp:code -->

<!-- wp:list {"ordered":true} -->
<ol><li>If you already have git installed, you can move on to PArt #2. If you do not have git installed, follow the&nbsp;<a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">installation instructions on the Git web site</a>.<ul><li>Another option: you can also download&nbsp;<a href="https://desktop.github.com/">GitHub Desktop</a>, a GUI client, that will automatically install git on your computer. However, I do not recommend using GitHub Desktop to learn Git. Instead, I recommend using the command line interface (CLI), which we will do in this lesson.</li></ul></li></ol>
<!-- /wp:list -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:heading -->
<h2><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#get-setup-on-github"></a>Get Setup on GitHub</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Create your first repository on Github from scratch</em></p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>Create an account at&nbsp;<a href="https://github.com/">Github.com</a>&nbsp;and log in.<ul><li>Note your user name</li><li>Note your user email address</li></ul></li><li>Configure your git username and email address to match your github account (e.g. if you are using github).</li></ul>
<!-- /wp:list -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>To test/ensure that your username and email configurations are correct:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git config --global user.name
$ git config --global user.email</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#create-your-repositories-on-githubcom-via-your-browser"></a>Create your repositories on Github.com via your browser</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>A&nbsp;<strong>repository</strong>&nbsp;is essentially a main project folder, designed to organize single projects. Each can contain multiple sub folders and files. All repositories should have a README, a default file for each repository with information about the project. GitHub makes it easy to add one whenever you create a new repository using your browser (via github.com). It also offers other common options such as adding a .gitignore file (which some beginners find challenging to create locally) along with license options. &nbsp;</p>
<!-- /wp:paragraph -->

<!-- wp:list {"ordered":true} -->
<ol><li>In the upper right corner, click + and then select "New Repository"</li><li>Name your repository whatever you want (e.g. “hello-world”)</li><li>Write a short description</li><li>Select Initialize this repository with a README</li><li>Optional: create a .gitignore file (this can always be edited or created later)</li></ol>
<!-- /wp:list -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:spacer -->
<div style="height:100px" aria-hidden="true" class="wp-block-spacer"></div>
<!-- /wp:spacer -->

<!-- wp:heading -->
<h2><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#daily-git-workflows"></a>Daily Git Workflows</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>Use Git (e.g. GitHub) as part of your daily practice</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Below are several different scenarios and processes for how you might use git as part of your daily workflow and what some of the more common commands might be.</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":3} -->
<h3><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#1-daily-workflow-for-a-new-project"></a>#1 Daily Workflow for a&nbsp;<strong>New</strong>&nbsp;Project</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>(if this is your first time working on locally, or you previously deleted your local folder and need to set it up again.)</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>NOTE:&nbsp;<em>This workflow assumes that you already have a repo created on Github and you now want to clone it locally to start editing it</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Via command line, navigate to your target parent directory (the folder where you will want to clone your github repo&nbsp;<em>into</em>)</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd targetparentdirectory</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>For example, some developers use the desktop and many found lessons will use the desktop for demo purposes. It doesn't matter where you choose to save your project folders because this is a personal choice. Plus, you can always move them later. For demo purposes, let's use the desktop.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd desktop</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Confirm that you are in the right place by listing the directory files/folders</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ ls -l // for Mac users
$ dir // for PC users</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Once you feel confident that you are in the correct place (e.g. the desktop), the next step is to clone the repo from GitHub. Clone the directory to your repo on GitHub (tip: copy/paste the url path to the repo via your browser, e.g.&nbsp;<a href="https://github.com/username/reponame/">https://github.com/username/reponame/</a>)</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git clone &lt;path-to-repository></code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Example:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git clone https://github.com/johndoenma/hello-world</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Once the repo is cloned to your local machine, you'll need to navigate into the project folder/directory</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd projectfolder</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Example:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd hello-world</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Once again, you can confirm that you are in the right place by listing the directory files/folders</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ ls -l // for Mac users
$ dir // for PC users</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Optional/additional confirmation: at any time you can double-check the status of your repo to see if your cloned local repo is up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You are set to begin editing! (e.g. edit the README.md file, add project folders or files, run gulp, edit/code, etc).</p>
<!-- /wp:paragraph -->

<!-- wp:list -->
<ul><li>For an initial "hello world" lesson (Your first Github repo), open your IDE (editor of choice) and edit the README.md file, then save it.</li><li>After you have made a change to your README.md file, move on the Daily Workflow steps below for&nbsp;<em>when you are done for the day</em>.</li></ul>
<!-- /wp:list -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":3} -->
<h3><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#2-daily-workflow-for-an-existing-project"></a>#2 Daily Workflow for an&nbsp;<strong>Existing</strong>&nbsp;Project</h3>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>(if you already have a project setup and worked on it locally before)</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Via command line, navigate to your a target parent directory</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ cd projectfolder</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>Check the status of your repo to see if your cloned local repo is up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If your local folder is up-to-date, then you are set to go! (e.g. edit files, run gulp, etc.)</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>If your local folder is not up-to-date, then you need to update your local repo to match the remote repo by "pulling" the latest version.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git pull</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>To confirm that your pull worked, you can double-check the status of your repo to see if your cloned local repo is now up-to-date</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>You are set to go! (e.g. edit files, run gulp, etc.)</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#3-daily-workflow-for-when-you-are-done-for-the-day"></a>#3 Daily Workflow for&nbsp;<strong>When You are Done for the Day</strong></h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p><em>(you should memorize these commonly used git commands)</em></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>When you are done editing for the day, the following are the most commonly used git commands for solo developers.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>First off, whenever you are done for the day, you should always check the status of your repo before you commit.</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git status</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If your local version is ahead of master (which it should be if you are a solo developer), then these three commands will be the most important ones to memorize:</p>
<!-- /wp:paragraph -->

<!-- wp:code -->
<pre class="wp-block-code"><code>$ git add -A
$ git commit -m “comment goes here”
$ git push origin master</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>If successful (e.g. no errors), you should be able to double-check by launching your browser and viewing your github.com repository to ensure that all recent updates/changes have been uploaded to github.com.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>NOTE: In recent years, code editors provide easy GUI-based workflows for version control, such as VS Code's built in support for git. Therefore some developers may not use the terminal always, especially when it can be done so quickly and easily without leaving their editor. Regardless, it is important to understand core git commands so that you understand what is happening under the hood when you commit and push your code to Github using a GUI. It will also come in handy when/if you ever run into errors or conflicts.</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>Congratulations, you are now up and running on GitHub!</p>
<!-- /wp:paragraph -->

<!-- wp:separator -->
<hr class="wp-block-separator"/>
<!-- /wp:separator -->

<!-- wp:heading {"level":3} -->
<h3><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#further-reading"></a>Further Reading</h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4><a href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-git-using-github-2.md#git-related-reading-and-learning-resources"></a>Git Related Reading and Learning Resources</h4>
<!-- /wp:heading -->

<!-- wp:list -->
<ul><li><a href="https://try.github.io/levels/1/challenges/1">GitHub's Interactive Learning Guide</a>&nbsp;(Intro to Git)</li><li><a href="https://guides.github.com/activities/hello-world/">GitHub's Hello World Guide</a>&nbsp;(Intro using Branching)</li><li><a href="https://help.github.com/">GitHub's Help Documentation</a></li><li><a href="https://www.youtube.com/githubguides">GitHub's Video Learning Guides</a></li><li><a href="https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf">GitHub's Cheat Sheet</a>&nbsp;(pdf)</li><li><a href="https://git-scm.com/docs">Git's Docs</a>&nbsp;(Cheat Sheet)</li><li><a href="https://www.atlassian.com/git">Atlassian's Getting Git Right</a>&nbsp;(Workflow Example)</li></ul>
<!-- /wp:list -->