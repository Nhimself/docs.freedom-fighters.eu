# Docs Readme

This page is published at [docs.freedom-fighters.eu](https://docs.freedom-fighters.eu/)

## Docsify - Framework that generates the docs

[docsify.js](https://docsify.js.org/#/)

[Github Repository](https://github.com/docsifyjs/docsify)

[Documentation](https://docsify.js.org/#/)

## Run Locally

`npm install` and then `npm start` while in root folder.

## Formatting documents

We use Prettier to format our code and Markdown files.

To format all files, do `npm run prettier`. For formatting on the fly in Visual Studio Code, please install the Prettier extension.

## Edit existing documentation

Open corresponding file in Github editor, make your changes, save and it will be commited to master

## Create new entry

Create new markdown file, current file structure corresponds to sidebar structure:

`Major Category(Folder) --- SubCategories (markdown files)`

`|`

`Major Category(Folder) --- SubCategories (markdown files)`

And add it to `_sidebar.md` to be shown in the sidebar. Identation represents hierarchy in the sidebar.

## Notes

- Headers in rendered markdown files are added to sidebar as subcategories. Maximum level is configurable in `index.html`, currently Max total level is set to 3 and max Sub level is set to 2, which means that only header 2 `##` will be added to sidebar. This can be overriden by 
  - adding ` {docsify-ignore}` at the end of a header to ignore it
  - ` {docsify-ignore-all}` to the first header in file to ignore all headers
  - nesting custom `_sidebar.md` https://docsify.js.org/#/more-pages?id=nested-sidebars
- The structure of the project can be changed, but after checking a few examples I found this structure to be cleanest
- Docsify supports a lot of customizations like:
  - [Cover pages](https://docsify.js.org/#/configuration?id=coverpage)
  - [Custom 404 pages](https://docsify.js.org/#/configuration?id=notfoundpage)
  - [Multiple language support](https://docsify.js.org/#/configuration?id=fallbacklanguages)
  - [Configuring markdown parser](https://docsify.js.org/#/markdown)
  - [Code Highlighting](https://docsify.js.org/#/language-highlight)
  - [Themes](https://docsify.js.org/#/themes)
  - [Various plugins](https://docsify.js.org/#/plugins)
