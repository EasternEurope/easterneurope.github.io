Eastern European Research Group
===============================

Site is running at: [easterneurope.github.io](http://easterneurope.github.io/)


Structure of the site
-------------------------------

All the content files are in root directory names *.md. Files are in markdown. Blog posts are in `_posts/` folder in markdown. css òf different themes are in `css` folder and it's subfolder. There are two layouts, `default.html` for pages and `post.html` for posts.

Developing through web
-------------------------------
You can make all edits through github-web interface. Once you commit the changes they will be displayed on the page immediately.


Blogging
-------------------------------

1. create new file with name `yyyy-mm-dd-some-name-here.markdown` including YAML-block in `_posts/` -folder. Easiest to copy-paste an existing blog post into new file and edit that
2. write text using [markdown-syntax]().
3. add images under `images`-folder and other files under `files`-folder.


----
----

# Some random instructions, not for maintainin EERG-website

## The easy way

The quickest way to put this into practise is to

1. for the repository
2. from **project settings** of forked project change the name of the repository from **digieast.github.io** into **youtusername.github.io**. This is enough to publish the website at **yourusername.github.io**.
3. Edit the following files to customize the page:
    1. `_config.yml`
    2. `_layout/default.html` (change the css path from **/css/main_flatly.css** to match some other css file in **/css-folder**
    3. edit `index.md`, `about.md`, `resources.md` etc. posts in the root directory
    4. add new blogposts into **_posts/** folder. (Follow the same naming scheme as the existing posts)
4. As you go with the edits check out the results at **yourusername.github.io**



## The hard way


### To run locally

1. fork the repository by hitting the **Fork**-button on the top right and pick your profile
1. clone the repository with `git clone git@github.com:username/digieast.github.io.git`
2. `cd digieast.github.io`
2. edit the content of .md files or create new ones
3. edit the links to pages & css files in `_layouts/default.html`
4. edit the _config.yml and change the baseurl to match your future repository. It may be `http://username.github.io/`
4. run `jekyll serve --watch --baseurl ''` to build the site locally and to react to your edits

### To run it in your username.github.io

Once your are happy with how it looks like:

1. create a new repository `username.github.io` at GitHub
2. reset the remote for your project `git remote set-url origin git@github.com:username/username.github.io.git`
3. add new files to git using `git add --all`
4. stage and commit the changes with `git commit -a -m "message comes here"`
5. push the first time `git push -u origin master`

### Update your remote site

1. add, remove, change files
2. add new files to git using `git add --all`
3. stage and commit the changes with `git commit -a -m "message comes here"`
4. push the committed change `git push`


License
-------------------------------


### The code

Made by [Thomas Park](http://thomaspark.me) Contact him at <a href="mailto:hello@thomaspark.me">hello@thomaspark.me</a>.

Code released under the [MIT License](https://github.com/thomaspark/bootswatch/blob/gh-pages/LICENSE)

Based on [Bootstrap](http://getbootstrap.com). Icons from [Font Awesome](http://fortawesome.github.io/Font-Awesome/). 

Web fonts from [Google](http://www.google.com/webfonts).


### Content

Content on folder `_posts` and files

- `events_impact.md`
- `events_media.md`
- `events_seminars.md`
- `home_blog.md`
- `home_blog_archive.md`
- `home_eastern_europe.md`
- `home_expertise.md`
- `index.md`
- `members_collaboration.md`
- `members_individual.md`
- `research_courses.md`
- `research_projects.md`
- `research_publications.md`

are copyright Eastern Europe Research Group
