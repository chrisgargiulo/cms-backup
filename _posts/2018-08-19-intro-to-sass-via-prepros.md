---
ID: 1945
post_title: Intro to SASS via Prepros
author: CMS
post_excerpt: ""
layout: post
permalink: >
  http://creativemedia.space/intro-to-sass-via-prepros/
published: true
post_date: 2018-08-19 17:28:34
---
<h3>Organizing Styles: Using SASS Partials for a Modular CSS Setup</h3>
How you choose to organize your styles can affect your efficiency as a front-end developer (how long it takes you to write code? how much code do you re-use from project to project? ), your ability to manage complex projects and work with others (how readable is your code? how easily can others understand it?), and how fast your site loads (how how much of that code is actually needed? do you always make time to refactor and optimize your code?).

This may not be a big concern for small static brochure sites, but as you work on larger, more complex projects with multiple designers/developers, style organization becomes essential. One solution is to separate your styles into smaller parts (partials) and then use a preprocessor (SASS) to compile the styles into one style.css.

There are several ways to learn SASS and multiple different approaches to setting up your projects and your CSS architecture, so below are a few different ways to go about it.
<div></div>

<hr>

<div></div>
<a href="https://github.com/kccnma/sassybase"><img src="https://camo.githubusercontent.com/95cbf2cfba163dbb2f8a34a79ec0b450a08de50d/68747470733a2f2f63726561746976656d656469612e73706163652f77702d636f6e74656e742f75706c6f6164732f7361737379626173652d686f6d652d646576696365732d766563746f722e706e67" alt="Sassy Base" data-canonical-src="https://creativemedia.space/wp-content/uploads/sassybase-home-devices-vector.png"></a>
<h3></h3>
<h2><a id="user-content-hands-on-activity-1-sassy-sitebase-from-scratch" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#hands-on-activity-1-sassy-sitebase-from-scratch" aria-hidden="true"></a>Hands-on Activity #1: Sassy Sitebase From Scratch</h2>
<h4><a id="user-content-outcomes" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#outcomes" aria-hidden="true"></a>Outcomes:</h4>
<ul>
 	<li>Spin up a local webserver from a dev environment (as opposed to using an IDE)</li>
 	<li>Auto-reload a browser whenever a file is saved without a manual refresh.</li>
 	<li>Auto-compile SASS (via a compiler/task manager that watches for changes)</li>
 	<li>Use SASS features to set up a modular style base for a small site (using SASS partials)</li>
</ul>
<h4><a id="user-content-steps" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#steps" aria-hidden="true"></a>Steps:</h4>
<ol>
 	<li><strong>Setup a local front-end web development environment to compile SASS.</strong>&nbsp;In this step, we will use a Prepros, a GUI-based front-end compiler. In another lesson, we will use Gulp.</li>
 	<li><strong>Establish a custom organizational file system</strong>&nbsp;using SASS partials that embrace best practices and strategies from popular CSS methodologies (e.g. SMACSS).</li>
 	<li><strong>Embrace Components</strong>&nbsp;by working on small, bite-sized pieces of code that will work together to form a larger, modular system consisting of multiple SASS partial files. The new SCSS files will embrace SASS features to improve the coding experience, such as variables and nesting.</li>
</ol>
<h4><a id="user-content-instructions" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#instructions" aria-hidden="true"></a>Instructions:</h4>
All instructions are embedded into the content of the "Sassy Base" site that you will be building (see the instuctions on the home page).
<ul>
 	<li>Sassy Base repo:&nbsp;<a href="https://github.com/kccnma/sassybase">https://github.com/kccnma/sassybase</a></li>
 	<li>Sassy base demo:&nbsp;<a href="https://kccnma.github.io/sassybase/" rel="nofollow">https://kccnma.github.io/sassybase/</a></li>
</ul>
Examples:
<ul>
 	<li>John Doe's 2018 Sassy Base:&nbsp;<a href="https://johndoenma.github.io/sassy-base/" rel="nofollow">https://johndoenma.github.io/sassy-base/</a></li>
</ul>
<div></div>

<hr>

<div></div>
<h2><a id="user-content-hands-on-activity-2-convert-a-static-site-to-a-sassy-site" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#hands-on-activity-2-convert-a-static-site-to-a-sassy-site" aria-hidden="true"></a>Hands-on Activity #2: Convert a Static Site to a Sassy Site</h2>
In this hands-on activity (initially done as an in-class exercise in 2018), we will code a simple, single page brochure site from scratch using a multi-file SASS development system (that ebraces SASS features such as variables, partials, and nesting) to auto-generate a single-file CSS site that is ready for production. The end product, a single “compiled” style.css file, will be minified and ready for production. The new "Sassy CSS" system (a scss folder with partials) and new workflow (using a local dev environment with a pre-processor) will provide a faster, more efficient way to write cleaner, more maintainable code&nbsp;that is re-usable and a more powerful, flexible way to export and deploy project styles.

In this hands-on activity (initially done as an in-class exercise in 2017), we will work backwards: using a stylesheet for a small brochure site, we will convert a single-file CSS system into an organized multi-file SASS system. The end product, a “compiled” style.css file, should be no different than it was in the beginning. However, the new organizational system (scss folder with partials) and new workflow (using a local dev environment) will provide a faster, more efficient way to write code, a cleaner, more maintainable code base that is re-usable, and a more powerful, flexible way to export and deploy project styles.
<h4><a id="user-content-outcomes-1" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#outcomes-1" aria-hidden="true"></a>Outcomes:</h4>
<ul>
 	<li>Spin up a local web server from a dev environment (as opposed to using an IDE)</li>
 	<li>Auto-reload a browser whenever a file is saved without a manual refresh.</li>
 	<li>Auto-compile SASS (via a compiler/task manager that watches for changes)</li>
 	<li>Use SASS features to set up a modular style base for a small site (using SASS partials)</li>
</ul>
<h4><a id="user-content-steps-1" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#steps-1" aria-hidden="true"></a>Steps:</h4>
<ol>
 	<li><strong>Setup a local front-end web development environment to compile SASS.</strong>&nbsp;In this step, we &nbsp;will use a Prepros, a GUI-based front-end compiler. In another lesson, we will use Gulp.</li>
 	<li><strong>Establish a custom organizational file system</strong>&nbsp;using SASS partials that embraces best practices and strategies from popular CSS methodologies (e.g. SMACSS).</li>
 	<li><strong>Convert the CSS to SASS</strong>&nbsp;by reverse engineering the original, singular CSS file and separating it into a modular system of multiple SASS partial files. The new SCSS files will embrace SASS features to improve the coding experience, such as variables and nesting.</li>
</ol>
<h3><a id="user-content-step-one" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#step-one" aria-hidden="true"></a>Step One</h3>
<a href="https://camo.githubusercontent.com/66d206fc7b72c824798dca0738f952f47f58953d/687474703a2f2f656761726769756c6f2e636f6d2f636d732f77702d636f6e74656e742f75706c6f6164732f323031372f30382f73697465626173652d73617373792d73746570312e676966" target="_blank" rel="noopener noreferrer"><img src="https://camo.githubusercontent.com/66d206fc7b72c824798dca0738f952f47f58953d/687474703a2f2f656761726769756c6f2e636f6d2f636d732f77702d636f6e74656e742f75706c6f6164732f323031372f30382f73697465626173652d73617373792d73746570312e676966" alt="" data-canonical-src="http://egargiulo.com/cms/wp-content/uploads/2017/08/sitebase-sassy-step1.gif"></a>
<h4><a id="user-content-download-starter-files" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#download-starter-files" aria-hidden="true"></a>Download Starter Files</h4>
<ol>
 	<li>You can start with your own static base (e.g. in a previous lesson, you might have already created a static "My Base 1.0" based on&nbsp;<a href="https://github.com/kccnma/sitebase1-static">Site Base 1.0</a>) that you already may have already created on your own. If not,&nbsp; you can download the provided&nbsp;<a href="https://github.com/kccnma/sitebase/blob/master/docs/versions/sitebase1.zip?raw=true">sitebase1.zip</a>&nbsp;or&nbsp;<a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-static-css.zip?raw=true">sitebase-static-css.zip&nbsp;</a>and expand it in a local folder on your computer</li>
 	<li>Rename the project folder to sitebase-sassy</li>
 	<li>Rename style.css to style-orig.css</li>
 	<li>Create a new folder named “scss”
<ul>
 	<li>Inside of scss, create a new file names style.scss
<ul>
 	<li>Add a $text-color variable and set the body color to the variable</li>
</ul>
</li>
</ul>
</li>
</ol>
<a href="https://camo.githubusercontent.com/cb0b52b409a0ef381ca4a263d21caeed75ceac34/687474703a2f2f656761726769756c6f2e636f6d2f636d732f77702d636f6e74656e742f75706c6f6164732f323031372f30382f73697465626173652d73617373792d73746570322e676966" target="_blank" rel="noopener noreferrer"><img src="https://camo.githubusercontent.com/cb0b52b409a0ef381ca4a263d21caeed75ceac34/687474703a2f2f656761726769756c6f2e636f6d2f636d732f77702d636f6e74656e742f75706c6f6164732f323031372f30382f73697465626173652d73617373792d73746570322e676966" alt="" data-canonical-src="http://egargiulo.com/cms/wp-content/uploads/2017/08/sitebase-sassy-step2.gif"></a>
<h4><a id="user-content-setup-a-local-environment-using-prepros" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#setup-a-local-environment-using-prepros" aria-hidden="true"></a>Setup a Local Environment using Prepros</h4>
<ol>
 	<li>Add sitebase-sassy project into prepros (drag &amp; drop folder)</li>
 	<li>Test sass compiling by editing style.scss
<ul>
 	<li>Ensure that a new style.css file is created and that the text turns red</li>
</ul>
</li>
 	<li>Use prepress “preview” to fire up a local web server</li>
</ol>
<h3><a id="user-content-step-two" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#step-two" aria-hidden="true"></a>Step Two</h3>
<h4><a id="user-content-create-sass-partials" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#create-sass-partials" aria-hidden="true"></a>Create SASS Partials</h4>
<ol>
 	<li>Inside of your scss folder, create a new folder named “partials”</li>
 	<li>In your editor, open up style-orig.css for reference (e.g. on the right)</li>
 	<li>Open up style.scss (e.g. on the left)</li>
 	<li>We are going to take css from the right and copy-paste it into new .scss files that we will create from scratch.</li>
</ol>
<h4><a id="user-content-link-sass-partials-via-import" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#link-sass-partials-via-import" aria-hidden="true"></a>Link SASS Partials via @import</h4>
<ul>
 	<li>Change the root stylesheet (style.scss) to import base (_base.scss)
<ul>
 	<li>@import "base";
<ul>
 	<li>Note: the @import statement does not include the underscore "_"</li>
</ul>
</li>
 	<li>optional: add site-specific comments after the base</li>
</ul>
</li>
 	<li>Create, then import all partials into "base"
<ul>
 	<li>Start by creating/adding variables (_variables.scss)</li>
 	<li>Then import it into base
<ul>
 	<li>@import "variables";</li>
</ul>
</li>
</ul>
</li>
 	<li>Order of files to create/add/import into base:
<ul>
 	<li>base.scss
<ol>
 	<li>@import "variables";</li>
 	<li>@import "partials/toc-base";</li>
 	<li>@import "partials/html5";</li>
 	<li>@import "partials/typography";</li>
 	<li>@import "partials/media";</li>
 	<li>@import "partials/components";</li>
 	<li>@import "partials/layout";</li>
 	<li>@import "partials/structure";</li>
 	<li>@import "partials/site-navigation";</li>
 	<li>@import "partials/site-navigation-togglenav";</li>
</ol>
</li>
</ul>
</li>
</ul>
In the end, your project folder look like this:
<pre><code> sitebase-sassy/ 
 └── css/
     ├── style.css (compiled/generated - OK to delete to test) 
 └── scss/
     ├── style.scss
     ├── _variables.scss
     ├── _base.scss
     ├── partials/
         ├── _toc-base.scss
         ├── _html5.scss
         ├── _typography.scss
         ├── _media.scss
         ├── _components.scss
         ├── _layout.scss
         ├── _structure.scss
         ├── _site-navigation.scss
         ├── _site-navigation-togglenav.scss </code></pre>
You can also reference the folder structure and list of partial SCSS files via the end/completed lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed</a></li>
</ul>
<h3><a id="user-content-step-three" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#step-three" aria-hidden="true"></a>Step Three</h3>
<h4><a id="user-content-copy--paste-from-css-to-scss" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#copy--paste-from-css-to-scss" aria-hidden="true"></a>Copy &amp; Paste from CSS to SCSS</h4>
<ol>
 	<li>Working from the top to the bottom, copy and paste css from style.css into the appropriate scss partial files.</li>
 	<li>As you copy and paste, convert the CSS to SCSS to embrace the following SASS features:
<ul>
 	<li>Variables: create new variables for any duplicate values</li>
 	<li>Nesting: nest and indent selectors when appropriate</li>
</ul>
</li>
 	<li>Test as you code</li>
</ol>
<h4><a id="user-content-customize" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#customize" aria-hidden="true"></a>Customize</h4>
When you are done, you are welcome to customize this base and make it your own. For example, if you saved your static version as "My Base 1.0" then consider naming this new base to "My Base 2.0" and uploading it to github for future reference. Here are two such repositories from John Doe:
<ul>
 	<li>John Doe's&nbsp;<a href="https://github.com/johndoenma/mybase1">My Base 1.0</a></li>
 	<li>John Doe's&nbsp;<a href="https://github.com/johndoenma/mybase2">My Base 2.0</a></li>
</ul>
<h4><a id="user-content-related-reading" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#related-reading" aria-hidden="true"></a>Related Reading</h4>
<ul>
 	<li><a href="http://thesassway.com/beginner/how-to-structure-a-sass-project" rel="nofollow">How to structure a Sass project</a></li>
 	<li><a href="https://smacss.com/" rel="nofollow">SMACSS: Scalable and Modular Architecture for CSS</a></li>
 	<li><a href="http://getbem.com/introduction/" rel="nofollow">BEM: Blocks, Elements and Modifiers</a></li>
</ul>
<h4><a id="user-content-lesson-resources" class="anchor" href="https://github.com/chrisgargiulo/creativemediaspace/blob/master/_posts/2018-08-19-intro-to-sass-via-prepros.md#lesson-resources" aria-hidden="true"></a>Lesson Resources:</h4>
<ul>
 	<li>Throughout this lesson, you can reference the start/beginning and end/completed lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-static-css">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-static-css</a></li>
 	<li><a href="https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed">https://github.com/kccnma/teachingmaterials/tree/master/sitebase-sassed</a></li>
</ul>
</li>
 	<li>You can also download the following archives (.zip files) of the lesson files here:
<ul>
 	<li><a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-static-css.zip?raw=true">sitebase-static-css.zip&nbsp;</a></li>
 	<li><a href="https://github.com/kccnma/teachingmaterials/blob/master/sitebase-sassed.zip?raw=true">sitebase-sassed.zip&nbsp;</a></li>
</ul>
</li>
</ul>