# test-jekyll-github-actions

## About

Example set up using [jekyll-action](https://github.com/helaili/jekyll-action), a GitHub action that allows uploading a Jekyll website that uses other plugins not supported by GitHub Pages.

There are 2 branches:
- **main**: the Jekyll site code and the file .github/workflows/jekyll.yml, which contains the actions (actions/checkout@v2 is required)
- **gh-pages**: the production site

The plugin **AsciiDoc** is [not supported by GitHub Pages](https://pages.github.com/versions/), however, in this way it is possible to use it.

## Important

Remember to:
- Create a token under your repository Settings/Secrets. In this case is called ["TOKEN"](https://github.com/martinmorando/test-jekyll-github-actions/blob/02d0b6c2acb1cea4657e059b0941edb367863012/.github/workflows/jekyll.yml#L22).
- Under the repository Settings, select as source the branch "gh-pages".

## Note
This is just an example for future reference. The Jekyll Action was created by [Alain Hélaïli](https://github.com/helaili/jekyll-action).
