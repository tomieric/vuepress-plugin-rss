# Vuepress Plugin RSS

> RSS Plugin for Vuepress

## Install

```
> yarn add @tomieric/vuepress-plugin-rss@next -D
# or
> npm i @tomieric/vuepress-plugin-rss@next -D
```

Has been merged into [vuepress-plugin-rss](https://github.com/youngtailors/vuepress-plugin-rss)

## Config for your site

* Update your `.vuepress/config.js`
``` js
module.exports = {
    ...
    plugins: [
      ['@tomieric/vuepress-plugin-rss',
        {
          // base_url: '/', // required
          site_url: 'https://coralo.io', // required
          copyright: '2018 Coralo', // optional
          // filter some post
          filter: (frontmatter) => { return [true|false] },
          // How much articles
          count: 20
        }
      ]
    ]
}
```

## Contributors

- Core Plugin - [dacsang97](https://github.com/dacsang97)
- Support Vuepress 1.0 - [tomieric](https://github.com/tomieric)

---

License MIT