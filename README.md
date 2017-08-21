# Stripped Down Jekyll Starter Project

<img src="img/github-screenshot.png" height="auto" width="100%" alt="jekyll-starter">

## Oh no, not another theme… 🙄

Nope this isn't a theme! I've been exploring jekyll lately and a few things annoy me:

1. Starting a new project via `jekyll new [my-project-name]` gives me a starter theme that's way too bloated.
2. On the flip side, using `jekyll new [my-project-name] --blank` doesn't even give me a `config.yml` file.
3. In both cases, no livereload or autoprefixing out of the box.

You can think of this as the Goldilocks of starter projects and you can check it out here: [https://luclemo.github.io/jekyll-starter/](https://luclemo.github.io/jekyll-starter/)

### OMG it's so ugly! 😱

Yup. that's the point. Now go make it gorgeous.

## Features 🍬

This is _not_ a theme. It's just a directory with some good starter bits:

### A very basic file structure 📂

- I've included stuff nearly every project needs: a `404` and `about` page and useful config stuff.
- Blog structure and permalinks are a pain to set up so I've included it.  
Don't want/need a blog it? Just delete the `_posts` directory and `blog.md` file. Done. 

### Minimal styling 🎨

- A few SCSS variables (colors & fonts)
- A few handy mixins (like really, there are 3)
- A bunch of empty sass partials for organization. Use 'em or don't.

### Do I need Gulp … Grunt … PostCSS … la-la-la ? 👯

- Nope. If all you're after is livereload and autoprefixing, it just works out of the box. However, you can definitely add/replace with your tooling of choice.

## Getting started 🚦

**Assumptions before we get going:**

You will need some _very_ minimal command line abilities. You will also need to know what jekyll is and have it installed on your machine. A few good resources for each: [Command Line Power User](https://commandlinepoweruser.com/) and [Jekyll docs](https://jekyllrb.com/docs/home/).

### Let's get this project to your machine ⬇️

1. Move into directory of your choice:

    ```text
    cd path/to/directory-of-your-choice
    ```

2. Create the project inside that directory:

    ```text
    git clone https://github.com/luclemo/jekyll-starter.git
    ```

### Working locally 👩‍💻

Fire it up in your browser:

```text
jekyll serve --config _config.yml,_config_dev.yml
```

That's it! Just do your thing. Edit your CSS, add pages or posts, create layouts etc. Your browser will automatically reload to show you your changes.

## Ready to deploy? 🚀

### Edit these two values in `_config.yml`

You will only need to do this once:

1. If your site will be served from a subdirectory, add it here:

    ```text
    baseurl: "/sub-directory"
    ```  

    Otherwise leave a set of empty quotes:

    ```text
    baseurl: ""
    ```

2. The hostname & protocol for your site:

    ```text
    url: "https://yourdomain.com"
    ```


### Build step for production:

Rebuild your files in `_site` with your new productions details:

```text
jekyll build
```

### Getting it on your server

Just upload the content of `_site` directory via FTP or use GitHub Pages or whatever you want.

That's it you're done! 👏

## I have questions, complaints, high-fives…!

Ok. Shoot. Do it with an issue or a [tweet](https://twitter.com/luclemo) ✌️