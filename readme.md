# Knockout.Markdown

A binding for knockout 2.3+ to allow you to do convert markdown to html using the great [markdown-it](https://github.com/markdown-it/markdown-it) library.

## Installing

Add knockout-2.3.js (or newer versions) to your project, then markdown-it and finally knockout.markdown.js to your project..

## Example

A simple example of using markdown to generate outputs:
```
<div id="some-markdown-preview" data-bind="markdown: someObservableContainingMarkdown"></div>
```

### markdown binding

The binding takes an observable which should contain a markdown string,

### markdown extension

As markdown-it supports extensions there is a `ko.markdown` instance that you can override if you wish, this is what is used to power the underlying markdown parsing.
So you could do `ko.markdown =  markdownit().use(someOtherMarkdownPlugin, { withSome: args });` which would override the default markdown instance.

### More Examples with Source Code

Here is an example of what it does and how to use it.
[View Example](https://rawgithub.com/grofit/knockout.markdown/master/example.html)