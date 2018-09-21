# Explaining HTML DOCTYPEs

## Problem Statement

Every web page in a browser is the rendered output of HTML that was requested
by a browser. The `DOCTYPE` tag tells our web browser which version of HTML
to use. HTML is a language that is still evolving, how do we declare the
`DOCTYPE` appropriately keeping accessibility and compatibility in mind?

## Objectives

1. Define the document type tag: `<DOCTYPE>`
2. Identify DOCTYPEs and its major releases

## Define The Document Type Tag: `<doctype>`

The special element proceeding the document structure is the `<!DOCTYPE>` tag.
The `DOCTYPE` tag defines the _entire_ HTML document. The HTML standard says that
all HTML documents begin with a "`DOCTYPE` declaration" tag. If one is missing, most
browsers pretend one is there and may load your page in "Quirks Mode", but you
should always be explicit and define it yourself.

The Doctype tells the browser the version of HTML that it should interpret the
document as. To use this standards mode, with cutting edge validation you state
`<!DOCTYPE html>` at the top of the document:

```html
<!DOCTYPE html>

```

```html
<!DOCTYPE html>
<html>
  <head>...</head>
  <body>...</body>
</html>
```

## Identify DOCTYPEs and its Major Releases

HTML5 is the latest evolution of the standard that defines HTML. It should ideally be
the default `DOCTYPE` being utilized to build modern-day websites and applications.
With this doctype, you can validate new features such as <video>, <canvas> and ARIA.

Older doctype declarations include HTML 4 Strict and HTML 4 Transitional.
The following `DOCTYPE`s have been commonly used in the past:

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
"http://www.w3.org/TR/html4/strict.dtd">
```
* **HTML 4.01 Strict** is a trimmed down version of HTML 4.01 that emphasizes structure over
presentation. Deprecated elements and attributes (including most presentational attributes),
frames, and link targets are not allowed in HTML 4 Strict. This doctype also triggers the
Standards mode, but lets you stick to less precise legacy validation that doesn’t know about
new features in case your organization has silly policies that require targeting legacy validation.
You ideally should be using <!DOCTYPE html> and get the policies of your organization revised.

```html
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"
"http://www.w3.org/TR/html4/loose.dtd">
```
* **HTML 4 Transitional** includes all elements and attributes of HTML 4 Strict but adds
presentational attributes, deprecated elements, and link targets. This would work if you'd
like to use the Standards mode, but the site in question uses sliced images in table layouts
and don’t want to/can't fix them. Layouts based on sliced images in tables are likely to break
if you later move to HTML5 (and, hence, the full Standards mode).

**XHTML doctypes are not recommended.**

## Conclusion

With this you now have the knowledge to craft your own, modern HTML documents. You should be
familiar with the concepts of `DOCTYPE`and tags. You may in rare cases encounter older DOCTYPEs,
but with these resources you will be empowered to build media-rich, highly-functional websites
with clean code in no time!

## Resources
[W3 HTML - <doctype> Tag](https://www.tutorialspoint.com/html/html_doctype_tag.htm)
[HTML DOCTYPEs](https://www.tutorialrepublic.com/html-tutorial/html-doctypes.php)
[Choosing DOCTYPEs](https://hsivonen.fi/doctype/#choosing)