![](images/pawel-czerwinski-EIfU0IUqZw8-unsplash.jpg ':class=banner-image')

# Markdown Publishing with Docsify&#8288;&#8211;&#8288;This

An introduction to Markdown publishing using the open source [Docsify-This.net](https://docsify-this.net/) project.

## Markdown

### What is Markdown? 
Markdown is a syntax to format the display of content stored as plain text - similar but simpler than HTML formatting

### Why Markdown? 

* System-independent
* Text only format (perfect for version control)
* Separation of content vs. presentation
* Human-readable (i.e. more than HTML)
* Can also contain HTML snippets

### Markdown Examples

```
# Your H1 Text Here  
## Your H2 Text Here  

_your italic text here_  

**your bold text here**  

* your unordered list item here  

  1. your numbered (and indented) list item here   

[link title](www.google.com)  
```
Tip: To ensure a new paragraph after text in markdown, put two spaces after the end of the line

## Publishing with Markdown

* Markdown Converters
  * For example, [Pandoc](https://pandoc.org/)
* Markdown Static Site Builders
  * For example, [Jekyll](https://jekyllrb.com/)
* Markdown Dynamic Renderers
  * For example, [Docsify](https://docsify.js.org)

## Docsify-This

[Docsify-This](https://github.com/hibbitts-design/docsify-this) is an open source Web app, built using the [Docsify Open Publishing Kit](https://github.com/hibbitts-design/docsify-open-publishing-starter-kit), that can quickly display online Markdown files as web pages (i.e. no file uploads or build processes).   

_Being open source, you can also host your own Docsify-This instance, with the possibility of even a custom domain! No platform lock-in here._

### Example Docsify-This Usage Scenarios

* Publish your Markdown files as standalone web pages, with no website setup or build process required
* Visually style your standalone web pages using a point-and-click Web Page Builder
* Share existing GitHub-hosted Markdown files as standalone web pages, with an optional 'Edit this Page' link
* Seamlessly embed constraint-free Markdown/HTML, which you have authored, into other platforms (e.g. LMS or CMS)
* Reuse existing Markdown content by seamlessly embedding it within other platforms (e.g. LMS or CMS)
* Utilize the supported URL parameters when embedding content to match each destination platform better visually

### Docsify-This Web Page Builder

To use the Docsify-This **Web Page Builder** enter the URL for an online Markdown file and tap the ‘Publish as Standalone Web Page’ button. The Markdown file will then be rendered as a standalone Web page with it’s own URL that can then be copied and shared.

![Docsify-This Web Page Builder](images/docsify-this-web-page-builder.jpg ':class=image-75-border')  
_Figure 1. Docsify-This Web Page Builder_

### Example Docsify-This URL

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md
```

![Docsify-This Rendered Markdown File](images/docsify-this-rendered-markdown-file.jpg ':class=image-75-border')  
_Figure 2. Docsify-This Rendered Markdown File_

Docsify-This rendered Web pages are also perfect for embedding, with the ability to visually style Docsify-This pages to the destination platform.

### Docsify-This URL Editing

You can also render other Markdown files in the same repository by directly editing the Docsify-This URL parameter **homepage**, for example:

```html
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=anotherfile.md
```

### Docsify-This Web Page Appearance

#### URL Parameters

The visual appearance of any Markdown file displayed by Docsify-This can be altered by using the provided set of [URL Parameters](https://docsify-this.net/#/?id=page-appearance-url-parameters). For example, **font-family**, **font-size**, **link-color** and **line-height**   

```
https://docsify-this.net/?basePath=https://raw.githubusercontent.com/hibbitts-design/docsify-this-one-page-article/main&homepage=home.md&font-family=Open%20Sans,sans-serif
```

#### Markdown CSS Classes

If you can edit the Markdown file that is displayed by Docsify-This the visual appearance can be further altered by using a set of provided [Markdown CSS Classes](https://docsify-this.net/#/?id=supported-markdown-css-classes). For example:  

**button**  

[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')

```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=button')
```

**banner-image**  

![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-image')

```markdown
![UX - User Experience](images/12650723674_d5c85af332_k.jpg ':class=banner-image')
```

#### Custom Markdown CSS Classes

<style>
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
</style>

In addition to the Markdown CSS classes supported by Docsify-This, you can also define your own custom classes within your displayed Markdown files, for example:

[Custom CSS Class Button](# ':class=mybutton')

CSS in Markdown file:  
```css
<style>
.markdown-section .mybutton, .markdown-section .mybutton:hover {
  cursor: pointer;
  color: #CC0000;
  height: auto;
  display: inline-block;
  border: 2px solid #CC0000;
  border-radius: 4rem;
  margin: 2px 0px 2px 0px;
  padding: 8px 18px 8px 18px;
  line-height: 1.2rem;
  background-color: white;
  font-family: -apple-system, "Segoe UI", "Helvetica Neue", sans-serif;
  font-weight: bold;
  text-decoration: none;
}
</style>
```

Markdown:  
```markdown
[Required Reading Quiz due Jun 4th](https://canvas.sfu.ca/courses/44038/quizzes/166553 ':class=mybutton')
```

#### HTML Snippets

As supported by standard Markdown, HTML snippets can also be included (and mixed) within Markdown , for example:  

```html
<div class="row">
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
<div class="column">

Lorem ipsum dolor sit amet, consectetur adipiscing elit.

</div>
</div>
```

### Embedding Docsify-This Pages

#### Example Docsify-This iFrame HMTL

You can embed Docsify-This web pages using iFrames in almost any platform. URL parameters can also be used to match each destination platform better visually.

![Docsify-This iFrame](images/docsify-this-iframe.jpg ':class=image-75-border')  
_Figure 3. Docsify-This iFrame (within the Canvas LMS Homepage), for example https://canvas.sfu.ca/courses/76289_

```html
<p><iframe style="overflow: hidden; border: 0px #ffffff none; margin-top: -26px; background: #ffffff;" src="https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=home.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue,Helvetica,Arial,sans-serif&font-size=1&hide-credits=true" width="800px" height="950px" allowfullscreen="allowfullscreen"></iframe></p>
```

Many LMSs, including Canvas and Moodle, have the ability to link external web pages to their course navigation menus. For example, with the Canvas LMS you would use the [Redirect Tool](https://help.canvas.yale.edu/m/55452/l/914676-creating-a-custom-link-in-your-course-navigation-using-the-redirect-tool) to display Docsify-This web pages.

#### External URL

The URL of a Markdown file rendered by Docsify-This can be included inside of other systems.  

![Docsify-This Module](images/docsify-this-page.jpg ':class=image-75-border')  
_Figure 4. Docsify-This External URL within Canvas LMS (used with the Redirect Tool), for example https://canvas.sfu.ca/courses/76289/external_tools/36154_

```html
url=https://docsify-this.net/?basePath=https://raw.githubusercontent.com/paulhibbitts/cmpt-363-222-pages/main&homepage=resources.md&edit-link=https://github.com/paulhibbitts/cmpt-363-222-pages/blob/main/resources.md&font-family=Lato%20Extended,Lato,Helvetica%20Neue, Helvetica,Arial,sans-serif&font-size=1&hide-credits=true
```

With the CanvasLMS it is also possible to use an [external web page as content within a course Module](https://community.canvaslms.com/t5/Instructor-Guide/How-do-I-add-an-external-URL-as-a-module-item/ta-p/967).

![Docsify-This Canvas LMS Module](images/docsify-this-module.jpg ':class=image-75-border')  
_Figure 5. Docsify-This External URL (used as a Canvas LMS Module), for example https://canvas.sfu.ca/courses/76289/modules/items/2816273_

## Git and GitHub

### Git

Git is a free and open source distributed version control system,  originally created by Linus Torvalds in 2005 for development of the Linux kernel. 

#### Version Control

Version control supports the management of changes, called revisions, to files... especially useful for pure text files such as those used by Docsify-This.

![Local Version Control](images/local.png ':class=image-75')  
_Figure 6. Local Version Control (source: https://git-scm.com)_

#### Collaboration

As a distributed version control system, Git also support collaboration with multiple contributors.

![Distributed Version Control](images/distributed.png ':class=image-75-border')  
_Figure 7. Distributed Version Control (source: https://git-scm.com)_

### GitHub

GitHub is an online Git service, providing point-and-click means to create and manage Git repositories.

In addition to supporting the hosting of Git repositories, online editing of repository content such as Markdown files (using the filename extension .md) is also provided.

![GitHub Markdown File](images/github-markdown-file.jpg ':class=image-75-border')  
_Figure 8. GitHub Markdown File_

### GitHub Desktop
  
* Locally Store Git/GitHub Repositories  
* **Push** and **Pull** Repository Changes  

![GitHub Desktop](images/github-desktop-screenshot-mac.jpg ':class=image-75-border')  
_Figure 9. GitHub Desktop Mac (source: https://desktop.github.com)_

### Docsify-This + GitHub or Codeberg Markdown Files 

To fully leverage the benefits of version control, and potentially collaboration using an optional "Edit this Page" link, store your Docsify-This Markdown pages within a GitHub or Codeberg repository and optionally use an app such as GitHub Desktop to push/pull changes to your desktop.

### Setting up GitHub Desktop

1. Install GitHub Desktop (https://desktop.github.com)
1. Enter your GitHub credentials as prompted
1. Go to a GitHub repository web page, tap **< > Code** and then choose **Open with GitHub Desktop** OR go to a Codeberg repository web page, copy the HTTPS address, then in GitHub Desktop choose **File > Clone Repository** and paste the copied URL
1. Choose the location for your cloned repository and tap the **Clone** button

### Desktop Text Editors

Once your Docsify-This Markdown files are synced (i.e. cloned) to your desktop via GitHub Desktop you can then use the text editor of your choice, such as VSCode, Pulsar Beta (was Atom.io), Typora etc.

Using GitHub Desktop you can preview any changes and then commit those changes back to the repository. VSCode can also be used alone to both sync and editing files.

![Docsify-This + GitHub Markdown Files](images/docsify-this-github.jpg ':class=image-75-border')  
_Figure 10. Docsify-This + GitHub Markdown Files Workflow_

![Docsify-This + Webserver Markdown Files_](images/docsify-this-webserver.jpg ':class=image-75-border')  
_Figure 11. Docsify-This + Webserver Markdown Files_

## Additional Resources

* Markdown Format
  * [Markdown Guide](http://markdownguide.org)
  * [Markdown Cheatsheet](http://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* Creating and Editing Markdown on GitHub
  * [Quickstart for writing on GitHub](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github)
  * [Authoring With Markdown](https://ucsbcarpentry.github.io/2022-01-31-ucsb-webpub-online/02-markdown/)
* Markdown Desktop Editors
  * [VSCode](https://code.visualstudio.com/)
  * [Pulsar Beta (was Atom.io)](https://pulsar-edit.dev/)
  * [Typora](https://typora.io/)
* GitHub Desktop
  * [GitHub Desktop App](https://desktop.github.com/)
  * [An Introduction to Version Control Using GitHub Desktop](http://programminghistorian.org/en/lessons/retired/getting-started-with-github-desktop)
  * [Getting Started with Git and GitHub Desktop](https://www.codecademy.com/article/what-is-git-and-github-desktop)