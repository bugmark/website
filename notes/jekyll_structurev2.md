This is the proof of concept for incorporating blocks of Markdown text into the website, as discussed previously:

I've included a _pages directory in the Jekyll structure, which has the following markdown files.

- 01_developer.md
- 02_investorandprojectmanager.md
- 03_mainpage.md
- 04_blog.md
- 05_docs.md

These can be easily edited by everyone with Markdown. The changes in the content are reflected in the index.html of each Markdown, in _site dir. I've also added a _blog directory for editing the blog posts in Markdown.
To accommodate these I've changed the Jekyll structure to the following:
```shell
.
├── .editorconfig
├── .gitignore
├── CONTRIBUTING.md
├── _config.yml
├── _data
│   ├── api.yml
│   ├── comparative.yml
│   └── testimonials.yml
├── _drafts
├── _includes
│   ├── footer.html
│   ├── head.html
│   └── navbar.html
├── _layouts
│   ├── default.html
│   ├── page.html
│   └── post.html
├── _site
│   ├── developer
│       └── index.html
│   ├──  investorandprojectmanager
│       └── index.html
│   ├──  mainpage
│       └── index.html
│   ├──  blog
│       └── index.html
│   └── docs
│       └── index.html
├── _pages
│   ├──  01_developer.md
│   ├──  02_investorandprojectmanager.md
│   ├──  03_mainpage.md
│   ├──  04_blog.md
│   └──  05_docs.md
├── _blog
│   └──  index.html
├── _posts
│   └──  blogpost.markdown
├── _sass
├── assets
│   ├── css
│   ├── fonts
│   ├── images
│   ├── js
│   └── vendor
│       └── bootstrap
├── docker-compose.yml
├── feed.xml
├── index.html
└── travis.yml
```

A quick guide on how to write text in Markdown effectively can be found here:
https://blog.ghost.org/markdown/
