# G.A.N.E webpage

The website is based on [GitHub pages](https://pages.github.com/) wich in turns uses the [Jekyll](https://jekyllrb.com/), a static website generator that transforms plain text files into static websites and blogs.

The website theme is based on [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)

## Local Development

While it is possible to edit the website directly from the GitHub web interface, it is recommended to first preview the changes in a local copy of the repository. 

To set up a local development environment, follow this steps:

1. Install [Docker](https://docs.docker.com/desktop/install/ubuntu/)

2. Clone this repository
```bash
git clone git@github.com:ganegroup/ganegroup.github.io.git
```

3. Start the docker container with the Jekyll development server
```bash
docker compose up
```

4. Navigate to http://0.0.0.0:4000 to preview changes


## Site structure

The site has two types of entries: pages and posts. Pages are largely standalone and static, used to communicate slow or permanent information. Posts, on the other hand are used to cummunicate transient or time-dependant information, like news. 

Pages are located in the `_pages` folder, while posts are located in the `_posts` folder

## Creating new pages

Pages are located in the `_pages` folder and can have any filename. You can add a [Front Matter](https://jekyllrb.com/docs/front-matter/) block with extra information such as title and layout

## Creating new blog entries

Blog entries are located in the `_posts` folder and their filename must use the following format: 

```
YEAR-MONTH-DAY-title.md
```

You can add a [Front Matter](https://jekyllrb.com/docs/front-matter/) block with extra information such as title, date, layout, category and tags

## Creating dual-language content

To create a translated entry create a file with the same filename as the original entry, but located under the `es/_pages` folder if it is a page or `es/_posts` if it is a post.



