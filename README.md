# IOCamlJS-static

A static build of [IOCamlJS](https://github.com/andrewray/iocamljs/tree/gh-pages), which is a list of Online OCaml Javascript REPLs.
They allow you to use the [OCaml](https://www.ocaml.org/) language, running on your browser (client-side, using Javascript), pretty much like [BetterOCaml](https://github.com/jbdo99/BetterOCaml/) (<https://BetterOCaml.ml>) but using the [IPython](https://www.ipython.org/) [notebook](https://jupyter.org/) interface from 2014.

**TL;DR:** I wanted to copy [this folder](https://andrewray.github.io/iocamljs/) <https://andrewray.github.io/iocamljs/> to <https://perso.crans.org/besson/publis/iocamljs/>, and so I did the following.

## How to obtain this?

Git clone [the repository](https://github.com/andrewray/iocamljs/), check out the [gh-pages](https://github.com/andrewray/iocamljs/tree/gh-pages) branch, then use [Jekyll](https://jekyllrb.com/) static website builder to compile the website:
```bash
git clone https://github.com/andrewray/iocamljs
git branch origin/gh-pages
jekyll build
```

The `_site/` folder is now ready to be sent to any folder on your website.

## How to deploy to your own website?
If you want this folder to be sent to `myserver.com/dest/folder/`, you have to change the `_config.yml` file from <https://github.com/andrewray/iocamljs/tree/gh-pages> to change the `root_path` key:

```yml
root_path: /dest/folder/
```

For instance, to deploy to <https://perso.crans.org/besson/publis/iocamljs/>, I had to use:
```yml
root_path: /besson/publis/iocamljs
```

## Where is this deployed on my own websites?

- Here on [`perso.crans.org/besson`](https://perso.crans.org/besson/) : <https://perso.crans.org/besson/publis/iocamljs/> ;
- Here on [`besson.link`](https://besson.link/) : <https://besson.link/publis/iocamljs/> ;
- And here on <http://iocamljs.besson.link> (an invisible mirror of the previous link, but not accessible by HTTPS).

## License and copyright?

This is NOT my property, it is the copyright of [@andrewray](https://github.com/andrewray/), released under the [MIT License](https://github.com/andrewray/iocamljs/blob/master/LICENSE).
