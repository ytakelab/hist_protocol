<!DOCTYPE html>
<html>
  <head>
      <meta charset="utf-8" />
      <title>Markdown to HTML</title>
      <style>.markdown-preview:not([data-use-github-style]) { padding: 2em; font-size: 1.2em; color: rgb(171, 178, 191); background-color: rgb(40, 44, 52); overflow: auto; }
.markdown-preview:not([data-use-github-style]) > :first-child { margin-top: 0px; }
.markdown-preview:not([data-use-github-style]) h1, .markdown-preview:not([data-use-github-style]) h2, .markdown-preview:not([data-use-github-style]) h3, .markdown-preview:not([data-use-github-style]) h4, .markdown-preview:not([data-use-github-style]) h5, .markdown-preview:not([data-use-github-style]) h6 { line-height: 1.2; margin-top: 1.5em; margin-bottom: 0.5em; color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) h1 { font-size: 2.4em; font-weight: 300; }
.markdown-preview:not([data-use-github-style]) h2 { font-size: 1.8em; font-weight: 400; }
.markdown-preview:not([data-use-github-style]) h3 { font-size: 1.5em; font-weight: 500; }
.markdown-preview:not([data-use-github-style]) h4 { font-size: 1.2em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) h5 { font-size: 1.1em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) h6 { font-size: 1em; font-weight: 600; }
.markdown-preview:not([data-use-github-style]) strong { color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) del { color: rgb(124, 135, 156); }
.markdown-preview:not([data-use-github-style]) a, .markdown-preview:not([data-use-github-style]) a code { color: rgb(82, 139, 255); }
.markdown-preview:not([data-use-github-style]) img { max-width: 100%; }
.markdown-preview:not([data-use-github-style]) > p { margin-top: 0px; margin-bottom: 1.5em; }
.markdown-preview:not([data-use-github-style]) > ul, .markdown-preview:not([data-use-github-style]) > ol { margin-bottom: 1.5em; }
.markdown-preview:not([data-use-github-style]) blockquote { margin: 1.5em 0px; font-size: inherit; color: rgb(124, 135, 156); border-color: rgb(75, 83, 98); border-width: 4px; }
.markdown-preview:not([data-use-github-style]) hr { margin: 3em 0px; border-top: 2px dashed rgb(75, 83, 98); background: none; }
.markdown-preview:not([data-use-github-style]) table { margin: 1.5em 0px; }
.markdown-preview:not([data-use-github-style]) th { color: rgb(255, 255, 255); }
.markdown-preview:not([data-use-github-style]) th, .markdown-preview:not([data-use-github-style]) td { padding: 0.66em 1em; border: 1px solid rgb(75, 83, 98); }
.markdown-preview:not([data-use-github-style]) code { color: rgb(255, 255, 255); background-color: rgb(58, 63, 75); }
.markdown-preview:not([data-use-github-style]) pre.editor-colors { margin: 1.5em 0px; padding: 1em; font-size: 0.92em; border-radius: 3px; background-color: rgb(49, 54, 63); }
.markdown-preview:not([data-use-github-style]) kbd { color: rgb(255, 255, 255); border-width: 1px 1px 2px; border-style: solid; border-color: rgb(75, 83, 98) rgb(75, 83, 98) rgb(62, 68, 81); border-image: initial; background-color: rgb(58, 63, 75); }
.markdown-preview[data-use-github-style] { font-family: "Helvetica Neue", Helvetica, "Segoe UI", Arial, freesans, sans-serif; line-height: 1.6; overflow-wrap: break-word; padding: 30px; font-size: 16px; color: rgb(51, 51, 51); background-color: rgb(255, 255, 255); overflow: scroll; }
.markdown-preview[data-use-github-style] > :first-child { margin-top: 0px !important; }
.markdown-preview[data-use-github-style] > :last-child { margin-bottom: 0px !important; }
.markdown-preview[data-use-github-style] a:not([href]) { color: inherit; text-decoration: none; }
.markdown-preview[data-use-github-style] .absent { color: rgb(204, 0, 0); }
.markdown-preview[data-use-github-style] .anchor { position: absolute; top: 0px; left: 0px; display: block; padding-right: 6px; padding-left: 30px; margin-left: -30px; }
.markdown-preview[data-use-github-style] .anchor:focus { outline: none; }
.markdown-preview[data-use-github-style] h1, .markdown-preview[data-use-github-style] h2, .markdown-preview[data-use-github-style] h3, .markdown-preview[data-use-github-style] h4, .markdown-preview[data-use-github-style] h5, .markdown-preview[data-use-github-style] h6 { position: relative; margin-top: 1em; margin-bottom: 16px; font-weight: bold; line-height: 1.4; }
.markdown-preview[data-use-github-style] h1 .octicon-link, .markdown-preview[data-use-github-style] h2 .octicon-link, .markdown-preview[data-use-github-style] h3 .octicon-link, .markdown-preview[data-use-github-style] h4 .octicon-link, .markdown-preview[data-use-github-style] h5 .octicon-link, .markdown-preview[data-use-github-style] h6 .octicon-link { display: none; color: rgb(0, 0, 0); vertical-align: middle; }
.markdown-preview[data-use-github-style] h1:hover .anchor, .markdown-preview[data-use-github-style] h2:hover .anchor, .markdown-preview[data-use-github-style] h3:hover .anchor, .markdown-preview[data-use-github-style] h4:hover .anchor, .markdown-preview[data-use-github-style] h5:hover .anchor, .markdown-preview[data-use-github-style] h6:hover .anchor { padding-left: 8px; margin-left: -30px; text-decoration: none; }
.markdown-preview[data-use-github-style] h1:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h2:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h3:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h4:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h5:hover .anchor .octicon-link, .markdown-preview[data-use-github-style] h6:hover .anchor .octicon-link { display: inline-block; }
.markdown-preview[data-use-github-style] h1 tt, .markdown-preview[data-use-github-style] h2 tt, .markdown-preview[data-use-github-style] h3 tt, .markdown-preview[data-use-github-style] h4 tt, .markdown-preview[data-use-github-style] h5 tt, .markdown-preview[data-use-github-style] h6 tt, .markdown-preview[data-use-github-style] h1 code, .markdown-preview[data-use-github-style] h2 code, .markdown-preview[data-use-github-style] h3 code, .markdown-preview[data-use-github-style] h4 code, .markdown-preview[data-use-github-style] h5 code, .markdown-preview[data-use-github-style] h6 code { font-size: inherit; }
.markdown-preview[data-use-github-style] h1 { padding-bottom: 0.3em; font-size: 2.25em; line-height: 1.2; border-bottom: 1px solid rgb(238, 238, 238); }
.markdown-preview[data-use-github-style] h1 .anchor { line-height: 1; }
.markdown-preview[data-use-github-style] h2 { padding-bottom: 0.3em; font-size: 1.75em; line-height: 1.225; border-bottom: 1px solid rgb(238, 238, 238); }
.markdown-preview[data-use-github-style] h2 .anchor { line-height: 1; }
.markdown-preview[data-use-github-style] h3 { font-size: 1.5em; line-height: 1.43; }
.markdown-preview[data-use-github-style] h3 .anchor { line-height: 1.2; }
.markdown-preview[data-use-github-style] h4 { font-size: 1.25em; }
.markdown-preview[data-use-github-style] h4 .anchor { line-height: 1.2; }
.markdown-preview[data-use-github-style] h5 { font-size: 1em; }
.markdown-preview[data-use-github-style] h5 .anchor { line-height: 1.1; }
.markdown-preview[data-use-github-style] h6 { font-size: 1em; color: rgb(119, 119, 119); }
.markdown-preview[data-use-github-style] h6 .anchor { line-height: 1.1; }
.markdown-preview[data-use-github-style] p, .markdown-preview[data-use-github-style] blockquote, .markdown-preview[data-use-github-style] ul, .markdown-preview[data-use-github-style] ol, .markdown-preview[data-use-github-style] dl, .markdown-preview[data-use-github-style] table, .markdown-preview[data-use-github-style] pre { margin-top: 0px; margin-bottom: 16px; }
.markdown-preview[data-use-github-style] hr { height: 4px; padding: 0px; margin: 16px 0px; background-color: rgb(231, 231, 231); border: 0px none; }
.markdown-preview[data-use-github-style] ul, .markdown-preview[data-use-github-style] ol { padding-left: 2em; }
.markdown-preview[data-use-github-style] ul.no-list, .markdown-preview[data-use-github-style] ol.no-list { padding: 0px; list-style-type: none; }
.markdown-preview[data-use-github-style] ul ul, .markdown-preview[data-use-github-style] ul ol, .markdown-preview[data-use-github-style] ol ol, .markdown-preview[data-use-github-style] ol ul { margin-top: 0px; margin-bottom: 0px; }
.markdown-preview[data-use-github-style] li > p { margin-top: 16px; }
.markdown-preview[data-use-github-style] dl { padding: 0px; }
.markdown-preview[data-use-github-style] dl dt { padding: 0px; margin-top: 16px; font-size: 1em; font-style: italic; font-weight: bold; }
.markdown-preview[data-use-github-style] dl dd { padding: 0px 16px; margin-bottom: 16px; }
.markdown-preview[data-use-github-style] blockquote { padding: 0px 15px; color: rgb(119, 119, 119); border-left: 4px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] blockquote > :first-child { margin-top: 0px; }
.markdown-preview[data-use-github-style] blockquote > :last-child { margin-bottom: 0px; }
.markdown-preview[data-use-github-style] table { display: block; width: 100%; overflow: auto; word-break: keep-all; }
.markdown-preview[data-use-github-style] table th { font-weight: bold; }
.markdown-preview[data-use-github-style] table th, .markdown-preview[data-use-github-style] table td { padding: 6px 13px; border: 1px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] table tr { background-color: rgb(255, 255, 255); border-top: 1px solid rgb(204, 204, 204); }
.markdown-preview[data-use-github-style] table tr:nth-child(2n) { background-color: rgb(248, 248, 248); }
.markdown-preview[data-use-github-style] img { max-width: 100%; box-sizing: border-box; }
.markdown-preview[data-use-github-style] .emoji { max-width: none; }
.markdown-preview[data-use-github-style] span.frame { display: block; overflow: hidden; }
.markdown-preview[data-use-github-style] span.frame > span { display: block; float: left; width: auto; padding: 7px; margin: 13px 0px 0px; overflow: hidden; border: 1px solid rgb(221, 221, 221); }
.markdown-preview[data-use-github-style] span.frame span img { display: block; float: left; }
.markdown-preview[data-use-github-style] span.frame span span { display: block; padding: 5px 0px 0px; clear: both; color: rgb(51, 51, 51); }
.markdown-preview[data-use-github-style] span.align-center { display: block; overflow: hidden; clear: both; }
.markdown-preview[data-use-github-style] span.align-center > span { display: block; margin: 13px auto 0px; overflow: hidden; text-align: center; }
.markdown-preview[data-use-github-style] span.align-center span img { margin: 0px auto; text-align: center; }
.markdown-preview[data-use-github-style] span.align-right { display: block; overflow: hidden; clear: both; }
.markdown-preview[data-use-github-style] span.align-right > span { display: block; margin: 13px 0px 0px; overflow: hidden; text-align: right; }
.markdown-preview[data-use-github-style] span.align-right span img { margin: 0px; text-align: right; }
.markdown-preview[data-use-github-style] span.float-left { display: block; float: left; margin-right: 13px; overflow: hidden; }
.markdown-preview[data-use-github-style] span.float-left span { margin: 13px 0px 0px; }
.markdown-preview[data-use-github-style] span.float-right { display: block; float: right; margin-left: 13px; overflow: hidden; }
.markdown-preview[data-use-github-style] span.float-right > span { display: block; margin: 13px auto 0px; overflow: hidden; text-align: right; }
.markdown-preview[data-use-github-style] code, .markdown-preview[data-use-github-style] tt { padding: 0.2em 0px; margin: 0px; font-size: 85%; background-color: rgba(0, 0, 0, 0.04); border-radius: 3px; }
.markdown-preview[data-use-github-style] code::before, .markdown-preview[data-use-github-style] tt::before, .markdown-preview[data-use-github-style] code::after, .markdown-preview[data-use-github-style] tt::after { letter-spacing: -0.2em; content: " "; }
.markdown-preview[data-use-github-style] code br, .markdown-preview[data-use-github-style] tt br { display: none; }
.markdown-preview[data-use-github-style] del code { text-decoration: inherit; }
.markdown-preview[data-use-github-style] pre > code { padding: 0px; margin: 0px; font-size: 100%; word-break: normal; white-space: pre; background: transparent; border: 0px; }
.markdown-preview[data-use-github-style] .highlight { margin-bottom: 16px; }
.markdown-preview[data-use-github-style] .highlight pre, .markdown-preview[data-use-github-style] pre { padding: 16px; overflow: auto; font-size: 85%; line-height: 1.45; background-color: rgb(247, 247, 247); border-radius: 3px; }
.markdown-preview[data-use-github-style] .highlight pre { margin-bottom: 0px; word-break: normal; }
.markdown-preview[data-use-github-style] pre { overflow-wrap: normal; }
.markdown-preview[data-use-github-style] pre code, .markdown-preview[data-use-github-style] pre tt { display: inline; max-width: initial; padding: 0px; margin: 0px; overflow: initial; line-height: inherit; overflow-wrap: normal; background-color: transparent; border: 0px; }
.markdown-preview[data-use-github-style] pre code::before, .markdown-preview[data-use-github-style] pre tt::before, .markdown-preview[data-use-github-style] pre code::after, .markdown-preview[data-use-github-style] pre tt::after { content: normal; }
.markdown-preview[data-use-github-style] kbd { display: inline-block; padding: 3px 5px; font-size: 11px; line-height: 10px; color: rgb(85, 85, 85); vertical-align: middle; background-color: rgb(252, 252, 252); border-width: 1px; border-style: solid; border-color: rgb(204, 204, 204) rgb(204, 204, 204) rgb(187, 187, 187); border-image: initial; border-radius: 3px; box-shadow: rgb(187, 187, 187) 0px -1px 0px inset; }
.markdown-preview[data-use-github-style] a { color: rgb(51, 122, 183); }
.markdown-preview[data-use-github-style] code { color: inherit; }
.markdown-preview[data-use-github-style] pre.editor-colors { padding: 0.8em 1em; margin-bottom: 1em; font-size: 0.85em; border-radius: 4px; overflow: auto; }
.markdown-preview pre.editor-colors { user-select: auto; }
.scrollbars-visible-always .markdown-preview pre.editor-colors .vertical-scrollbar, .scrollbars-visible-always .markdown-preview pre.editor-colors .horizontal-scrollbar { visibility: hidden; }
.scrollbars-visible-always .markdown-preview pre.editor-colors:hover .vertical-scrollbar, .scrollbars-visible-always .markdown-preview pre.editor-colors:hover .horizontal-scrollbar { visibility: visible; }
.markdown-preview .task-list-item input[type="checkbox"] { position: absolute; margin: 0.25em 0px 0px -1.4em; }
.markdown-preview .task-list-item { list-style-type: none; }
.bracket-matcher .region {
  border-bottom: 1px dotted lime;
  position: absolute;
}
.line-number.bracket-matcher.bracket-matcher {
  color: hsl(220, 14%, 71%);
  background-color: hsl(220, 13%, 26%);
}

.spell-check-misspelling .region {
  border-bottom: 2px dotted hsla(0, 100%, 60%, 0.75);
}
.spell-check-corrections {
  width: 25em !important;
}

pre.editor-colors {
  background-color: hsl(220, 13%, 18%);
  color: hsl(220, 14%, 71%);
}
pre.editor-colors .line.cursor-line {
  background-color: hsla(220, 100%, 80%, 0.04);
}
pre.editor-colors .invisible {
  color: hsl(220, 14%, 71%);
}
pre.editor-colors .cursor {
  border-left: 2px solid hsl(220, 100%, 66%);
}
pre.editor-colors .selection .region {
  background-color: hsl(220, 13%, 28%);
}
pre.editor-colors .bracket-matcher .region {
  border-bottom: 1px solid hsl(220, 100%, 66%);
  box-sizing: border-box;
}
pre.editor-colors .invisible-character {
  color: hsla(220, 14%, 71%, 0.15);
}
pre.editor-colors .indent-guide {
  color: hsla(220, 14%, 71%, 0.15);
}
pre.editor-colors .wrap-guide {
  background-color: hsla(220, 14%, 71%, 0.15);
}
pre.editor-colors .find-result .region.region.region,
pre.editor-colors .current-result .region.region.region {
  border-radius: 2px;
  background-color: hsla(220, 100%, 66%, 0.24);
  transition: border-color 0.4s;
}
pre.editor-colors .find-result .region.region.region {
  border: 2px solid transparent;
}
pre.editor-colors .current-result .region.region.region {
  border: 2px solid hsl(220, 100%, 66%);
  transition-duration: 0.1s;
}
pre.editor-colors .gutter .line-number {
  color: hsl(220, 14%, 45%);
  -webkit-font-smoothing: antialiased;
}
pre.editor-colors .gutter .line-number.cursor-line {
  color: hsl(220, 14%, 71%);
  background-color: hsl(220, 13%, 26%);
}
pre.editor-colors .gutter .line-number.cursor-line-no-selection {
  background-color: transparent;
}
pre.editor-colors .gutter .line-number .icon-right {
  color: hsl(220, 14%, 71%);
}
pre.editor-colors .gutter:not(.git-diff-icon) .line-number.git-line-removed.git-line-removed::before {
  bottom: -3px;
}
pre.editor-colors .gutter:not(.git-diff-icon) .line-number.git-line-removed::after {
  content: "";
  position: absolute;
  left: 0px;
  bottom: 0px;
  width: 25px;
  border-bottom: 1px dotted hsla(0, 70%, 60%, 0.5);
  pointer-events: none;
}
pre.editor-colors .gutter .line-number.folded,
pre.editor-colors .gutter .line-number:after,
pre.editor-colors .fold-marker:after {
  color: hsl(220, 14%, 71%);
}
.syntax--comment {
  color: hsl(220, 10%, 40%);
  font-style: italic;
}
.syntax--comment .syntax--markup.syntax--link {
  color: hsl(220, 10%, 40%);
}
.syntax--entity.syntax--name.syntax--type {
  color: hsl(39, 67%, 69%);
}
.syntax--entity.syntax--other.syntax--inherited-class {
  color: hsl(39, 67%, 69%);
}
.syntax--keyword {
  color: hsl(286, 60%, 67%);
}
.syntax--keyword.syntax--control {
  color: hsl(286, 60%, 67%);
}
.syntax--keyword.syntax--operator {
  color: hsl(286, 60%, 67%);
}
.syntax--keyword.syntax--other.syntax--special-method {
  color: hsl(207, 82%, 66%);
}
.syntax--keyword.syntax--other.syntax--unit {
  color: hsl(29, 54%, 61%);
}
.syntax--storage {
  color: hsl(286, 60%, 67%);
}
.syntax--storage.syntax--type.syntax--annotation,
.syntax--storage.syntax--type.syntax--primitive {
  color: hsl(286, 60%, 67%);
}
.syntax--storage.syntax--modifier.syntax--package,
.syntax--storage.syntax--modifier.syntax--import {
  color: hsl(220, 14%, 71%);
}
.syntax--constant {
  color: hsl(29, 54%, 61%);
}
.syntax--constant.syntax--variable {
  color: hsl(29, 54%, 61%);
}
.syntax--constant.syntax--character.syntax--escape {
  color: hsl(187, 47%, 55%);
}
.syntax--constant.syntax--numeric {
  color: hsl(29, 54%, 61%);
}
.syntax--constant.syntax--other.syntax--color {
  color: hsl(187, 47%, 55%);
}
.syntax--constant.syntax--other.syntax--symbol {
  color: hsl(187, 47%, 55%);
}
.syntax--variable {
  color: hsl(355, 65%, 65%);
}
.syntax--variable.syntax--interpolation {
  color: hsl(5, 48%, 51%);
}
.syntax--variable.syntax--parameter {
  color: hsl(220, 14%, 71%);
}
.syntax--string {
  color: hsl(95, 38%, 62%);
}
.syntax--string > .syntax--source,
.syntax--string .syntax--embedded {
  color: hsl(220, 14%, 71%);
}
.syntax--string.syntax--regexp {
  color: hsl(187, 47%, 55%);
}
.syntax--string.syntax--regexp .syntax--source.syntax--ruby.syntax--embedded {
  color: hsl(39, 67%, 69%);
}
.syntax--string.syntax--other.syntax--link {
  color: hsl(355, 65%, 65%);
}
.syntax--punctuation.syntax--definition.syntax--comment {
  color: hsl(220, 10%, 40%);
}
.syntax--punctuation.syntax--definition.syntax--method-parameters,
.syntax--punctuation.syntax--definition.syntax--function-parameters,
.syntax--punctuation.syntax--definition.syntax--parameters,
.syntax--punctuation.syntax--definition.syntax--separator,
.syntax--punctuation.syntax--definition.syntax--seperator,
.syntax--punctuation.syntax--definition.syntax--array {
  color: hsl(220, 14%, 71%);
}
.syntax--punctuation.syntax--definition.syntax--bold {
  color: hsl(39, 67%, 69%);
  font-weight: bold;
}
.syntax--punctuation.syntax--definition.syntax--italic {
  color: hsl(286, 60%, 67%);
  font-style: italic;
}
.syntax--punctuation.syntax--section.syntax--embedded {
  color: hsl(5, 48%, 51%);
}
.syntax--punctuation.syntax--section.syntax--method,
.syntax--punctuation.syntax--section.syntax--class,
.syntax--punctuation.syntax--section.syntax--inner-class {
  color: hsl(220, 14%, 71%);
}
.syntax--support.syntax--class,
.syntax--support.syntax--module {
  color: hsl(39, 67%, 69%);
}
.syntax--support.syntax--namespace {
  color: hsl(39, 67%, 69%);
}
.syntax--support.syntax--type {
  color: hsl(187, 47%, 55%);
}
.syntax--support.syntax--other.syntax--function {
  color: hsl(207, 82%, 66%);
}
.syntax--support.syntax--function {
  color: hsl(187, 47%, 55%);
}
.syntax--support.syntax--function.syntax--any-method {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--name.syntax--function {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--name.syntax--class,
.syntax--entity.syntax--name.syntax--type.syntax--class {
  color: hsl(39, 67%, 69%);
}
.syntax--entity.syntax--name.syntax--section {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--name.syntax--tag {
  color: hsl(355, 65%, 65%);
}
.syntax--entity.syntax--other.syntax--attribute-name {
  color: hsl(29, 54%, 61%);
}
.syntax--entity.syntax--other.syntax--attribute-name.syntax--id {
  color: hsl(207, 82%, 66%);
}
.syntax--meta.syntax--class:not(.syntax--block) {
  color: hsl(39, 67%, 69%);
}
.syntax--meta.syntax--class:not(.syntax--block).syntax--body {
  color: hsl(220, 14%, 71%);
}
.syntax--meta.syntax--method-call,
.syntax--meta.syntax--method {
  color: hsl(220, 14%, 71%);
}
.syntax--meta.syntax--definition.syntax--variable {
  color: hsl(355, 65%, 65%);
}
.syntax--meta.syntax--link {
  color: hsl(29, 54%, 61%);
}
.syntax--meta.syntax--require {
  color: hsl(207, 82%, 66%);
}
.syntax--meta.syntax--selector {
  color: hsl(286, 60%, 67%);
}
.syntax--meta.syntax--separator {
  color: hsl(220, 14%, 71%);
}
.syntax--meta.syntax--tag {
  color: hsl(220, 14%, 71%);
}
.syntax--underline {
  text-decoration: underline;
}
.syntax--none {
  color: hsl(220, 14%, 71%);
}
.syntax--invalid.syntax--deprecated {
  color: hsl(40, 60%, 20%) !important;
  background-color: hsl(40, 60%, 70%) !important;
}
.syntax--invalid.syntax--illegal {
  color: white !important;
  background-color: hsl(0, 70%, 60%) !important;
}
.syntax--markup.syntax--bold {
  color: hsl(29, 54%, 61%);
  font-weight: bold;
}
.syntax--markup.syntax--changed {
  color: hsl(286, 60%, 67%);
}
.syntax--markup.syntax--deleted {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--italic {
  color: hsl(286, 60%, 67%);
  font-style: italic;
}
.syntax--markup.syntax--heading {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--heading .syntax--punctuation.syntax--definition.syntax--heading {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--link {
  color: hsl(187, 47%, 55%);
}
.syntax--markup.syntax--inserted {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--quote {
  color: hsl(29, 54%, 61%);
}
.syntax--markup.syntax--raw {
  color: hsl(95, 38%, 62%);
}
.syntax--source.syntax--cs .syntax--keyword.syntax--operator {
  color: hsl(286, 60%, 67%);
}
.syntax--source.syntax--css .syntax--property-name,
.syntax--source.syntax--css .syntax--property-value {
  color: hsl(220, 9%, 55%);
}
.syntax--source.syntax--css .syntax--property-name.syntax--support,
.syntax--source.syntax--css .syntax--property-value.syntax--support {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--elixir .syntax--source.syntax--embedded.syntax--source {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--elixir .syntax--constant.syntax--language,
.syntax--source.syntax--elixir .syntax--constant.syntax--numeric,
.syntax--source.syntax--elixir .syntax--constant.syntax--definition {
  color: hsl(207, 82%, 66%);
}
.syntax--source.syntax--elixir .syntax--variable.syntax--definition,
.syntax--source.syntax--elixir .syntax--variable.syntax--anonymous {
  color: hsl(286, 60%, 67%);
}
.syntax--source.syntax--elixir .syntax--parameter.syntax--variable.syntax--function {
  color: hsl(29, 54%, 61%);
  font-style: italic;
}
.syntax--source.syntax--elixir .syntax--quoted {
  color: hsl(95, 38%, 62%);
}
.syntax--source.syntax--elixir .syntax--keyword.syntax--special-method,
.syntax--source.syntax--elixir .syntax--embedded.syntax--section,
.syntax--source.syntax--elixir .syntax--embedded.syntax--source.syntax--empty {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--elixir .syntax--readwrite.syntax--module .syntax--punctuation {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--elixir .syntax--regexp.syntax--section,
.syntax--source.syntax--elixir .syntax--regexp.syntax--string {
  color: hsl(5, 48%, 51%);
}
.syntax--source.syntax--elixir .syntax--separator,
.syntax--source.syntax--elixir .syntax--keyword.syntax--operator {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--elixir .syntax--variable.syntax--constant {
  color: hsl(39, 67%, 69%);
}
.syntax--source.syntax--elixir .syntax--array,
.syntax--source.syntax--elixir .syntax--scope,
.syntax--source.syntax--elixir .syntax--section {
  color: hsl(220, 9%, 55%);
}
.syntax--source.syntax--gfm .syntax--markup {
  -webkit-font-smoothing: auto;
}
.syntax--source.syntax--gfm .syntax--link .syntax--entity {
  color: hsl(207, 82%, 66%);
}
.syntax--source.syntax--gfm .syntax--punctuation.syntax--definition.syntax--list-item {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--gfm .syntax--meta.syntax--link.syntax--text {
  color: hsl(207, 82%, 66%);
}
.syntax--source.syntax--ini .syntax--keyword.syntax--other.syntax--definition.syntax--ini {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--java .syntax--storage.syntax--modifier.syntax--import {
  color: hsl(39, 67%, 69%);
}
.syntax--source.syntax--java .syntax--storage.syntax--type {
  color: hsl(39, 67%, 69%);
}
.syntax--source.syntax--java .syntax--keyword.syntax--operator.syntax--instanceof {
  color: hsl(286, 60%, 67%);
}
.syntax--source.syntax--java-properties .syntax--meta.syntax--key-pair {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--java-properties .syntax--meta.syntax--key-pair > .syntax--punctuation {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--ts .syntax--keyword.syntax--operator {
  color: hsl(187, 47%, 55%);
}
.syntax--source.syntax--flow .syntax--keyword.syntax--operator {
  color: hsl(187, 47%, 55%);
}
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--dictionary.syntax--json > .syntax--string.syntax--quoted.syntax--json {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--dictionary.syntax--json > .syntax--string.syntax--quoted.syntax--json > .syntax--punctuation.syntax--string {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--dictionary.syntax--json > .syntax--value.syntax--json > .syntax--string.syntax--quoted.syntax--json,
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--array.syntax--json > .syntax--value.syntax--json > .syntax--string.syntax--quoted.syntax--json,
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--dictionary.syntax--json > .syntax--value.syntax--json > .syntax--string.syntax--quoted.syntax--json > .syntax--punctuation,
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--array.syntax--json > .syntax--value.syntax--json > .syntax--string.syntax--quoted.syntax--json > .syntax--punctuation {
  color: hsl(95, 38%, 62%);
}
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--dictionary.syntax--json > .syntax--constant.syntax--language.syntax--json,
.syntax--source.syntax--json .syntax--meta.syntax--structure.syntax--array.syntax--json > .syntax--constant.syntax--language.syntax--json {
  color: hsl(187, 47%, 55%);
}
.syntax--ng.syntax--interpolation {
  color: hsl(355, 65%, 65%);
}
.syntax--ng.syntax--interpolation.syntax--begin,
.syntax--ng.syntax--interpolation.syntax--end {
  color: hsl(207, 82%, 66%);
}
.syntax--ng.syntax--interpolation .syntax--function {
  color: hsl(355, 65%, 65%);
}
.syntax--ng.syntax--interpolation .syntax--function.syntax--begin,
.syntax--ng.syntax--interpolation .syntax--function.syntax--end {
  color: hsl(207, 82%, 66%);
}
.syntax--ng.syntax--interpolation .syntax--bool {
  color: hsl(29, 54%, 61%);
}
.syntax--ng.syntax--interpolation .syntax--bracket {
  color: hsl(220, 14%, 71%);
}
.syntax--ng.syntax--pipe,
.syntax--ng.syntax--operator {
  color: hsl(220, 14%, 71%);
}
.syntax--ng.syntax--tag {
  color: hsl(187, 47%, 55%);
}
.syntax--ng.syntax--attribute-with-value .syntax--attribute-name {
  color: hsl(39, 67%, 69%);
}
.syntax--ng.syntax--attribute-with-value .syntax--string {
  color: hsl(286, 60%, 67%);
}
.syntax--ng.syntax--attribute-with-value .syntax--string.syntax--begin,
.syntax--ng.syntax--attribute-with-value .syntax--string.syntax--end {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--php .syntax--class.syntax--bracket {
  color: hsl(220, 14%, 71%);
}
/*
   This defines styling rules for syntax classes.

   See the naming conventions for a list of syntax classes:
   https://flight-manual.atom.io/hacking-atom/sections/syntax-naming-conventions

   When styling rules conflict:
   - The last rule overrides previous rules.
   - The rule with most classes and pseudo-classes overrides the last rule.
*/
.syntax--keyword {
  color: hsl(286, 60%, 67%);
}
.syntax--keyword.syntax--type {
  color: hsl(187, 47%, 55%);
}
.syntax--keyword.syntax--function {
  color: hsl(355, 65%, 65%);
}
.syntax--keyword.syntax--variable {
  color: hsl(355, 65%, 65%);
}
.syntax--entity {
  color: hsl(220, 14%, 71%);
}
.syntax--entity.syntax--parameter {
  color: hsl(220, 14%, 71%);
}
.syntax--entity.syntax--support {
  color: hsl(355, 65%, 65%);
}
.syntax--entity.syntax--decorator:last-child {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--label {
  text-decoration: underline;
}
.syntax--entity.syntax--function {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--operator {
  color: hsl(207, 82%, 66%);
}
.syntax--entity.syntax--operator.syntax--symbolic {
  color: hsl(220, 14%, 71%);
}
.syntax--entity.syntax--type {
  color: hsl(187, 47%, 55%);
}
.syntax--entity.syntax--tag {
  color: hsl(355, 65%, 65%);
}
.syntax--entity.syntax--attribute {
  color: hsl(29, 54%, 61%);
}
.syntax--punctuation {
  color: hsl(220, 14%, 71%);
}
.syntax--punctuation.syntax--accessor {
  color: hsl(220, 14%, 71%);
}
.syntax--punctuation.syntax--accessor.syntax--member,
.syntax--punctuation.syntax--accessor.syntax--scope {
  color: hsl(286, 60%, 67%);
}
.syntax--punctuation.syntax--embedded {
  color: hsl(286, 60%, 67%);
}
.syntax--string {
  color: hsl(95, 38%, 62%);
}
.syntax--string.syntax--immutable {
  color: hsl(95, 38%, 62%);
}
.syntax--string.syntax--part {
  color: hsl(187, 47%, 55%);
}
.syntax--string.syntax--interpolation {
  color: hsl(286, 60%, 67%);
}
.syntax--string.syntax--regexp {
  color: hsl(95, 38%, 62%);
}
.syntax--string.syntax--regexp.syntax--language {
  color: hsl(286, 60%, 67%);
}
.syntax--string.syntax--regexp.syntax--variable {
  color: hsl(207, 82%, 66%);
}
.syntax--string.syntax--regexp.syntax--punctuation {
  color: hsl(286, 60%, 67%);
}
.syntax--constant {
  color: hsl(29, 54%, 61%);
}
.syntax--constant.syntax--character {
  color: hsl(95, 38%, 62%);
}
.syntax--constant.syntax--character.syntax--escape {
  color: hsl(95, 38%, 62%);
}
.syntax--constant.syntax--character.syntax--code {
  color: hsl(187, 47%, 55%);
}
.syntax--text {
  color: hsl(220, 14%, 71%);
}
.syntax--markup.syntax--heading {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--list.syntax--punctuation {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--quote {
  color: hsl(220, 10%, 40%);
  font-style: italic;
}
.syntax--markup.syntax--bold {
  color: hsl(29, 54%, 61%);
  font-weight: bold;
}
.syntax--markup.syntax--italic {
  color: hsl(286, 60%, 67%);
  font-style: italic;
}
.syntax--markup.syntax--underline {
  color: hsl(187, 47%, 55%);
  text-decoration: underline;
}
.syntax--markup.syntax--strike {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--raw {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--link {
  color: hsl(187, 47%, 55%);
}
.syntax--markup.syntax--alt {
  color: hsl(207, 82%, 66%);
}
.syntax--markup.syntax--inserted {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--inserted .syntax--punctuation {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--highlighted {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--highlighted .syntax--punctuation {
  color: hsl(95, 38%, 62%);
}
.syntax--markup.syntax--deleted {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--deleted .syntax--punctuation {
  color: hsl(355, 65%, 65%);
}
.syntax--markup.syntax--changed {
  color: hsl(286, 60%, 67%);
}
.syntax--markup.syntax--changed .syntax--punctuation {
  color: hsl(286, 60%, 67%);
}
.syntax--markup.syntax--commented {
  color: hsl(220, 10%, 40%);
}
.syntax--markup.syntax--commented .syntax--punctuation {
  color: hsl(220, 10%, 40%);
}
.syntax--comment {
  color: hsl(220, 10%, 40%);
  font-style: italic;
}
.syntax--comment.syntax--caption {
  color: hsl(220, 10%, 46%);
  font-weight: bold;
}
.syntax--comment.syntax--term {
  color: hsl(220, 10%, 49%);
}
.syntax--comment.syntax--punctuation {
  color: hsl(220, 10%, 40%);
  font-weight: normal;
}
.syntax--invalid:not(.syntax--punctuation).syntax--illegal {
  color: white !important;
  background-color: hsl(0, 70%, 60%) !important;
}
.syntax--invalid:not(.syntax--punctuation).syntax--deprecated {
  color: hsl(40, 60%, 20%) !important;
  background-color: hsl(40, 60%, 70%) !important;
}
.syntax--source.syntax--css .syntax--entity.syntax--function {
  color: hsl(220, 9%, 55%);
}
.syntax--source.syntax--css .syntax--entity.syntax--function.syntax--support {
  color: hsl(187, 47%, 55%);
}
.syntax--source.syntax--css .syntax--entity.syntax--selector {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--css .syntax--entity.syntax--selector.syntax--tag {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--css .syntax--entity.syntax--selector.syntax--id {
  color: hsl(207, 82%, 66%);
}
.syntax--source.syntax--css .syntax--entity.syntax--property {
  color: hsl(220, 9%, 55%);
}
.syntax--source.syntax--css .syntax--entity.syntax--property.syntax--support {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--css .syntax--entity.syntax--variable {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--css .syntax--constant {
  color: hsl(220, 9%, 55%);
}
.syntax--source.syntax--css .syntax--constant.syntax--support {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--css .syntax--constant.syntax--numeric {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--css .syntax--constant.syntax--media {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--css .syntax--constant.syntax--color {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--css .syntax--constant.syntax--offset {
  color: hsl(220, 14%, 71%);
}
.syntax--source.syntax--css .syntax--constant.syntax--attribute-value {
  color: hsl(95, 38%, 62%);
}
.syntax--source.syntax--css .syntax--punctuation.syntax--selector {
  color: hsl(29, 54%, 61%);
}
.syntax--source.syntax--css .syntax--punctuation.syntax--selector.syntax--wildcard {
  color: hsl(355, 65%, 65%);
}
.syntax--source.syntax--css .syntax--punctuation.syntax--selector.syntax--id {
  color: hsl(207, 82%, 66%);
}
.syntax--source.syntax--css .syntax--punctuation.syntax--selector.syntax--attribute {
  color: hsl(220, 14%, 71%);
}
</style>
  </head>
  <body class='markdown-preview' data-use-github-style><h1 id="pcp4-sigma-immunostaining-with-fluoro-nissl-counterfloating-xg">PCP4 (Sigma) immunostaining with Fluoro Nissl counter(Floating) XG</h1>
<h2 id="animals">Animals</h2>
<p>1.If needed, 150 ug colchicine should be injected into lateral ventricle or targeted tissue two days before perfusion to enhance GAD signals in the soma.</p>
<h2 id="procedure">Procedure</h2>
<h3 id="perfusion-agarose-embedding-sectioning">Perfusion, Agarose-Embedding, Sectioning</h3>
<ol>
<li>Transcardially perfuse with saline followed by 4% paraformaldehyde and 0.2% picric acid with 0.1 M phosphate buffer (pH 7.2–7.3). Postfix overnight with the same fixative.</li>
<li>Remove the dura. If possible, the arachnoid membrane, the pia also.</li>
<li>Embed the brain into the 4% electrophoresis quality agarose.
1.Section the brain with vibrating blade microtome into 40 to 70-µm-thick slices and harvest them in 12 well plates containing PBS
​</li>
</ol>
<h3 id="antibody-application-room-temperature-light-shielding">Antibody application (room temperature, light shielding)</h3>
<ol>
<li>10% NGS in PBS-X, 30 min on shaker</li>
<li>1st antibody in PBS-XG, overnight on shaker</li>
<li>PBS-X wash (quick × 1, 10 min × 2)</li>
<li>2nd antibody in PBS-XG for 2 h on shaker</li>
<li>PBS-X wash (quick × 1, 10 min × 2)</li>
<li>PBS wash
​</li>
</ol>
<h3 id="counterstaining-with-fluorescent-nissl">Counterstaining with Fluorescent Nissl</h3>
<ol>
<li>Diluted NeuroTrace (Blue), 40–60 min.</li>
<li>PBS wash (quick × 1, 10 min × 2)
​</li>
</ol>
<h3 id="mounting">Mounting</h3>
<ol>
<li>Mount on gelatin-coated glass slides and Airdry (30 min).
​</li>
</ol>
<h3 id="cover-slipping">Cover-slipping</h3>
<ol>
<li>Coverslip with 50% (v/v) glycerol/2.5% (w/v) DABCO in PBS.
​</li>
</ol>
<h3 id="observation">Observation</h3>
<ol>
<li>Observe with epifluorescence or confocal microscopy.
​</li>
</ol>
<h2 id="solutions">Solutions</h2>
<h3 id="pbs-x-final-03-total-550-ml">PBS-X (final 0.3%, total 550 ml)</h3>
<ul>
<li>20% Triton X-100 8.25 ml in PBS 541.75 ml
​</li>
</ul>
<h3 id="pbs-xg-150-ml">PBS-XG (150 ml)</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>amount</th>
<th>final conc.</th>
</tr>
</thead>
<tbody><tr>
<td>normal goat serum</td>
<td>1.5 ml</td>
<td>1%</td>
</tr>
<tr>
<td>sodium azide</td>
<td>30 mg</td>
<td>0.02%</td>
</tr>
<tr>
<td>PBS-X</td>
<td>148.5 ml</td>
<td></td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
</tr>
</tbody></table>
<h3 id="10-ngs-in-pbs-x-5-ml">10% NGS in PBS-X (5 ml)</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>amount</th>
<th>final conc.</th>
</tr>
</thead>
<tbody><tr>
<td>normal goat serum</td>
<td>0.45 ml</td>
<td>10%</td>
</tr>
<tr>
<td>PBS-XG</td>
<td>4.55</td>
<td></td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
</tr>
</tbody></table>
<h3 id="1st-antibody-oliva-et-al20161500-11000-recommended-in-doc-form-manufacture">1st antibody (Oliva et al.,2016)(1:500-1:1000 recommended in doc form manufacture)</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>manufacture</th>
<th>article no.</th>
<th>RRID</th>
<th>dilution</th>
</tr>
</thead>
<tbody><tr>
<td>Rb anti-PCP4</td>
<td>Sigma-Aldrich</td>
<td>HPA005792</td>
<td>AB_1855086</td>
<td>1:300</td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody></table>
<ul>
<li>dilute with PBS-XG
​</li>
</ul>
<h3 id="2nd-antibody11000-dilution-2-ugml-final">2nd antibody(1:1000 dilution, 2 ug/mL final)</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>manufacture</th>
<th>article no.</th>
<th>stock</th>
<th>dilution</th>
<th>final conc.</th>
</tr>
</thead>
<tbody><tr>
<td>Goat anti-rabbit IgG Alexa 488</td>
<td>Thermo Fisher Scientific</td>
<td>A-11034</td>
<td>2 mg/ml</td>
<td>1:1000</td>
<td>2 µg/ml final</td>
</tr>
<tr>
<td>Goat anti-rabbit IgG Alexa 633</td>
<td>Thermo Fisher Scientific</td>
<td>A-21071</td>
<td>2 mg/ml</td>
<td>1:1000</td>
<td>2 µg/ml final</td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody></table>
<ul>
<li>dilute with PBS-XG</li>
<li>choose one of them
​</li>
</ul>
<h3 id="diluted-neurotrace-solution">Diluted NeuroTrace Solution</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>manufacture</th>
<th>article no.</th>
<th>dilution</th>
</tr>
</thead>
<tbody><tr>
<td>NeuroTrace Blue</td>
<td>Thermo Fisher Scientific</td>
<td>N-21479</td>
<td>1:150 for Confocal microscopy</td>
</tr>
<tr>
<td></td>
<td></td>
<td></td>
<td>1:300 for epifluorescence microscopy</td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody></table>
<ul>
<li>dilute with PBS
​</li>
</ul>
<h3 id="reagents">Reagents</h3>
<table>
<thead>
<tr>
<th>name</th>
<th>manufacture</th>
<th>article no.</th>
<th>unit</th>
<th>price</th>
</tr>
</thead>
<tbody><tr>
<td>1st Antibody</td>
<td>Sigma</td>
<td></td>
<td>100 µL</td>
<td>123.165 HUF</td>
</tr>
<tr>
<td>2nd antibody</td>
<td>Thermo Fisher Scientific</td>
<td>A-11034</td>
<td>0.5 ml</td>
<td>71,900 HUF</td>
</tr>
<tr>
<td>2nd antibody</td>
<td>Thermo Fisher Scientific</td>
<td>A-21071</td>
<td>0.5 ml</td>
<td>71,900 HUF</td>
</tr>
<tr>
<td>NeuroTrace Blue</td>
<td>Thermo Fisher Scientific</td>
<td>N-21479</td>
<td>1.0 ml</td>
<td>34,000 JPY</td>
</tr>
<tr>
<td>Normal Goat serum S-100</td>
<td>Vector laboratories</td>
<td>G9023-10ML</td>
<td>20 ml</td>
<td></td>
</tr>
<tr>
<td>​</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>##References</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr>
<td>Oliva A, Fernandez-Ruiz A, Buzsaki G, Berenyi A (2016) Role of Hippocampal CA2 Region in Triggering Sharp-Wave Ripples. Neuron 91:1342-1355.</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody></table></body>
</html>
