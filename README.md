# test-jekyll-github-actions

## About

Example set up using [jekyll-action](https://github.com/helaili/jekyll-action), a GitHub action that allows uploading a Jekyll website that uses other plugins not supported by GitHub Pages.

There are 2 branches:
- **main**: contains the Jekyll site code and the file `.github/workflows/jekyll.yml`, which calls the actions ([actions/checkout@v2 is also required](https://github.com/martinmorando/test-jekyll-github-actions/blob/147b0ea6fa72fdcd38ba26fb9a21584c9f2c728e/.github/workflows/jekyll.yml#L10)).
- **gh-pages**: the production site; its content is created automatically on every push to the main branch. The actions compile the code which is in the main branch.

The plugin **AsciiDoc** is [not supported by GitHub Pages](https://pages.github.com/versions/), however, in this way it is possible to use it. See this repository hosted on GitHub: https://martinmorando.github.io/test-jekyll-github-actions/ In this way it is possible to use many more useful plugins.


## Important

Remember to:
- Create a token under your repository Settings/Secrets. In this case is called ["TOKEN"](https://github.com/martinmorando/test-jekyll-github-actions/blob/02d0b6c2acb1cea4657e059b0941edb367863012/.github/workflows/jekyll.yml#L22).
- Under the repository Settings, select as source the branch "gh-pages".

## Note
This is just an example for future reference. The Jekyll Action was created by [Alain Hélaïli](https://github.com/helaili/jekyll-action).
