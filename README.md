Blog website hosted with Hugo.  Currently uses the [hugo-PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme.

## Usage
Run website locally:
```
hugo server
```

Run website with draft posts published:
```
hugo server --buildDrafts
```

Create a new post:
```
hugo new posts/name-of-post.md
```

Publish site with new post.  Hugo creates the static site in `public/`.  This includes the HTML files, and assets such as images, CSS files, and JavaScript files.  This excludes draft, future and expired content.
```
hugo
```

## Blog Initialization Instructions
1. Create a new Hugo site
    
    `hugo new site "Bruce MacKenzie's Professional Blog"`

    To work with yaml intead of toml, add the flag `-f yml`

    This initializes a new Hugo site configured with a config.[toml|yaml] file.

2. Add the theme
    
    `git submodule add --depth=1 https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod`

3. Create a new post

    `hugo new posts/name-of-post.md`

    This creates `content/posts/` folders containing `name-of-post.md`.
