<p align="center"><img src="https://socialify.git.ci/johnisadev/mjml-email-starter/image?description=1&amp;font=Inter&amp;logo=https%3A%2F%2Fdocumentation.mjml.io%2Fimages%2Flogo.png&amp;pattern=Overlapping%20Hexagons&amp;theme=Dark" alt="project-image"></p>

<div style="font-size: 34px; padding: 3%">

<h2 >Minimal starter template for using mjml with vscode</h2>
<hr />

* [MJML Docs](https://documentation.mjml.io/)
* [MJML CLI Docs](https://github.com/mjmlio/mjml/blob/master/packages/mjml-cli/README.md)

<h2 style="font-weight: bold;">Requirements</h2>

- Node
- npm
- vscode

vscode mjml extension highly recommended but not required: 
[mjml vscode extension (unofficial fork)](https://marketplace.visualstudio.com/items?itemName=DanielKnights.vscode-mjml)
<h2 style="font-weight: bold;">🧐 Features</h2>

Here're some of the project's best features:

- Hot reload development
- build .html file from .mjml
- "clean" git command deletes old build files to rebuild

<hr />

<h2 style="font-weight: bold">🛠️ Installation Steps:</h2>

<p>1. Create a new repo by using this as a template.</p>

<p align="center"><img src="https://i.ibb.co/zPMtWqM/readme-template.png" alt="use this repo as a template"></p>

<p>2. install all dependencies</p>

```
npm ci
```

<p>3. build a HTML file from mjml file.</p>

```
npm run build
```

<p>4. For hot reloading dev environment once an HTML file is built.</p>

```
npm run dev
```

<hr />

<h2>Scripts</h2>

<b>build</b>

```
npm run build
```
<div style="font-size: 16px;">

    Takes the "index.mjml" and builds and "index.html" file.

    Note: changing the name of the mjml input file and name of the
    HTML output can be configured under the build script in the package.json file.
</div>
<hr />

<b>build:watch</b>

```
npm run build:watch
```
<div style="font-size: 16px;">

    Same thing as build but constantly listens for updates

    Note: this handldes the "hot-reloading" for the HTML compilation. See the dev script for this and browser "hot-reloading" in parallel.
</div>
<hr />

<b>clean</b>

```
npm run clean
```
<div style="font-size: 16px;">

    will delete "index.html" and compressed folders generated from the build or compress script. 

</div>
<hr />

<b>compress</b>

```
npm run compress 
```
<div style="font-size: 16px;">

    Compresses the "img" folder.

</div>
<hr />

<b>deploy</b>

```
npm run deploy
```
<div style="font-size: 16px;">

    Runs clean, build, and compress commands in sequential order.

</div>
<hr />

<b>serve</b>

```
npm run serve
```
<div style="font-size: 16px;">

    displays "index.html" in a local live server with "hot-reloading". 

    Note: the default local server port is 3000
</div>
<hr />

<b>dev</b>

```
npm run dev
```
<div style="font-size: 16px;">

    Runs build:watch and serve commands in parallel. Will automatically re-compile the "index.html" and updated changes will display on local server.

    Note: The command will throw an error if no "index.html" exists. If you get this error, inspect if "index.html" exists and run the build command if neccessary.

</div>
<hr />

<h2>💻 Built with</h2>

Technologies used in the project:

- node
- mjml
- mjml-cli
- npm-run-all
- browser-sync

<h2>🛡️ License:</h2>

This project is licensed under the MIT

</div>
