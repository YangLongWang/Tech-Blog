# Tech-Blog

<details>
<summary>Table of Content</summary>

- [Overview](#overview)
  - [Description](#description)
  - [Usage](#usage)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
</details>

## Overview

### Description
A CMS-style blog site so that people can publish articles, blog posts, and any thoughts and opinions.

### Usage

The application will be deployed on Heroku, link: https://tech-blog-app-6408.herokuapp.com/

### The challenge

Users should be able to:

- login and logout the site
- create post
- update and delete posts posted by the user
- leave a comment for posts

### Screenshot

![](./assets/images/The%20Tech%20Blog%20-%201.png)
![](./assets/images/The%20Tech%20Blog%20-%202.png)
![](./assets/images/The%20Tech%20Blog%20-%203.png)
![](./assets/images/The%20Tech%20Blog%20-%204.png)
![](./assets/images/The%20Tech%20Blog%20-%205.png)
![](./assets/images/The%20Tech%20Blog%20-%206.png)

### Links

- Solution URL: [https://github.com/YangLongWang/Tech-Blog](https://github.com/YangLongWang/Tech-Blog)
- Deployed URL: [https://tech-blog-app-6408.herokuapp.com/](https://tech-blog-app-6408.herokuapp.com/)

## My process

### Built with

- Handlebars
- CSS
- JavaScript

### What I learned

- built handlebars and partials by myself

To see how I add code snippets, see below:

```Handlebars
<section>
  <h2>Your Dashboard</h2>
  {{#if posts.length}}
  <section>
    {{#each posts as |post|}}
    <article>
      {{> dashboard-post post}}
    </article>
    {{/each}}
  </section>
  {{/if}}
  <div class="add-post">
    <a href="/dashboard/create" class="edit-link row justify-content-center"><button class="btn-add-post">+ New Post</button></a>
  </div>
</section>

<div class="list-group">
  <a href="/dashboard/edit/{{id}}" class="post-header edit-link list-group-item">
    <h5 class="mb-1 title">{{title}}</h5>
    <small>
      Posted on {{format_date created_at}}
    </small>
  </a>
</div>
```
## Author

- Github - [Longyang Wang](https://github.com/YangLongWang)