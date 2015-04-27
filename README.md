# Media

The Media  object module is implementation of
[Nicole Sullivan](https://twitter.com/stubbornella)’s
<cite>media object</cite>—the poster child of OOCSS.

To find out where it all started, read [Nicole’s blog
post](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/).

## Dependencies

The `media` object depends on three other modules:

* [settings.defaults](https://github.com/treeframework/settings.defaults)
* [tools.functions](https://github.com/treeframework/tools.functions)
* [trump.clearfix](https://github.com/treeframework/trump.clearfix)

If you install the `media` object using Bower or npm, you will get these 
dependencies at the same time. If not using Bower or npm, please be sure to 
install and `@import` these dependencies in the relevant way.

## Instalation

You can install the `media` module via Bower, npm, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-media --save
```

### Install using npm:

```sh
$ npm install tree-media --save
```

Once installed, `@import` into your project in its Objects layer:

```scss
@import "bower_components/tree-media/object.media";
```

### Install via file download

The least recommended option for installation is to simply download
`_object.media.scss` into your project and `@import` it into your project in
its Objects layer.

## Usage

Basic usage of the `media` object uses the required classes:

```html
<div class="o-media">
    <img class="o-media__img" src="/path/to/image.png" alt="" />
    <div class="o-media__body">
        <p>Text-like content goes here.<p>
    </div>
</div>
```

The only valid children of the `.o-media` node are `.o-media__img` and
`.o-media__body`.

## Options

Other, optional classes can supplement the required base classes:

* `.o-media--flush`: remove the space between the image- and text-content.
* `.o-media--[tiny|small|large|huge]`: alter the spacing between the image- and
  text-content.
* `o-.media--rev`: reverse the horizontal rendered order of the image- and
  text-content.
* `.o-media--responsive`: a very basic responsive implementation of the media
  object. Pragmatic; far from perfect.

For example:

```html
<div class="o-media  o-media--flush  o-media--rev">
    <img class="o-media__img" src="/path/to/image.png" alt="" />
    <div class="o-media__body">
        <p>Text-like content goes here.</p>
    </div>
</div>
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
