# One Fact website

This repository contains the Jekyll source for the redesigned One Fact website.

## Local preview

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

The current GitHub Pages project-site configuration uses `baseurl: /onefactinc`.
When the site is eventually moved to the `onefact.net` custom domain, update
`url` and set `baseurl: ""`, then add the appropriate `CNAME` file and
configure the domain in GitHub Pages.

The WordPress site and the existing static archive remain separate and untouched.
