<h1 align="center">
  Landon Rainwater LLP
</h1>

## ✨ Features

- MDX
- Fully customizable through the usage of Gatsby Themes (and Theme UI)
- Light Mode / Dark Mode
- Typography driven, minimal style
- Tags/Categories support
- Code highlighting with [prism-react-renderer](https://github.com/FormidableLabs/prism-react-renderer) and [react-live](https://github.com/FormidableLabs/react-live) support. Also allows adding line numbers, line highlighting, language tabs, and file titles.
- RSS Feed for blog posts
- Google Analytics Support
- SEO (Sitemap, OpenGraph tags, Twitter tags)
- Offline Support & WebApp Manifest

## 🚀 Getting Started

1. **Create a Gatsby site.**

Clone there repo to your local development directory

```sh
git clone https://github.com/amponce/landon-rainwater-llp
```

2. **Start developing.**

Navigate into project directory and start it up.

```sh
cd landon-rainwater-llp
gatsby develop
```

3. **Open the code and start customizing!**

Your site is now running at `http://localhost:8000`!

**Language tabs:**

When you add a language (such as e.g. `js` or `javascript`) to the code block, a little tab will appear at the top left corner.

````
```js
// code goes here
```
````

**Code titles:**

You can display a title (e.g. the file path) above the code block.

````
```jsx:title=your-title
// code goes here
```
````

Or without a specific language:

````
```:title=your-title
// code goes here
```
````

**Line highlighting:**

You can highlight single or multiple (or both) lines in a code block. You need to add a language.

````
```js {2,4-5}
const test = 3
const foo = 'bar'
const harry = 'potter'
const hermione = 'granger'
const ron = 'weasley'
```
````

**Hide line numbers:**

If you want to hide line numbers you can either globally disable them (see Theme options) or on a block-by-block basis. You can also combine that with the other attributes.

````
```noLineNumbers
// code goes here
```
````

**react-live:**

Add `react-live` to the code block (and render the component) to see a preview below it.

````
```js react-live
const onClick = () => {
  alert("You opened me");
};
render(<button onClick={onClick}>Alohomora!</button>);
```
````

### Adding content

#### Adding a new blog post

New blog posts will be shown on the index page (the three most recent ones) of this theme and on the blog overview page. They can be added by creating MDX files inside `content/posts`. General setup:

1. Create a new folder inside `content/posts`
1. Create a new `index.mdx` file, and add the frontmatter
1. Add images to the created folder (from step 1) you want to reference in your blog post
1. Reference an image as your `banner` in the frontmatter
1. Write your content below the frontmatter

**Frontmatter reference:**

```md
---
title: Has Coronavirus Unraveled American Business
date: 2020-11-12
tags:
  - Covid
  - Business
banner: ./defence-against-the-dark-arts.jpg
---
```

**The fields `description` and `banner` are optional!** If no description is provided, an excerpt of the blog post will be used. If no banner is provided, the default `siteImage` (from `siteMetadata`) is used.

The `date` field has to be written in the format `YYYY-MM-DD`!

#### Adding a new page

Additional pages can be created by placing MDX files inside `contents/pages`, e.g. an "About" or "Contact" page. You'll manually need to link to those pages, for example by adding them to the navigation (in `navigation` option of the theme). General instructions:

1. Create a new folder inside `content/pages`
1. Create a new `index.mdx` file, and add the frontmatter
1. Write your content below the frontmatter
1. Optionally add files/images to the folder you want to reference from the page

**Frontmatter reference:**

```md
---
title: About
slug: '/about'
---
```

### Change your `static` folder

The `static` folder contains the icons, social media images and robots.txt. Don't forget to change these files, too!

## 🎓 Learning Gatsby

Looking for more guidance? Full documentation for Gatsby lives [on Gatsby's website](https://www.gatsbyjs.org/).

### Themes

- To learn more about Gatsby themes specifically, we recommend checking out the [theme docs](https://www.gatsbyjs.org/docs/themes/).
