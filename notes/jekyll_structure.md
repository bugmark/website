# Jekyll Structure

Based on [these specifications](https://github.com/bugmark/website/issues/3) and the [LoFi mockup](https://github.com/bugmark/website/issues/2), this structure was planned:

```shell
.
├── .editorconfig
├── .gitignore
├── CONTRIBUTING.md
├── _config.yml
├── _data
│   ├── api.yml
│   ├── authors.yml
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
├── _posts
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

## Data

To avoid repetition in the templates and accepts `.yml`, `.yaml`, `.json` or `.csv` formats and extensions.

`api.yml` - _(more info needed)._

`authors.yml` - for simple authoring. See also [posts and drafts](#posts-and-drafts).

`comparative.yml` - for comparison with other markets.

`testimonials.yml` - for testimonials from developers, investors and project managers.

## Posts and Drafts

Why not use the same structure to run the blog? As the intention is to use it only for infrequent updates and announcements, keep it in the same structure and if possible with the same visual identity of the site would be ideal. We can point the relative path as `/blog` in the same way as specified in issue [#6](https://github.com/bugmark/website/issues/6). Also, if we implement alternative ways to make a post, it will not be problem for authors unfamiliar with the Jekyll.

`_drafts` - drafts for unpublished posts.

`_posts` - blog posts.

`feed.xml` - RSS for blog posts.

## Docker Compose

For a quick and easy way to contribute with the repo using docker.

`docker-compose.yml` – with jekyll's official image optimized to work with gh-pages.

## Misc

`.editorconfig` - helps developers define and maintain consistent coding styles between different editors and IDEs.

`.gitignore` - for intentionally untracked files.

`CONTRIBUTING.md` - how to build and contribute with this repository.

`travis.yml` - for test and deploy.