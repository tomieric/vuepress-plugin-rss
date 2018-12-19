# Vuepress Plugin RSS

> RSS Plugin for Vuepress

## Install

```
> yarn add vuepress-plugin-rss -D
# or
> npm i vuepress-plugin-rss -D
```

## Config for your site

* Update your `.vuepress/config.js`
``` js
module.exports = {
    ...
    plugins: [
      ['vuepress-plugin-rss',
        {
          // base: '/blog/', It's set to 'https://coralo.io/blog'
          site_url: 'https://coralo.io', // required
          copyright: '2018 Coralo', // optional
          // filter some post
          // filter : (page) => {}
          filter: ({ frontmatter }) => { return true },
          // How much articles
          count: 20
        }
      ]
    ]
}
```

License MIT