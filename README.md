# Insomnia Documentation

Welcome to the open-source Insomnia documentation repository. Find the Insomnia documentation site at docs.insomnia.rest.

## Site overview and markdown styling

The Insomnia documentation site is built using [Jekyll](https://jekyllrb.com/), a static site generator and [Bootstrap 5](https://getbootstrap.com/docs/5.0/getting-started/introduction/). When updating content, navigate to:

* the `inso-cli` directory for Inso CLI documentation pages
* the `insomnia` directory for Insomnia (client) documentation pages

### Use Markdown instead of HTML

Stick to Markdown as much as possible in Markdown files. Use the following classes to style elements:

Element | Markdown class
------- | --------------
table | `{:.table .table-striped}`
note callout | `{:.alert .alert-primary}`

### Add a new page

Add a new page if you are adding documentation for a new topic. Don't add a new page for FAQ-type content. Take time to see where the content fits in. 

* Add the file to either the `inso-cli` or `insomnia` folder. 
* Name the file descriptively and use full words where possible. 
* Add the page title and local url to **_data** > **main-nav.yaml** under the corresponding section. 

### Keep it simple

* Don't add unnecessary and excessive packages. 
* Use screenshots very sparingly. And if you add a screenshot, ensure it has descriptive alt text and a short description underneath. See [Introduction to Insomnia](/insomnia/get-started) for an example.  

## Contributing resources

Insomnia is a [Kong](https://konghq.com/) product, and we follow the same Contributing Guidelines and Style Guide. Here's more information about becoming an effective contributor. 

* [Contributing Guidelines](https://docs.konghq.com/contributing/)
* [How to contribute to docs-as-code as a beginner](https://docs.konghq.com/contributing/community/#how-to-contribute-to-docs-as-code-as-a-beginner)
* [Community Expectations](https://docs.konghq.com/contributing/community-expectations/) regarding inclusive language and accessibility

## Run locally

1. Clone the repository. 
2. Run `cd docs`.
3. Run `bundle exec jekyll serve`.
4. Browse to http://localhost:4000.