# Cyrus' Curious Blog

Here's the repo for my static website which uses [Hugo](https://gohugo.io/) the [Clarity theme](https://themes.gohugo.io/themes/hugo-clarity/) 

Compilation is simple, after navigating to directory with the repo simply run
```
hugo server
```

Then browse to [http://locahost:1313](http://localhost:1313) to view the site

# New Posts
To create a new post, use the command below and then make sure to update the meta-data at the top of the file.  Remove the `draft: true` line to have the 
post show up on the site.

```
hugo new --kind post YYYY/MM/slug-for-your-new-article.md
```
Make sure to include the `YYYY` value in the `config\_default\params.toml` element called `mainSections`.