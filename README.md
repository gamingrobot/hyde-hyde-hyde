# hyde-hyde-hyde

__`hyde-hyde-hyde`__ is a [Hugo](https://gohugo.io)'s theme inspired and derived from htr3n [hyde-hyde](https://github.com/htr3n/hyde-hyde)

## Changes

- Remove font awesome
- Remove Portfolio
- Use local fonts
- Remove social from sidebar
- Improved mobile sidebar
- Move copyright to bottom
- Remove comments
- Added search
- Center content
- Add better note shortcodes
- Add support for GoatCounter
- Use chroma instead of highlightjs

## Usage

### Installation

__`hyde-hyde-hyde`__ can be easily installed as many other Hugo themes:

```sh
$ cd HUGO_PROJECT

# then either clone hyde-hyde-hyde
$ git clone https://github.com/gamingrobot/hyde-hyde-hyde.git themes/hyde-hyde-hyde

# or just add hyde-hyde-hyde as a submodule
$ git submodule add https://github.com/gamingrobot/hyde-hyde-hyde.git themes/hyde-hyde-hyde
```

After that, choose `hyde-hyde-hyde` as the main theme.

* `config.toml` 

```toml
theme = "hyde-hyde-hyde"
```

That's all. You can render your site using `hugo` and see `hyde-hyde-hyde` in action.

### Options

__`hyde-hyde-hyde`__ essentially inherits most of Hyde's [options](https://github.com/spf13/hyde#options). There are some extra options though

*  `goatcounter = "your-goatcounter-site-code"`: Enables [GoatCounter](https://www.goatcounter.com/) analytics

*  `mermaid = true`: Enable mermaid.js diagrams
   * `mermaid_theme = "default"` Select a [mermaid.js theme](https://mermaid.js.org/config/theming.html)
   * `mermaid_align = "center"` Select an alignment for diagrams

* `postNavigation = true|false` (default `true`): Setting to `false` will disable the navigation _Previous Post_/ _Next Post_

* `relatedPosts = false|true` (default `false`): Setting to `true` allows related posts. Please refer [here](https://gohugo.io/content-management/related) for more details on related contents with Hugo.

*  `include_toc = false`: Setting to `false` in FrontMatter will disable too short TOC data as your want. 

* Search page, to use create [example search page](exampleSite/content/search.md)

### Customizations

* Most of the customizable SCSS styles in [_assets/scss/hyde-hyde_](assets/scss/hyde-hyde) and Hugo templates in [_hyde-hyde/layouts_](layouts) are modularized and can be altered/adapted easily.

### Posts in home page
By default hugo will show in your home page the most populated section.
This means that if you have more projects than posts, by default your home page will list your projects instead of your posts.
If you want to change this behaviour you can change the [mainsections](https://gohugo.io/functions/where/#mainsections).
For example, for the [exampleSite](https://github.com/htr3n/hyde-hyde-hyde/tree/master/exampleSite) this is how you should change the `config.toml` file:
```
[params]
    mainSections = ["posts"]
```

## Some Screenshots

### Main page

![hyde-hyde-hyde main screen](images/main.png)

### A post

![A post in hyde-hyde-hyde](images/post.png)

### Mobile

![mobile mode in hyde-hyde-hyde](images/mobile1.png)

![mobile mode in hyde-hyde-hyde](images/mobile2.png)

### Note Shortcodes

![note shortcodes in hyde-hyde-hyde](images/shortcodes.png)


## Author(s)

* Hyde-Hyde by [htr3n](https://github.com/htr3n)

* Original developed by [Mark Otto](https://github.com/mdo)

* Hugo's `hyde` ported by [Steve Francia](https://github.com/spf13)

## License

Open sourced under the [MIT license](LICENSE.md)

## Notes for rendering exampleSite

```
./hugo server --minify --source exampleSite/ --themesDir ../..
```