# dot-ry.fi

## TODO
 - [ ] [Multilingual support](https://gohugo.io/content-management/multilingual/)
 - [ ] Membership form
 - [ ] Event calendar
 - [x] GitHub Actions workflow

## Development
### Prerequisites
Install [Hugo](https://gohugo.io/installation/). It is available in the package repositories of most distros under the name `hugo` (Arch, Fedora, Debian etc.).

### Local development
To run the site on your local computer, run the command `hugo server`. The site will be available at [http://localhost:1313/](http://localhost:1313/).

The site can be built by running the command `hugo` without any parameters. The site will be generated in `public/`.


### Templates
The site can be edited easily by modifying the HTML and Markdown template files. Hugo uses [Go’s templating language](https://gohugo.io/templates/introduction/).

#### File locations
* Building blocks such as head and nav are located in `layouts/partials`
* Index page content is in `layouts/index.html`
* Layouts for different page types are located in `layouts/_default`
* News feed items are located in `content/news`

### Adding new news items
Either run `hugo new news/example.md` or just add the file under `content/news` manually. Both Markdown and HTML are okay. 

Items in the newsfeed should have the following header:

    ---
    title: "Title here"
    date: 2023-08-14T20:17:36+03:00
    draft: false
    tags: ["define", "some", "categories", "here"]
    ---

The option `draft` specifies if the news item is shown on the website.

### Adding static pages
Just add a Markdown or HTML file to the `content` directory. It needs to have the following header (both md and HTML):

    ---
    title: "Put your title here"
    layout: staticpage
    ---

The page will be available at `/filename`.

### Navigation
Navigation bar items are defined in the main configuration file `config.toml`.

### Static files
Files such as CSS, JavaScript and images are stored in the `static` directory.

Example of using these files in templates:

    {{ $dotlogo := "dot_logo_white.png" | relURL }}
    <img src="{{ $dotlogo }}" alt="DOT ry logo" />

### Deployment
The site is hosted on GitHub Pages. There is a Github Actions workflow that updates the
site when there are new commits. After making modifications, just push to GitHub and the
site will update.
