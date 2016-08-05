# Easily

Light, minimalist and simple Bootstrap CSS style based on [Bootswatch](https://github.com/thomaspark/bootswatch).

## Usage

Download the `bootstrap.min.css` file associated with the easily theme and replace Bootstrap's default stylesheet. You must still include Bootstrap's JavaScript file to have functional dropdowns, modals, etc.

You can import a theme into your styles using either LESS:

```
@import "bootstrap/less/bootstrap.less";
@import "easily/variables.less";
@import "easily/bootswatch.less";
```

## Customization

Easily is open source and you’re welcome to modify this theme.

The theme consists of two LESS files. `variables.less`, which is included by default in Bootstrap, allows you to [customize settings](http://getbootstrap.com/customize/#less-variables). `bootswatch.less` introduces more extensive structural changes.

To building your theme:

1. Download the Bootswatch repository: `git clone https://github.com/thomaspark/bootswatch.git`

2. Install Bootswatch dependencies: `npm install`

3. Download the Easily repository inside `bootswatch/` root directory: `git clone https://github.com/noogen-projects/easily.git`

4. Modify Bootswatch `Gruntfile.js`: append `, easily:{}` in the end of `swatch: {` section.

5. Modify `variables.less` and `bootswatch.less` in the `easily/` theme directory.

6. In the `bootswatch/` root directory type `grunt swatch:easily` to build the CSS for the Easily theme. Or type `grunt swatch` to build them all at once. (For install `grunt` globally type `npm install -g grunt-cli`.)

7. You can run `grunt` in the `bootswatch/` root directory to start a server, watch for any changes to the LESS files, and automatically build a theme and reload it on change. Run `grunt server` for just the server, and `grunt watch` for just the watcher.

For additional information see [Bootswatch README](https://github.com/thomaspark/bootswatch/blob/gh-pages/README.md).