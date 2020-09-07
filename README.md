<div align="center">

<a href="https://www.jammeryhq.com" title="JammeryHQ" target="_blank">

  <img src="./jammeryhq.png" width="128" />
  
</a>

<p>
Fast-track your JAMstack development & learning
</p>
</div>

<hr />

# About this plugin

Gridsome remark plugin to embed external stuff into your gridsome site.

# Installation

```bash
npm install @jammeryhq/gridsome-plugin-remark-embed

# or

yarn add @jammeryhq/gridsome-plugin-remark-embed
```

## Key features

* Support for
  * Codepen
  * Code Sandbox
  * Facebook Post
  * Facebook Video
  * Giphy
  * Github Gist
  * JSFiddle
  * Soundcloud
  * Spotify
  * Twitter
  * Vimeo
  * Youtube
* Custom templates
* Configuable

# How to use

```js
//gridsome.config.js

module.exports = {
  plugins: [
    {
      use: '@gridsome/source-filesystem',
      options: {
        path: 'blog/**/*.md',
        route: '/blog/:year/:month/:day/:slug',
        remark: {
          plugins: [
            [ '@jammeryhq/gridsome-plugin-remark-embed', {
                'enabledProviders' : ['Youtube', 'Twitter', 'Gist'],
            }]
          ]
        }
      }
    }
  ]
}
```

# Documentation

You can find the complete documentation here: https://webstone.info/documentation/gridsome-plugin-remark-embed
