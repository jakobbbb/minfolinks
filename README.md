# Medieninformatik-Links

A neat collection of links for my fellow Computer Science and Media
students at Bauhaus Universität Weimar.

The site is built using Jekyll and deployed with
[GitHub Pages](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll).

## Making changes to the links

The links themselves are read from `_data/records.json`.  Feel free to
make a PR if you notice any out of date or missing links.

## Building the website locally

You'll need to install `ruby` and `jekyll` on your system.  You can
usually get `ruby` from your distro's package manager, after which you
can install `jekyll` with `gem install jekyll`.

To run a local development server, start Jekyll with the following
command: `jekyll serve`.

## Deploying the website to GH Pages

To make this site available at
__https://jakobbbb.github.io/minfolinks__, the site was put into a
branch named `gh-pages` inside a repo named `minfolinks`.

When looking at the repo on
[GitHub](https://github.com/jakobbbb/minfolinks),
you should see *1 environment* in the *commits, branch, released, …*
bar.  Clicking that link lets you check the deployments, which should
happen after you push into the repo.
