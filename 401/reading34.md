# React IV

## Reading

### Next.js - Dynamic Routes

[Source](https://nextjs.org/learn/basics/dynamic-routes)

"Page path depends on external data. You can pre-render pages with paths that depend on external data."

How to statically generate pages with dynamic routes

- Each post needs the path `/posts/<id>`

  - `<id>` - markdown file name from `posts` directory

**Steps Overview:**

Create a page called `[id].js` under `pages/posts`

- dynamic routes are pages beginning and ending with `[]`

Write code that renders a post page

Export an async function, `getStaticPaths`

- return a list of possible values for id

- list needs to be an array of objects

- each object needs `params` key and to contain it's own object with the `id` key

- import `getAllPostIds` function to use inside `getStaticPaths`

- reading contains code to copy

Implement `getStaticProps` and give `params` to fetch necessary data

**Dynamic Routes Details:**

In development, `getStaticPaths` runs on every request

In production, `getStaticPaths` runs at build time

Fallback

- When fallback is false, any path not returned by `getStaticPaths` results in a 404 page

- When fallback is true, `getStaticProps` behavior changes

Adding three dots to the dynamic route brackets will catch all paths/routes `[...id]`

Custom 404 page file can be created with `pages/404.js`

### Next.js - Deployment

[Source](https://nextjs.org/learn/basics/deploying-nextjs-app)

Push to Github

Deploy to Vercel

- Create Vercel account

- give access to repositories

Next.js app will start building when you deploy

When complete, deployment URLs will be given

---

## Videos

### Next.js 10 is here

[Source](https://www.youtube.com/watch?v=JWCS5IdECVI)

---

## Bookmark and Review

### Next.js - Static File Serving

[Source](https://nextjs.org/docs/basic-features/static-file-serving)

---

</br>

[<<<Back](README.md)
