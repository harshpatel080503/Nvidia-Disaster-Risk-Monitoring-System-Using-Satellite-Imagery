<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>assessment</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>




<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>



<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/*
 * Webkit scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-corner {
  background: var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-thumb {
  background: rgb(var(--jp-scrollbar-thumb-color));
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-right: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-bottom: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar */

[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-corner,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-corner {
  background-color: transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-thumb,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid transparent;
  border-right: var(--jp-scrollbar-endpad) solid transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid transparent;
  border-bottom: var(--jp-scrollbar-endpad) solid transparent;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0px solid transparent;
  border-right: 0px solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0px solid transparent;
  border-bottom: 0px solid transparent;
}

/*
 * Phosphor
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Widget, /* </DEPRECATED> */
.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  cursor: default;
}


/* <DEPRECATED> */ .p-Widget.p-mod-hidden, /* </DEPRECATED> */
.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-CommandPalette, /* </DEPRECATED> */
.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-CommandPalette-search, /* </DEPRECATED> */
.lm-CommandPalette-search {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-content, /* </DEPRECATED> */
.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-CommandPalette-header, /* </DEPRECATED> */
.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}


/* <DEPRECATED> */ .p-CommandPalette-item, /* </DEPRECATED> */
.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}


/* <DEPRECATED> */ .p-CommandPalette-itemIcon, /* </DEPRECATED> */
.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemContent, /* </DEPRECATED> */
.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}


/* <DEPRECATED> */ .p-CommandPalette-itemShortcut, /* </DEPRECATED> */
.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemLabel, /* </DEPRECATED> */
.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
	border:1px solid transparent;
  background-color: transparent;
  position: absolute;
	z-index:1;
	right:3%;
	top: 0;
	bottom: 0;
	margin: auto;
	padding: 7px 0;
	display: none;
	vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
	content: "X";
	display: block;
	width: 15px;
	height: 15px;
	text-align: center;
	color:#000;
	font-weight: normal;
	font-size: 12px;
	cursor: pointer;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-DockPanel, /* </DEPRECATED> */
.lm-DockPanel {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-widget, /* </DEPRECATED> */
.lm-DockPanel-widget {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-tabBar, /* </DEPRECATED> */
.lm-DockPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-DockPanel-handle, /* </DEPRECATED> */
.lm-DockPanel-handle {
  z-index: 2;
}


/* <DEPRECATED> */ .p-DockPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-DockPanel-handle:after, /* </DEPRECATED> */
.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}


/* <DEPRECATED> */ .p-DockPanel-overlay, /* </DEPRECATED> */
.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}


/* <DEPRECATED> */ .p-DockPanel-overlay.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Menu, /* </DEPRECATED> */
.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-Menu-content, /* </DEPRECATED> */
.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-Menu-item, /* </DEPRECATED> */
.lm-Menu-item {
  display: table-row;
}


/* <DEPRECATED> */
.p-Menu-item.p-mod-hidden,
.p-Menu-item.p-mod-collapsed,
/* </DEPRECATED> */
.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}


/* <DEPRECATED> */
.p-Menu-itemIcon,
.p-Menu-itemSubmenuIcon,
/* </DEPRECATED> */
.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}


/* <DEPRECATED> */ .p-Menu-itemLabel, /* </DEPRECATED> */
.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}


/* <DEPRECATED> */ .p-Menu-itemShortcut, /* </DEPRECATED> */
.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-MenuBar, /* </DEPRECATED> */
.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-MenuBar-content, /* </DEPRECATED> */
.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}


/* <DEPRECATED> */ .p--MenuBar-item, /* </DEPRECATED> */
.lm-MenuBar-item {
  box-sizing: border-box;
}


/* <DEPRECATED> */
.p-MenuBar-itemIcon,
.p-MenuBar-itemLabel,
/* </DEPRECATED> */
.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-ScrollBar, /* </DEPRECATED> */
.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-ScrollBar-button, /* </DEPRECATED> */
.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-track, /* </DEPRECATED> */
.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-thumb, /* </DEPRECATED> */
.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-SplitPanel-child, /* </DEPRECATED> */
.lm-SplitPanel-child {
  z-index: 0;
}


/* <DEPRECATED> */ .p-SplitPanel-handle, /* </DEPRECATED> */
.lm-SplitPanel-handle {
  z-index: 1;
}


/* <DEPRECATED> */ .p-SplitPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-SplitPanel-handle:after, /* </DEPRECATED> */
.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabBar, /* </DEPRECATED> */
.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='horizontal'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='vertical'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}


/* <DEPRECATED> */ .p-TabBar-content, /* </DEPRECATED> */
.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='horizontal'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='vertical'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
}


/* <DEPRECATED> */
.p-TabBar-tabIcon,
.p-TabBar-tabCloseIcon,
/* </DEPRECATED> */
.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-TabBar-tabLabel, /* </DEPRECATED> */
.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}


.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
}


/* <DEPRECATED> */ .p-TabBar-tab.p-mod-hidden, /* </DEPRECATED> */
.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}


.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-TabBar.p-mod-dragging .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='horizontal'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='vertical'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing : border-box;
  background: inherit;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabPanel-tabBar, /* </DEPRECATED> */
.lm-TabPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-TabPanel-stackedPanel, /* </DEPRECATED> */
.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

@charset "UTF-8";
html{
  -webkit-box-sizing:border-box;
          box-sizing:border-box; }

*,
*::before,
*::after{
  -webkit-box-sizing:inherit;
          box-sizing:inherit; }

body{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none;
  color:#182026;
  font-family:-apple-system, "BlinkMacSystemFont", "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Open Sans", "Helvetica Neue", "Icons16", sans-serif; }

p{
  margin-bottom:10px;
  margin-top:0; }

small{
  font-size:12px; }

strong{
  font-weight:600; }

::-moz-selection{
  background:rgba(125, 188, 255, 0.6); }

::selection{
  background:rgba(125, 188, 255, 0.6); }
.bp3-heading{
  color:#182026;
  font-weight:600;
  margin:0 0 10px;
  padding:0; }
  .bp3-dark .bp3-heading{
    color:#f5f8fa; }

h1.bp3-heading, .bp3-running-text h1{
  font-size:36px;
  line-height:40px; }

h2.bp3-heading, .bp3-running-text h2{
  font-size:28px;
  line-height:32px; }

h3.bp3-heading, .bp3-running-text h3{
  font-size:22px;
  line-height:25px; }

h4.bp3-heading, .bp3-running-text h4{
  font-size:18px;
  line-height:21px; }

h5.bp3-heading, .bp3-running-text h5{
  font-size:16px;
  line-height:19px; }

h6.bp3-heading, .bp3-running-text h6{
  font-size:14px;
  line-height:16px; }
.bp3-ui-text{
  font-size:14px;
  font-weight:400;
  letter-spacing:0;
  line-height:1.28581;
  text-transform:none; }

.bp3-monospace-text{
  font-family:monospace;
  text-transform:none; }

.bp3-text-muted{
  color:#5c7080; }
  .bp3-dark .bp3-text-muted{
    color:#a7b6c2; }

.bp3-text-disabled{
  color:rgba(92, 112, 128, 0.6); }
  .bp3-dark .bp3-text-disabled{
    color:rgba(167, 182, 194, 0.6); }

.bp3-text-overflow-ellipsis{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal; }
.bp3-running-text{
  font-size:14px;
  line-height:1.5; }
  .bp3-running-text h1{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h1{
      color:#f5f8fa; }
  .bp3-running-text h2{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h2{
      color:#f5f8fa; }
  .bp3-running-text h3{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h3{
      color:#f5f8fa; }
  .bp3-running-text h4{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h4{
      color:#f5f8fa; }
  .bp3-running-text h5{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h5{
      color:#f5f8fa; }
  .bp3-running-text h6{
    color:#182026;
    font-weight:600;
    margin-bottom:20px;
    margin-top:40px; }
    .bp3-dark .bp3-running-text h6{
      color:#f5f8fa; }
  .bp3-running-text hr{
    border:none;
    border-bottom:1px solid rgba(16, 22, 26, 0.15);
    margin:20px 0; }
    .bp3-dark .bp3-running-text hr{
      border-color:rgba(255, 255, 255, 0.15); }
  .bp3-running-text p{
    margin:0 0 10px;
    padding:0; }

.bp3-text-large{
  font-size:16px; }

.bp3-text-small{
  font-size:12px; }
a{
  color:#106ba3;
  text-decoration:none; }
  a:hover{
    color:#106ba3;
    cursor:pointer;
    text-decoration:underline; }
  a .bp3-icon, a .bp3-icon-standard, a .bp3-icon-large{
    color:inherit; }
  a code,
  .bp3-dark a code{
    color:inherit; }
  .bp3-dark a,
  .bp3-dark a:hover{
    color:#48aff0; }
    .bp3-dark a .bp3-icon, .bp3-dark a .bp3-icon-standard, .bp3-dark a .bp3-icon-large,
    .bp3-dark a:hover .bp3-icon,
    .bp3-dark a:hover .bp3-icon-standard,
    .bp3-dark a:hover .bp3-icon-large{
      color:inherit; }
.bp3-running-text code, .bp3-code{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  font-size:smaller;
  padding:2px 5px; }
  .bp3-dark .bp3-running-text code, .bp3-running-text .bp3-dark code, .bp3-dark .bp3-code{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
  .bp3-running-text a > code, a > .bp3-code{
    color:#137cbd; }
    .bp3-dark .bp3-running-text a > code, .bp3-running-text .bp3-dark a > code, .bp3-dark a > .bp3-code{
      color:inherit; }

.bp3-running-text pre, .bp3-code-block{
  font-family:monospace;
  text-transform:none;
  background:rgba(255, 255, 255, 0.7);
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
  color:#182026;
  display:block;
  font-size:13px;
  line-height:1.4;
  margin:10px 0;
  padding:13px 15px 12px;
  word-break:break-all;
  word-wrap:break-word; }
  .bp3-dark .bp3-running-text pre, .bp3-running-text .bp3-dark pre, .bp3-dark .bp3-code-block{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
  .bp3-running-text pre > code, .bp3-code-block > code{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit;
    font-size:inherit;
    padding:0; }

.bp3-running-text kbd, .bp3-key{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#5c7080;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-family:inherit;
  font-size:12px;
  height:24px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  line-height:24px;
  min-width:24px;
  padding:3px 6px;
  vertical-align:middle; }
  .bp3-running-text kbd .bp3-icon, .bp3-key .bp3-icon, .bp3-running-text kbd .bp3-icon-standard, .bp3-key .bp3-icon-standard, .bp3-running-text kbd .bp3-icon-large, .bp3-key .bp3-icon-large{
    margin-right:5px; }
  .bp3-dark .bp3-running-text kbd, .bp3-running-text .bp3-dark kbd, .bp3-dark .bp3-key{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#a7b6c2; }
.bp3-running-text blockquote, .bp3-blockquote{
  border-left:solid 4px rgba(167, 182, 194, 0.5);
  margin:0 0 10px;
  padding:0 20px; }
  .bp3-dark .bp3-running-text blockquote, .bp3-running-text .bp3-dark blockquote, .bp3-dark .bp3-blockquote{
    border-color:rgba(115, 134, 148, 0.5); }
.bp3-running-text ul,
.bp3-running-text ol, .bp3-list{
  margin:10px 0;
  padding-left:30px; }
  .bp3-running-text ul li:not(:last-child), .bp3-running-text ol li:not(:last-child), .bp3-list li:not(:last-child){
    margin-bottom:5px; }
  .bp3-running-text ul ol, .bp3-running-text ol ol, .bp3-list ol,
  .bp3-running-text ul ul,
  .bp3-running-text ol ul,
  .bp3-list ul{
    margin-top:5px; }

.bp3-list-unstyled{
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-list-unstyled li{
    padding:0; }
.bp3-rtl{
  text-align:right; }

.bp3-dark{
  color:#f5f8fa; }

:focus{
  outline:rgba(19, 124, 189, 0.6) auto 2px;
  outline-offset:2px;
  -moz-outline-radius:6px; }

.bp3-focus-disabled :focus{
  outline:none !important; }
  .bp3-focus-disabled :focus ~ .bp3-control-indicator{
    outline:none !important; }

.bp3-alert{
  max-width:400px;
  padding:20px; }

.bp3-alert-body{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-alert-body .bp3-icon{
    font-size:40px;
    margin-right:20px;
    margin-top:0; }

.bp3-alert-contents{
  word-break:break-word; }

.bp3-alert-footer{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:reverse;
      -ms-flex-direction:row-reverse;
          flex-direction:row-reverse;
  margin-top:10px; }
  .bp3-alert-footer .bp3-button{
    margin-left:10px; }
.bp3-breadcrumbs{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  cursor:default;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:wrap;
      flex-wrap:wrap;
  height:30px;
  list-style:none;
  margin:0;
  padding:0; }
  .bp3-breadcrumbs > li{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }
    .bp3-breadcrumbs > li::after{
      background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M10.71 7.29l-4-4a1.003 1.003 0 00-1.42 1.42L8.59 8 5.3 11.29c-.19.18-.3.43-.3.71a1.003 1.003 0 001.71.71l4-4c.18-.18.29-.43.29-.71 0-.28-.11-.53-.29-.71z' fill='%235C7080'/%3e%3c/svg%3e");
      content:"";
      display:block;
      height:16px;
      margin:0 5px;
      width:16px; }
    .bp3-breadcrumbs > li:last-of-type::after{
      display:none; }

.bp3-breadcrumb,
.bp3-breadcrumb-current,
.bp3-breadcrumbs-collapsed{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  font-size:16px; }

.bp3-breadcrumb,
.bp3-breadcrumbs-collapsed{
  color:#5c7080; }

.bp3-breadcrumb:hover{
  text-decoration:none; }

.bp3-breadcrumb.bp3-disabled{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-breadcrumb .bp3-icon{
  margin-right:5px; }

.bp3-breadcrumb-current{
  color:inherit;
  font-weight:600; }
  .bp3-breadcrumb-current .bp3-input{
    font-size:inherit;
    font-weight:inherit;
    vertical-align:baseline; }

.bp3-breadcrumbs-collapsed{
  background:#ced9e0;
  border:none;
  border-radius:3px;
  cursor:pointer;
  margin-right:2px;
  padding:1px 5px;
  vertical-align:text-bottom; }
  .bp3-breadcrumbs-collapsed::before{
    background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cg fill='%235C7080'%3e%3ccircle cx='2' cy='8.03' r='2'/%3e%3ccircle cx='14' cy='8.03' r='2'/%3e%3ccircle cx='8' cy='8.03' r='2'/%3e%3c/g%3e%3c/svg%3e") center no-repeat;
    content:"";
    display:block;
    height:16px;
    width:16px; }
  .bp3-breadcrumbs-collapsed:hover{
    background:#bfccd6;
    color:#182026;
    text-decoration:none; }

.bp3-dark .bp3-breadcrumb,
.bp3-dark .bp3-breadcrumbs-collapsed{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumbs > li::after{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumb.bp3-disabled{
  color:rgba(167, 182, 194, 0.6); }

.bp3-dark .bp3-breadcrumb-current{
  color:#f5f8fa; }

.bp3-dark .bp3-breadcrumbs-collapsed{
  background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-breadcrumbs-collapsed:hover{
    background:rgba(16, 22, 26, 0.6);
    color:#f5f8fa; }
.bp3-button{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  min-height:30px;
  min-width:30px; }
  .bp3-button > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-button > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-button::before,
  .bp3-button > *{
    margin-right:7px; }
  .bp3-button:empty::before,
  .bp3-button > :last-child{
    margin-right:0; }
  .bp3-button:empty{
    padding:0 !important; }
  .bp3-button:disabled, .bp3-button.bp3-disabled{
    cursor:not-allowed; }
  .bp3-button.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button.bp3-align-right,
  .bp3-align-right .bp3-button{
    text-align:right; }
  .bp3-button.bp3-align-left,
  .bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-button:not([class*="bp3-intent-"]){
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026; }
    .bp3-button:not([class*="bp3-intent-"]):hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-button:not([class*="bp3-intent-"]):active, .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active:hover, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-button.bp3-intent-primary{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover, .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover{
      background-color:#106ba3;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      background-color:#0e5a8a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-primary:disabled, .bp3-button.bp3-intent-primary.bp3-disabled{
      background-color:rgba(19, 124, 189, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-success{
    background-color:#0f9960;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-success:hover, .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-success:hover{
      background-color:#0d8050;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      background-color:#0a6640;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-success:disabled, .bp3-button.bp3-intent-success.bp3-disabled{
      background-color:rgba(15, 153, 96, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-warning{
    background-color:#d9822b;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover, .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover{
      background-color:#bf7326;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      background-color:#a66321;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-warning:disabled, .bp3-button.bp3-intent-warning.bp3-disabled{
      background-color:rgba(217, 130, 43, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-danger{
    background-color:#db3737;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover, .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover{
      background-color:#c23030;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      background-color:#a82a2a;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-button.bp3-intent-danger:disabled, .bp3-button.bp3-intent-danger.bp3-disabled{
      background-color:rgba(219, 55, 55, 0.5);
      background-image:none;
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
    stroke:#ffffff; }
  .bp3-button.bp3-large,
  .bp3-large .bp3-button{
    min-height:40px;
    min-width:40px;
    font-size:16px;
    padding:5px 15px; }
    .bp3-button.bp3-large::before,
    .bp3-button.bp3-large > *,
    .bp3-large .bp3-button::before,
    .bp3-large .bp3-button > *{
      margin-right:10px; }
    .bp3-button.bp3-large:empty::before,
    .bp3-button.bp3-large > :last-child,
    .bp3-large .bp3-button:empty::before,
    .bp3-large .bp3-button > :last-child{
      margin-right:0; }
  .bp3-button.bp3-small,
  .bp3-small .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-button.bp3-loading{
    position:relative; }
    .bp3-button.bp3-loading[class*="bp3-icon-"]::before{
      visibility:hidden; }
    .bp3-button.bp3-loading .bp3-button-spinner{
      margin:0;
      position:absolute; }
    .bp3-button.bp3-loading > :not(.bp3-button-spinner){
      visibility:hidden; }
  .bp3-button[class*="bp3-icon-"]::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    color:#5c7080; }
  .bp3-button .bp3-icon, .bp3-button .bp3-icon-standard, .bp3-button .bp3-icon-large{
    color:#5c7080; }
    .bp3-button .bp3-icon.bp3-align-right, .bp3-button .bp3-icon-standard.bp3-align-right, .bp3-button .bp3-icon-large.bp3-align-right{
      margin-left:7px; }
  .bp3-button .bp3-icon:first-child:last-child,
  .bp3-button .bp3-spinner + .bp3-icon:last-child{
    margin:0 -7px; }
  .bp3-dark .bp3-button:not([class*="bp3-intent-"]){
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover, .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"])[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-large{
      color:#a7b6c2; }
  .bp3-dark .bp3-button[class*="bp3-intent-"]{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:active, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:disabled, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-disabled{
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(255, 255, 255, 0.3); }
    .bp3-dark .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
      stroke:#8a9ba8; }
  .bp3-button:disabled::before,
  .bp3-button:disabled .bp3-icon, .bp3-button:disabled .bp3-icon-standard, .bp3-button:disabled .bp3-icon-large, .bp3-button.bp3-disabled::before,
  .bp3-button.bp3-disabled .bp3-icon, .bp3-button.bp3-disabled .bp3-icon-standard, .bp3-button.bp3-disabled .bp3-icon-large, .bp3-button[class*="bp3-intent-"]::before,
  .bp3-button[class*="bp3-intent-"] .bp3-icon, .bp3-button[class*="bp3-intent-"] .bp3-icon-standard, .bp3-button[class*="bp3-intent-"] .bp3-icon-large{
    color:inherit !important; }
  .bp3-button.bp3-minimal{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button.bp3-minimal:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-minimal:active, .bp3-button.bp3-minimal.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-minimal:disabled, .bp3-button.bp3-minimal:disabled:hover, .bp3-button.bp3-minimal.bp3-disabled, .bp3-button.bp3-minimal.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-minimal{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-minimal:hover, .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-minimal:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-minimal:disabled, .bp3-dark .bp3-button.bp3-minimal:disabled:hover, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover, .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover, .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover, .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover, .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button.bp3-outlined{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    border:1px solid rgba(24, 32, 38, 0.2);
    -webkit-box-sizing:border-box;
            box-sizing:border-box; }
    .bp3-button.bp3-outlined:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button.bp3-outlined:active, .bp3-button.bp3-outlined.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-outlined{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-outlined:hover, .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button.bp3-outlined:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover, .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover, .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover, .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover, .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-outlined.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
    .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled:hover{
      border-color:rgba(92, 112, 128, 0.1); }
    .bp3-dark .bp3-button.bp3-outlined{
      border-color:rgba(255, 255, 255, 0.4); }
      .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
        border-color:rgba(255, 255, 255, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-primary{
      border-color:rgba(16, 107, 163, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
        border-color:rgba(16, 107, 163, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
        border-color:rgba(72, 175, 240, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
          border-color:rgba(72, 175, 240, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-success{
      border-color:rgba(13, 128, 80, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
        border-color:rgba(13, 128, 80, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
        border-color:rgba(61, 204, 145, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
          border-color:rgba(61, 204, 145, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-warning{
      border-color:rgba(191, 115, 38, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
        border-color:rgba(191, 115, 38, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
        border-color:rgba(255, 179, 102, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
          border-color:rgba(255, 179, 102, 0.2); }
    .bp3-button.bp3-outlined.bp3-intent-danger{
      border-color:rgba(194, 48, 48, 0.6); }
      .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
        border-color:rgba(194, 48, 48, 0.2); }
      .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
        border-color:rgba(255, 115, 115, 0.6); }
        .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
          border-color:rgba(255, 115, 115, 0.2); }

a.bp3-button{
  text-align:center;
  text-decoration:none;
  -webkit-transition:none;
  transition:none; }
  a.bp3-button, a.bp3-button:hover, a.bp3-button:active{
    color:#182026; }
  a.bp3-button.bp3-disabled{
    color:rgba(92, 112, 128, 0.6); }

.bp3-button-text{
  -webkit-box-flex:0;
      -ms-flex:0 1 auto;
          flex:0 1 auto; }

.bp3-button.bp3-align-left .bp3-button-text, .bp3-button.bp3-align-right .bp3-button-text,
.bp3-button-group.bp3-align-left .bp3-button-text,
.bp3-button-group.bp3-align-right .bp3-button-text{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto; }
.bp3-button-group{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex; }
  .bp3-button-group .bp3-button{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    position:relative;
    z-index:4; }
    .bp3-button-group .bp3-button:focus{
      z-index:5; }
    .bp3-button-group .bp3-button:hover{
      z-index:6; }
    .bp3-button-group .bp3-button:active, .bp3-button-group .bp3-button.bp3-active{
      z-index:7; }
    .bp3-button-group .bp3-button:disabled, .bp3-button-group .bp3-button.bp3-disabled{
      z-index:3; }
    .bp3-button-group .bp3-button[class*="bp3-intent-"]{
      z-index:9; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:focus{
        z-index:10; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:hover{
        z-index:11; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:active, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-active{
        z-index:12; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:disabled, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-disabled{
        z-index:8; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:first-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:first-child){
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    border-bottom-right-radius:0;
    border-top-right-radius:0;
    margin-right:-1px; }
  .bp3-button-group.bp3-minimal .bp3-button{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-button-group.bp3-minimal .bp3-button:hover{
      background:rgba(167, 182, 194, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026;
      text-decoration:none; }
    .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
      background:rgba(115, 134, 148, 0.3);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#182026; }
    .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
      background:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed; }
      .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button-group.bp3-minimal .bp3-button{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:inherit; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
        background:none;
        color:rgba(167, 182, 194, 0.6);
        cursor:not-allowed; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
      color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
      color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button-group .bp3-popover-wrapper,
  .bp3-button-group .bp3-popover-target{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button-group .bp3-button.bp3-fill,
  .bp3-button-group.bp3-fill .bp3-button:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-vertical{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column;
    vertical-align:top; }
    .bp3-button-group.bp3-vertical.bp3-fill{
      height:100%;
      width:unset; }
    .bp3-button-group.bp3-vertical .bp3-button{
      margin-right:0 !important;
      width:100%; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:first-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:first-child{
      border-radius:3px 3px 0 0; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:last-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:last-child{
      border-radius:0 0 3px 3px; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:not(:last-child){
      margin-bottom:-1px; }
  .bp3-button-group.bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    margin-right:1px; }
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-button:not(:last-child){
    margin-bottom:1px; }
.bp3-callout{
  font-size:14px;
  line-height:1.5;
  background-color:rgba(138, 155, 168, 0.15);
  border-radius:3px;
  padding:10px 12px 9px;
  position:relative;
  width:100%; }
  .bp3-callout[class*="bp3-icon-"]{
    padding-left:40px; }
    .bp3-callout[class*="bp3-icon-"]::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout.bp3-callout-icon{
    padding-left:40px; }
    .bp3-callout.bp3-callout-icon > .bp3-icon:first-child{
      color:#5c7080;
      left:10px;
      position:absolute;
      top:10px; }
  .bp3-callout .bp3-heading{
    line-height:20px;
    margin-bottom:5px;
    margin-top:0; }
    .bp3-callout .bp3-heading:last-child{
      margin-bottom:0; }
  .bp3-dark .bp3-callout{
    background-color:rgba(138, 155, 168, 0.2); }
    .bp3-dark .bp3-callout[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
  .bp3-callout.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15); }
    .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-primary .bp3-heading{
      color:#106ba3; }
    .bp3-dark .bp3-callout.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-primary .bp3-heading{
        color:#48aff0; }
  .bp3-callout.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15); }
    .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-success .bp3-heading{
      color:#0d8050; }
    .bp3-dark .bp3-callout.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-success .bp3-heading{
        color:#3dcc91; }
  .bp3-callout.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15); }
    .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-warning .bp3-heading{
      color:#bf7326; }
    .bp3-dark .bp3-callout.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-warning .bp3-heading{
        color:#ffb366; }
  .bp3-callout.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15); }
    .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-danger .bp3-heading{
      color:#c23030; }
    .bp3-dark .bp3-callout.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-danger .bp3-heading{
        color:#ff7373; }
  .bp3-running-text .bp3-callout{
    margin:20px 0; }
.bp3-card{
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
  padding:20px;
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-card.bp3-dark,
  .bp3-dark .bp3-card{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-0{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }
  .bp3-elevation-0.bp3-dark,
  .bp3-dark .bp3-elevation-0{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-1{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-1.bp3-dark,
  .bp3-dark .bp3-elevation-1{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-elevation-2{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-2.bp3-dark,
  .bp3-dark .bp3-elevation-2{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4); }

.bp3-elevation-3{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-3.bp3-dark,
  .bp3-dark .bp3-elevation-3{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-elevation-4{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-4.bp3-dark,
  .bp3-dark .bp3-elevation-4{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:hover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  cursor:pointer; }
  .bp3-card.bp3-interactive:hover.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:hover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:active{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  opacity:0.9;
  -webkit-transition-duration:0;
          transition-duration:0; }
  .bp3-card.bp3-interactive:active.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:active{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-collapse{
  height:0;
  overflow-y:hidden;
  -webkit-transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-collapse .bp3-collapse-body{
    -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-collapse .bp3-collapse-body[aria-hidden="true"]{
      display:none; }

.bp3-context-menu .bp3-popover-target{
  display:block; }

.bp3-context-menu-popover-target{
  position:fixed; }

.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-dialog-container{
  opacity:1;
  -webkit-transform:scale(1);
          transform:scale(1);
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  min-height:100%;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  width:100%; }
  .bp3-dialog-container.bp3-overlay-enter > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5); }
  .bp3-dialog-container.bp3-overlay-enter-active > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear-active > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-dialog-container.bp3-overlay-exit > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-dialog-container.bp3-overlay-exit-active > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }

.bp3-dialog{
  background:#ebf1f5;
  border-radius:6px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:30px 0;
  padding-bottom:20px;
  pointer-events:all;
  -webkit-user-select:text;
     -moz-user-select:text;
      -ms-user-select:text;
          user-select:text;
  width:500px; }
  .bp3-dialog:focus{
    outline:0; }
  .bp3-dialog.bp3-dark,
  .bp3-dark .bp3-dialog{
    background:#293742;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-dialog-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background:#ffffff;
  border-radius:6px 6px 0 0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding-left:20px;
  padding-right:5px;
  z-index:30; }
  .bp3-dialog-header .bp3-icon-large,
  .bp3-dialog-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-dialog-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-dialog-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-dialog-header{
    background:#30404d;
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-dialog-header .bp3-icon-large,
    .bp3-dark .bp3-dialog-header .bp3-icon{
      color:#a7b6c2; }

.bp3-dialog-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  margin:20px; }

.bp3-dialog-footer{
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  margin:0 20px; }

.bp3-dialog-footer-actions{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:end;
      -ms-flex-pack:end;
          justify-content:flex-end; }
  .bp3-dialog-footer-actions .bp3-button{
    margin-left:10px; }
.bp3-multistep-dialog-panels{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }

.bp3-multistep-dialog-left-panel{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column; }
  .bp3-dark .bp3-multistep-dialog-left-panel{
    background:#202b33; }

.bp3-multistep-dialog-right-panel{
  background-color:#f5f8fa;
  border-left:1px solid rgba(16, 22, 26, 0.15);
  border-radius:0 0 6px 0;
  -webkit-box-flex:3;
      -ms-flex:3;
          flex:3;
  min-width:0; }
  .bp3-dark .bp3-multistep-dialog-right-panel{
    background-color:#293742;
    border-left:1px solid rgba(16, 22, 26, 0.4); }

.bp3-multistep-dialog-footer{
  background-color:#ffffff;
  border-radius:0 0 6px 0;
  border-top:1px solid rgba(16, 22, 26, 0.15);
  padding:10px; }
  .bp3-dark .bp3-multistep-dialog-footer{
    background:#30404d;
    border-top:1px solid rgba(16, 22, 26, 0.4); }

.bp3-dialog-step-container{
  background-color:#f5f8fa;
  border-bottom:1px solid rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-dialog-step-container{
    background:#293742;
    border-bottom:1px solid rgba(16, 22, 26, 0.4); }
  .bp3-dialog-step-container.bp3-dialog-step-viewed{
    background-color:#ffffff; }
    .bp3-dark .bp3-dialog-step-container.bp3-dialog-step-viewed{
      background:#30404d; }

.bp3-dialog-step{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#f5f8fa;
  border-radius:6px;
  cursor:not-allowed;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:4px;
  padding:6px 14px; }
  .bp3-dark .bp3-dialog-step{
    background:#293742; }
  .bp3-dialog-step-viewed .bp3-dialog-step{
    background-color:#ffffff;
    cursor:pointer; }
    .bp3-dark .bp3-dialog-step-viewed .bp3-dialog-step{
      background:#30404d; }
  .bp3-dialog-step:hover{
    background-color:#f5f8fa; }
    .bp3-dark .bp3-dialog-step:hover{
      background:#293742; }

.bp3-dialog-step-icon{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:rgba(92, 112, 128, 0.6);
  border-radius:50%;
  color:#ffffff;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:25px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  width:25px; }
  .bp3-dark .bp3-dialog-step-icon{
    background-color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#2b95d6; }
  .bp3-dialog-step-viewed .bp3-dialog-step-icon{
    background-color:#8a9ba8; }

.bp3-dialog-step-title{
  color:rgba(92, 112, 128, 0.6);
  -webkit-box-flex:1;
      -ms-flex:1;
          flex:1;
  padding-left:10px; }
  .bp3-dark .bp3-dialog-step-title{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-title{
    color:#2b95d6; }
  .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
    color:#182026; }
    .bp3-dark .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
      color:#f5f8fa; }
.bp3-drawer{
  background:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0;
  padding:0; }
  .bp3-drawer:focus{
    outline:0; }
  .bp3-drawer.bp3-position-top{
    height:50%;
    left:0;
    right:0;
    top:0; }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter, .bp3-drawer.bp3-position-top.bp3-overlay-appear{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%); }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter-active, .bp3-drawer.bp3-position-top.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit-active{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-bottom{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter-active, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-left{
    bottom:0;
    left:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter, .bp3-drawer.bp3-position-left.bp3-overlay-appear{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%); }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter-active, .bp3-drawer.bp3-position-left.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit-active{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-position-right{
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter, .bp3-drawer.bp3-position-right.bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter-active, .bp3-drawer.bp3-position-right.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right):not(.bp3-vertical){
    bottom:0;
    right:0;
    top:0;
    width:50%; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right).bp3-vertical{
    bottom:0;
    height:50%;
    left:0;
    right:0; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-delay:0;
              transition-delay:0;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-drawer.bp3-dark,
  .bp3-dark .bp3-drawer{
    background:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }

.bp3-drawer-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border-radius:0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  min-height:40px;
  padding:5px;
  padding-left:20px;
  position:relative; }
  .bp3-drawer-header .bp3-icon-large,
  .bp3-drawer-header .bp3-icon{
    color:#5c7080;
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px; }
  .bp3-drawer-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:inherit;
    margin:0; }
    .bp3-drawer-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-drawer-header{
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-drawer-header .bp3-icon-large,
    .bp3-dark .bp3-drawer-header .bp3-icon{
      color:#a7b6c2; }

.bp3-drawer-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  line-height:18px;
  overflow:auto; }

.bp3-drawer-footer{
  -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  padding:10px 20px;
  position:relative; }
  .bp3-dark .bp3-drawer-footer{
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4); }
.bp3-editable-text{
  cursor:text;
  display:inline-block;
  max-width:100%;
  position:relative;
  vertical-align:top;
  white-space:nowrap; }
  .bp3-editable-text::before{
    bottom:-3px;
    left:-3px;
    position:absolute;
    right:-3px;
    top:-3px;
    border-radius:3px;
    content:"";
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#137cbd; }
  .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4); }
  .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#0f9960; }
  .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4); }
  .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#d9822b; }
  .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4); }
  .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#db3737; }
  .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4); }
  .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15); }
  .bp3-dark .bp3-editable-text.bp3-editable-text-editing::before{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#48aff0; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4);
            box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#3dcc91; }
  .bp3-dark .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4);
            box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#ffb366; }
  .bp3-dark .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4);
            box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#ff7373; }
  .bp3-dark .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4);
            box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-editable-text-input,
.bp3-editable-text-content{
  color:inherit;
  display:inherit;
  font:inherit;
  letter-spacing:inherit;
  max-width:inherit;
  min-width:inherit;
  position:relative;
  resize:none;
  text-transform:inherit;
  vertical-align:top; }

.bp3-editable-text-input{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0;
  white-space:pre-wrap;
  width:100%; }
  .bp3-editable-text-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-editable-text-input:focus{
    outline:none; }
  .bp3-editable-text-input::-ms-clear{
    display:none; }

.bp3-editable-text-content{
  overflow:hidden;
  padding-right:2px;
  text-overflow:ellipsis;
  white-space:pre; }
  .bp3-editable-text-editing > .bp3-editable-text-content{
    left:0;
    position:absolute;
    visibility:hidden; }
  .bp3-editable-text-placeholder > .bp3-editable-text-content{
    color:rgba(92, 112, 128, 0.6); }
    .bp3-dark .bp3-editable-text-placeholder > .bp3-editable-text-content{
      color:rgba(167, 182, 194, 0.6); }

.bp3-editable-text.bp3-multiline{
  display:block; }
  .bp3-editable-text.bp3-multiline .bp3-editable-text-content{
    overflow:auto;
    white-space:pre-wrap;
    word-wrap:break-word; }
.bp3-divider{
  border-bottom:1px solid rgba(16, 22, 26, 0.15);
  border-right:1px solid rgba(16, 22, 26, 0.15);
  margin:5px; }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-control-group{
  -webkit-transform:translateZ(0);
          transform:translateZ(0);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:stretch;
      -ms-flex-align:stretch;
          align-items:stretch; }
  .bp3-control-group > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select,
  .bp3-control-group .bp3-input,
  .bp3-control-group .bp3-select{
    position:relative; }
  .bp3-control-group .bp3-input{
    border-radius:inherit;
    z-index:2; }
    .bp3-control-group .bp3-input:focus{
      border-radius:3px;
      z-index:14; }
    .bp3-control-group .bp3-input[class*="bp3-intent"]{
      z-index:13; }
      .bp3-control-group .bp3-input[class*="bp3-intent"]:focus{
        z-index:15; }
    .bp3-control-group .bp3-input[readonly], .bp3-control-group .bp3-input:disabled, .bp3-control-group .bp3-input.bp3-disabled{
      z-index:1; }
  .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input{
    z-index:13; }
    .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input:focus{
      z-index:15; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select select,
  .bp3-control-group .bp3-select select{
    -webkit-transform:translateZ(0);
            transform:translateZ(0);
    border-radius:inherit;
    z-index:4; }
    .bp3-control-group .bp3-button:focus,
    .bp3-control-group .bp3-html-select select:focus,
    .bp3-control-group .bp3-select select:focus{
      z-index:5; }
    .bp3-control-group .bp3-button:hover,
    .bp3-control-group .bp3-html-select select:hover,
    .bp3-control-group .bp3-select select:hover{
      z-index:6; }
    .bp3-control-group .bp3-button:active,
    .bp3-control-group .bp3-html-select select:active,
    .bp3-control-group .bp3-select select:active{
      z-index:7; }
    .bp3-control-group .bp3-button[readonly], .bp3-control-group .bp3-button:disabled, .bp3-control-group .bp3-button.bp3-disabled,
    .bp3-control-group .bp3-html-select select[readonly],
    .bp3-control-group .bp3-html-select select:disabled,
    .bp3-control-group .bp3-html-select select.bp3-disabled,
    .bp3-control-group .bp3-select select[readonly],
    .bp3-control-group .bp3-select select:disabled,
    .bp3-control-group .bp3-select select.bp3-disabled{
      z-index:3; }
    .bp3-control-group .bp3-button[class*="bp3-intent"],
    .bp3-control-group .bp3-html-select select[class*="bp3-intent"],
    .bp3-control-group .bp3-select select[class*="bp3-intent"]{
      z-index:9; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:focus{
        z-index:10; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:hover{
        z-index:11; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:active{
        z-index:12; }
      .bp3-control-group .bp3-button[class*="bp3-intent"][readonly], .bp3-control-group .bp3-button[class*="bp3-intent"]:disabled, .bp3-control-group .bp3-button[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"].bp3-disabled{
        z-index:8; }
  .bp3-control-group .bp3-input-group > .bp3-icon,
  .bp3-control-group .bp3-input-group > .bp3-button,
  .bp3-control-group .bp3-input-group > .bp3-input-left-container,
  .bp3-control-group .bp3-input-group > .bp3-input-action{
    z-index:16; }
  .bp3-control-group .bp3-select::after,
  .bp3-control-group .bp3-html-select::after,
  .bp3-control-group .bp3-select > .bp3-icon,
  .bp3-control-group .bp3-html-select > .bp3-icon{
    z-index:17; }
  .bp3-control-group .bp3-select:focus-within{
    z-index:5; }
  .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:-1px; }
  .bp3-control-group:not(.bp3-vertical) > .bp3-divider:not(:first-child){
    margin-left:6px; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > *:not(.bp3-divider){
    margin-right:0; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > .bp3-button + .bp3-button{
    margin-left:1px; }
  .bp3-control-group .bp3-popover-wrapper,
  .bp3-control-group .bp3-popover-target{
    border-radius:inherit; }
  .bp3-control-group > :first-child{
    border-radius:3px 0 0 3px; }
  .bp3-control-group > :last-child{
    border-radius:0 3px 3px 0;
    margin-right:0; }
  .bp3-control-group > :only-child{
    border-radius:3px;
    margin-right:0; }
  .bp3-control-group .bp3-input-group .bp3-button{
    border-radius:3px; }
  .bp3-control-group .bp3-numeric-input:not(:first-child) .bp3-input-group{
    border-bottom-left-radius:0;
    border-top-left-radius:0; }
  .bp3-control-group.bp3-fill{
    width:100%; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-fill > *:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-vertical{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-control-group.bp3-vertical > *{
      margin-top:-1px; }
    .bp3-control-group.bp3-vertical > :first-child{
      border-radius:3px 3px 0 0;
      margin-top:0; }
    .bp3-control-group.bp3-vertical > :last-child{
      border-radius:0 0 3px 3px; }
.bp3-control{
  cursor:pointer;
  display:block;
  margin-bottom:10px;
  position:relative;
  text-transform:none; }
  .bp3-control input:checked ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control:hover input:checked ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control:not(.bp3-align-right){
    padding-left:26px; }
    .bp3-control:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-26px; }
  .bp3-control.bp3-align-right{
    padding-right:26px; }
    .bp3-control.bp3-align-right .bp3-control-indicator{
      margin-right:-26px; }
  .bp3-control.bp3-disabled{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-control.bp3-inline{
    display:inline-block;
    margin-right:20px; }
  .bp3-control input{
    left:0;
    opacity:0;
    position:absolute;
    top:0;
    z-index:-1; }
  .bp3-control .bp3-control-indicator{
    background-clip:padding-box;
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    border:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    cursor:pointer;
    display:inline-block;
    font-size:16px;
    height:1em;
    margin-right:10px;
    margin-top:-3px;
    position:relative;
    -webkit-user-select:none;
       -moz-user-select:none;
        -ms-user-select:none;
            user-select:none;
    vertical-align:middle;
    width:1em; }
    .bp3-control .bp3-control-indicator::before{
      content:"";
      display:block;
      height:1em;
      width:1em; }
  .bp3-control:hover .bp3-control-indicator{
    background-color:#ebf1f5; }
  .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
    background:#d8e1e8;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    cursor:not-allowed; }
  .bp3-control input:focus ~ .bp3-control-indicator{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:2px;
    -moz-outline-radius:6px; }
  .bp3-control.bp3-align-right .bp3-control-indicator{
    float:right;
    margin-left:10px;
    margin-top:1px; }
  .bp3-control.bp3-large{
    font-size:16px; }
    .bp3-control.bp3-large:not(.bp3-align-right){
      padding-left:30px; }
      .bp3-control.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
        margin-left:-30px; }
    .bp3-control.bp3-large.bp3-align-right{
      padding-right:30px; }
      .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
        margin-right:-30px; }
    .bp3-control.bp3-large .bp3-control-indicator{
      font-size:20px; }
    .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-top:0; }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    color:#ffffff; }
  .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background:#0e5a8a;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    background-color:#106ba3;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    background-color:#0e5a8a;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-control.bp3-checkbox .bp3-control-indicator{
    border-radius:3px; }
  .bp3-control.bp3-checkbox input:checked ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-radio .bp3-control-indicator{
    border-radius:50%; }
  .bp3-control.bp3-radio input:checked ~ .bp3-control-indicator::before{
    background-image:radial-gradient(#ffffff, #ffffff 28%, transparent 32%); }
  .bp3-control.bp3-radio input:checked:disabled ~ .bp3-control-indicator::before{
    opacity:0.5; }
  .bp3-control.bp3-radio input:focus ~ .bp3-control-indicator{
    -moz-outline-radius:16px; }
  .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(167, 182, 194, 0.5); }
  .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(115, 134, 148, 0.5); }
  .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(92, 112, 128, 0.5); }
  .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5); }
    .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5); }
    .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch:not(.bp3-align-right){
    padding-left:38px; }
    .bp3-control.bp3-switch:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-38px; }
  .bp3-control.bp3-switch.bp3-align-right{
    padding-right:38px; }
    .bp3-control.bp3-switch.bp3-align-right .bp3-control-indicator{
      margin-right:-38px; }
  .bp3-control.bp3-switch .bp3-control-indicator{
    border:none;
    border-radius:1.75em;
    -webkit-box-shadow:none !important;
            box-shadow:none !important;
    min-width:1.75em;
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:auto; }
    .bp3-control.bp3-switch .bp3-control-indicator::before{
      background:#ffffff;
      border-radius:50%;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
      height:calc(1em - 4px);
      left:0;
      margin:2px;
      position:absolute;
      -webkit-transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      width:calc(1em - 4px); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    left:calc(100% - 1em); }
  .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right){
    padding-left:45px; }
    .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-45px; }
  .bp3-control.bp3-switch.bp3-large.bp3-align-right{
    padding-right:45px; }
    .bp3-control.bp3-switch.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-right:-45px; }
  .bp3-dark .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.7); }
  .bp3-dark .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.9); }
  .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(57, 75, 89, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-dark .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-dark .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch .bp3-control-indicator::before{
    background:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-control.bp3-switch .bp3-switch-inner-text{
    font-size:0.7em;
    text-align:center; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:first-child{
    line-height:0;
    margin-left:0.5em;
    margin-right:1.2em;
    visibility:hidden; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:last-child{
    line-height:1em;
    margin-left:1.2em;
    margin-right:0.5em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:first-child{
    line-height:1em;
    visibility:visible; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:last-child{
    line-height:0;
    visibility:hidden; }
  .bp3-dark .bp3-control{
    color:#f5f8fa; }
    .bp3-dark .bp3-control.bp3-disabled{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-control .bp3-control-indicator{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-control:hover .bp3-control-indicator{
      background-color:#30404d; }
    .bp3-dark .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
      background:#202b33;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-control input:disabled ~ .bp3-control-indicator{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      cursor:not-allowed; }
    .bp3-dark .bp3-control.bp3-checkbox input:disabled:checked ~ .bp3-control-indicator, .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
      color:rgba(167, 182, 194, 0.6); }
.bp3-file-input{
  cursor:pointer;
  display:inline-block;
  height:30px;
  position:relative; }
  .bp3-file-input input{
    margin:0;
    min-width:200px;
    opacity:0; }
    .bp3-file-input input:disabled + .bp3-file-upload-input,
    .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
      background:rgba(206, 217, 224, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      resize:none; }
      .bp3-file-input input:disabled + .bp3-file-upload-input::after,
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
        background-color:rgba(206, 217, 224, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(92, 112, 128, 0.6);
        cursor:not-allowed;
        outline:none; }
        .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active:hover,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active:hover{
          background:rgba(206, 217, 224, 0.7); }
      .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input, .bp3-dark
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
        background:rgba(57, 75, 89, 0.5);
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after, .bp3-dark
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
          background-color:rgba(57, 75, 89, 0.5);
          background-image:none;
          -webkit-box-shadow:none;
                  box-shadow:none;
          color:rgba(167, 182, 194, 0.6); }
          .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-dark
          .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active{
            background:rgba(57, 75, 89, 0.7); }
  .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#182026; }
  .bp3-dark .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#f5f8fa; }
  .bp3-file-input.bp3-fill{
    width:100%; }
  .bp3-file-input.bp3-large,
  .bp3-large .bp3-file-input{
    height:40px; }
  .bp3-file-input .bp3-file-upload-input-custom-text::after{
    content:attr(bp3-button-text); }

.bp3-file-upload-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle;
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:rgba(92, 112, 128, 0.6);
  left:0;
  padding-right:80px;
  position:absolute;
  right:0;
  top:0;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-file-upload-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-file-upload-input:focus, .bp3-file-upload-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-file-upload-input[type="search"], .bp3-file-upload-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-file-upload-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-file-upload-input:disabled, .bp3-file-upload-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-file-upload-input::after{
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    color:#182026;
    min-height:24px;
    min-width:24px;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    border-radius:3px;
    content:"Browse";
    line-height:24px;
    margin:3px;
    position:absolute;
    right:0;
    text-align:center;
    top:0;
    width:70px; }
    .bp3-file-upload-input::after:hover{
      background-clip:padding-box;
      background-color:#ebf1f5;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
    .bp3-file-upload-input::after:active, .bp3-file-upload-input::after.bp3-active{
      background-color:#d8e1e8;
      background-image:none;
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-file-upload-input::after:disabled, .bp3-file-upload-input::after.bp3-disabled{
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(92, 112, 128, 0.6);
      cursor:not-allowed;
      outline:none; }
      .bp3-file-upload-input::after:disabled.bp3-active, .bp3-file-upload-input::after:disabled.bp3-active:hover, .bp3-file-upload-input::after.bp3-disabled.bp3-active, .bp3-file-upload-input::after.bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-file-upload-input:hover::after{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-file-upload-input:active::after{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-large .bp3-file-upload-input{
    font-size:16px;
    height:40px;
    line-height:40px;
    padding-right:95px; }
    .bp3-large .bp3-file-upload-input[type="search"], .bp3-large .bp3-file-upload-input.bp3-round{
      padding:0 15px; }
    .bp3-large .bp3-file-upload-input::after{
      min-height:30px;
      min-width:30px;
      line-height:30px;
      margin:5px;
      width:85px; }
  .bp3-dark .bp3-file-upload-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:disabled, .bp3-dark .bp3-file-upload-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::after{
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover, .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover{
        background-color:#30404d;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        background-color:#202b33;
        background-image:none;
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
      .bp3-dark .bp3-file-upload-input::after:disabled, .bp3-dark .bp3-file-upload-input::after.bp3-disabled{
        background-color:rgba(57, 75, 89, 0.5);
        background-image:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-upload-input::after:disabled.bp3-active, .bp3-dark .bp3-file-upload-input::after.bp3-disabled.bp3-active{
          background:rgba(57, 75, 89, 0.7); }
      .bp3-dark .bp3-file-upload-input::after .bp3-button-spinner .bp3-spinner-head{
        background:rgba(16, 22, 26, 0.5);
        stroke:#8a9ba8; }
    .bp3-dark .bp3-file-upload-input:hover::after{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:active::after{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
.bp3-file-upload-input::after{
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
.bp3-form-group{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0 0 15px; }
  .bp3-form-group label.bp3-label{
    margin-bottom:5px; }
  .bp3-form-group .bp3-control{
    margin-top:7px; }
  .bp3-form-group .bp3-form-helper-text{
    color:#5c7080;
    font-size:12px;
    margin-top:5px; }
  .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#106ba3; }
  .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#0d8050; }
  .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#bf7326; }
  .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#c23030; }
  .bp3-form-group.bp3-inline{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row; }
    .bp3-form-group.bp3-inline.bp3-large label.bp3-label{
      line-height:40px;
      margin:0 10px 0 0; }
    .bp3-form-group.bp3-inline label.bp3-label{
      line-height:30px;
      margin:0 10px 0 0; }
  .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-dark .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#48aff0; }
  .bp3-dark .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#3dcc91; }
  .bp3-dark .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#ffb366; }
  .bp3-dark .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#ff7373; }
  .bp3-dark .bp3-form-group .bp3-form-helper-text{
    color:#a7b6c2; }
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(167, 182, 194, 0.6) !important; }
.bp3-input-group{
  display:block;
  position:relative; }
  .bp3-input-group .bp3-input{
    position:relative;
    width:100%; }
    .bp3-input-group .bp3-input:not(:first-child){
      padding-left:30px; }
    .bp3-input-group .bp3-input:not(:last-child){
      padding-right:30px; }
  .bp3-input-group .bp3-input-action,
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-button,
  .bp3-input-group > .bp3-icon{
    position:absolute;
    top:0; }
    .bp3-input-group .bp3-input-action:first-child,
    .bp3-input-group > .bp3-input-left-container:first-child,
    .bp3-input-group > .bp3-button:first-child,
    .bp3-input-group > .bp3-icon:first-child{
      left:0; }
    .bp3-input-group .bp3-input-action:last-child,
    .bp3-input-group > .bp3-input-left-container:last-child,
    .bp3-input-group > .bp3-button:last-child,
    .bp3-input-group > .bp3-icon:last-child{
      right:0; }
  .bp3-input-group .bp3-button{
    min-height:24px;
    min-width:24px;
    margin:3px;
    padding:0 7px; }
    .bp3-input-group .bp3-button:empty{
      padding:0; }
  .bp3-input-group > .bp3-input-left-container,
  .bp3-input-group > .bp3-icon{
    z-index:1; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon{
    color:#5c7080; }
    .bp3-input-group > .bp3-input-left-container > .bp3-icon:empty,
    .bp3-input-group > .bp3-icon:empty{
      font-family:"Icons16", sans-serif;
      font-size:16px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased; }
  .bp3-input-group > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group > .bp3-icon,
  .bp3-input-group .bp3-input-action > .bp3-spinner{
    margin:7px; }
  .bp3-input-group .bp3-tag{
    margin:5px; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus),
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
    color:#5c7080; }
    .bp3-dark .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus), .bp3-dark
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
      color:#a7b6c2; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large{
      color:#5c7080; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled,
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled{
    color:rgba(92, 112, 128, 0.6) !important; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-large{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-input-group.bp3-disabled{
    cursor:not-allowed; }
    .bp3-input-group.bp3-disabled .bp3-icon{
      color:rgba(92, 112, 128, 0.6); }
  .bp3-input-group.bp3-large .bp3-button{
    min-height:30px;
    min-width:30px;
    margin:5px; }
  .bp3-input-group.bp3-large > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-large > .bp3-icon,
  .bp3-input-group.bp3-large .bp3-input-action > .bp3-spinner{
    margin:12px; }
  .bp3-input-group.bp3-large .bp3-input{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input-group.bp3-large .bp3-input[type="search"], .bp3-input-group.bp3-large .bp3-input.bp3-round{
      padding:0 15px; }
    .bp3-input-group.bp3-large .bp3-input:not(:first-child){
      padding-left:40px; }
    .bp3-input-group.bp3-large .bp3-input:not(:last-child){
      padding-right:40px; }
  .bp3-input-group.bp3-small .bp3-button{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small .bp3-tag{
    min-height:20px;
    min-width:20px;
    margin:2px; }
  .bp3-input-group.bp3-small > .bp3-input-left-container > .bp3-icon,
  .bp3-input-group.bp3-small > .bp3-icon,
  .bp3-input-group.bp3-small .bp3-input-action > .bp3-spinner{
    margin:4px; }
  .bp3-input-group.bp3-small .bp3-input{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input-group.bp3-small .bp3-input[type="search"], .bp3-input-group.bp3-small .bp3-input.bp3-round{
      padding:0 12px; }
    .bp3-input-group.bp3-small .bp3-input:not(:first-child){
      padding-left:24px; }
    .bp3-input-group.bp3-small .bp3-input:not(:last-child){
      padding-right:24px; }
  .bp3-input-group.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-input-group.bp3-round .bp3-button,
  .bp3-input-group.bp3-round .bp3-input,
  .bp3-input-group.bp3-round .bp3-tag{
    border-radius:30px; }
  .bp3-dark .bp3-input-group .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-input-group.bp3-disabled .bp3-icon{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-input-group.bp3-intent-primary .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input-group.bp3-intent-primary .bp3-input:disabled, .bp3-input-group.bp3-intent-primary .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-primary > .bp3-icon{
    color:#106ba3; }
    .bp3-dark .bp3-input-group.bp3-intent-primary > .bp3-icon{
      color:#48aff0; }
  .bp3-input-group.bp3-intent-success .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input-group.bp3-intent-success .bp3-input:disabled, .bp3-input-group.bp3-intent-success .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-success > .bp3-icon{
    color:#0d8050; }
    .bp3-dark .bp3-input-group.bp3-intent-success > .bp3-icon{
      color:#3dcc91; }
  .bp3-input-group.bp3-intent-warning .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input-group.bp3-intent-warning .bp3-input:disabled, .bp3-input-group.bp3-intent-warning .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-warning > .bp3-icon{
    color:#bf7326; }
    .bp3-dark .bp3-input-group.bp3-intent-warning > .bp3-icon{
      color:#ffb366; }
  .bp3-input-group.bp3-intent-danger .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input-group.bp3-intent-danger .bp3-input:disabled, .bp3-input-group.bp3-intent-danger .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-danger > .bp3-icon{
    color:#c23030; }
    .bp3-dark .bp3-input-group.bp3-intent-danger > .bp3-icon{
      color:#ff7373; }
.bp3-input{
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  background:#ffffff;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  color:#182026;
  font-size:14px;
  font-weight:400;
  height:30px;
  line-height:30px;
  outline:none;
  padding:0 10px;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  vertical-align:middle; }
  .bp3-input::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input:focus, .bp3-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-input[type="search"], .bp3-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-input:disabled, .bp3-input.bp3-disabled{
    background:rgba(206, 217, 224, 0.5);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    resize:none; }
  .bp3-input.bp3-large{
    font-size:16px;
    height:40px;
    line-height:40px; }
    .bp3-input.bp3-large[type="search"], .bp3-input.bp3-large.bp3-round{
      padding:0 15px; }
  .bp3-input.bp3-small{
    font-size:12px;
    height:24px;
    line-height:24px;
    padding-left:8px;
    padding-right:8px; }
    .bp3-input.bp3-small[type="search"], .bp3-input.bp3-small.bp3-round{
      padding:0 12px; }
  .bp3-input.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-dark .bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input:disabled, .bp3-dark .bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-input.bp3-intent-primary{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input.bp3-intent-primary:disabled, .bp3-input.bp3-intent-primary.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary:focus{
        -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #137cbd;
                box-shadow:inset 0 0 0 1px #137cbd; }
      .bp3-dark .bp3-input.bp3-intent-primary:disabled, .bp3-dark .bp3-input.bp3-intent-primary.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-success{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input.bp3-intent-success:disabled, .bp3-input.bp3-intent-success.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-success{
      -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success:focus{
        -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #0f9960;
                box-shadow:inset 0 0 0 1px #0f9960; }
      .bp3-dark .bp3-input.bp3-intent-success:disabled, .bp3-dark .bp3-input.bp3-intent-success.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-warning{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input.bp3-intent-warning:disabled, .bp3-input.bp3-intent-warning.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning:focus{
        -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #d9822b;
                box-shadow:inset 0 0 0 1px #d9822b; }
      .bp3-dark .bp3-input.bp3-intent-warning:disabled, .bp3-dark .bp3-input.bp3-intent-warning.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-danger{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input.bp3-intent-danger:disabled, .bp3-input.bp3-intent-danger.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger:focus{
        -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #db3737;
                box-shadow:inset 0 0 0 1px #db3737; }
      .bp3-dark .bp3-input.bp3-intent-danger:disabled, .bp3-dark .bp3-input.bp3-intent-danger.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input::-ms-clear{
    display:none; }
textarea.bp3-input{
  max-width:100%;
  padding:10px; }
  textarea.bp3-input, textarea.bp3-input.bp3-large, textarea.bp3-input.bp3-small{
    height:auto;
    line-height:inherit; }
  textarea.bp3-input.bp3-small{
    padding:8px; }
  .bp3-dark textarea.bp3-input{
    background:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark textarea.bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input:disabled, .bp3-dark textarea.bp3-input.bp3-disabled{
      background:rgba(57, 75, 89, 0.5);
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
label.bp3-label{
  display:block;
  margin-bottom:15px;
  margin-top:0; }
  label.bp3-label .bp3-html-select,
  label.bp3-label .bp3-input,
  label.bp3-label .bp3-select,
  label.bp3-label .bp3-slider,
  label.bp3-label .bp3-popover-wrapper{
    display:block;
    margin-top:5px;
    text-transform:none; }
  label.bp3-label .bp3-button-group{
    margin-top:5px; }
  label.bp3-label .bp3-select select,
  label.bp3-label .bp3-html-select select{
    font-weight:400;
    vertical-align:top;
    width:100%; }
  label.bp3-label.bp3-disabled,
  label.bp3-label.bp3-disabled .bp3-text-muted{
    color:rgba(92, 112, 128, 0.6); }
  label.bp3-label.bp3-inline{
    line-height:30px; }
    label.bp3-label.bp3-inline .bp3-html-select,
    label.bp3-label.bp3-inline .bp3-input,
    label.bp3-label.bp3-inline .bp3-input-group,
    label.bp3-label.bp3-inline .bp3-select,
    label.bp3-label.bp3-inline .bp3-popover-wrapper{
      display:inline-block;
      margin:0 0 0 5px;
      vertical-align:top; }
    label.bp3-label.bp3-inline .bp3-button-group{
      margin:0 0 0 5px; }
    label.bp3-label.bp3-inline .bp3-input-group .bp3-input{
      margin-left:0; }
    label.bp3-label.bp3-inline.bp3-large{
      line-height:40px; }
  label.bp3-label:not(.bp3-inline) .bp3-popover-target{
    display:block; }
  .bp3-dark label.bp3-label{
    color:#f5f8fa; }
    .bp3-dark label.bp3-label.bp3-disabled,
    .bp3-dark label.bp3-label.bp3-disabled .bp3-text-muted{
      color:rgba(167, 182, 194, 0.6); }
.bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button{
  -webkit-box-flex:1;
      -ms-flex:1 1 14px;
          flex:1 1 14px;
  min-height:0;
  padding:0;
  width:30px; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:first-child{
    border-radius:0 3px 0 0; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:last-child{
    border-radius:0 0 3px 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:first-child{
  border-radius:3px 0 0 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:last-child{
  border-radius:0 0 0 3px; }

.bp3-numeric-input.bp3-large .bp3-button-group.bp3-vertical > .bp3-button{
  width:40px; }

form{
  display:block; }
.bp3-html-select select,
.bp3-select select{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  font-size:14px;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  padding:5px 10px;
  text-align:left;
  vertical-align:middle;
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  -moz-appearance:none;
  -webkit-appearance:none;
  border-radius:3px;
  height:30px;
  padding:0 25px 0 10px;
  width:100%; }
  .bp3-html-select select > *, .bp3-select select > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-html-select select > .bp3-fill, .bp3-select select > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-html-select select::before,
  .bp3-select select::before, .bp3-html-select select > *, .bp3-select select > *{
    margin-right:7px; }
  .bp3-html-select select:empty::before,
  .bp3-select select:empty::before,
  .bp3-html-select select > :last-child,
  .bp3-select select > :last-child{
    margin-right:0; }
  .bp3-html-select select:hover,
  .bp3-select select:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-html-select select:active,
  .bp3-select select:active, .bp3-html-select select.bp3-active,
  .bp3-select select.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-html-select select:disabled,
  .bp3-select select:disabled, .bp3-html-select select.bp3-disabled,
  .bp3-select select.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-html-select select:disabled.bp3-active,
    .bp3-select select:disabled.bp3-active, .bp3-html-select select:disabled.bp3-active:hover,
    .bp3-select select:disabled.bp3-active:hover, .bp3-html-select select.bp3-disabled.bp3-active,
    .bp3-select select.bp3-disabled.bp3-active, .bp3-html-select select.bp3-disabled.bp3-active:hover,
    .bp3-select select.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }

.bp3-html-select.bp3-minimal select,
.bp3-select.bp3-minimal select{
  background:none;
  -webkit-box-shadow:none;
          box-shadow:none; }
  .bp3-html-select.bp3-minimal select:hover,
  .bp3-select.bp3-minimal select:hover{
    background:rgba(167, 182, 194, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026;
    text-decoration:none; }
  .bp3-html-select.bp3-minimal select:active,
  .bp3-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal select.bp3-active,
  .bp3-select.bp3-minimal select.bp3-active{
    background:rgba(115, 134, 148, 0.3);
    -webkit-box-shadow:none;
            box-shadow:none;
    color:#182026; }
  .bp3-html-select.bp3-minimal select:disabled,
  .bp3-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal select:disabled:hover,
  .bp3-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal select.bp3-disabled,
  .bp3-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal select.bp3-disabled:hover,
  .bp3-select.bp3-minimal select.bp3-disabled:hover{
    background:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
    .bp3-html-select.bp3-minimal select:disabled.bp3-active,
    .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active{
      background:rgba(115, 134, 148, 0.3); }
  .bp3-dark .bp3-html-select.bp3-minimal select, .bp3-html-select.bp3-minimal .bp3-dark select,
  .bp3-dark .bp3-select.bp3-minimal select, .bp3-select.bp3-minimal .bp3-dark select{
    background:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:inherit; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover, .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover{
      background:rgba(138, 155, 168, 0.15); }
    .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:rgba(138, 155, 168, 0.3);
      color:#f5f8fa; }
    .bp3-dark .bp3-html-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal .bp3-dark select:disabled,
    .bp3-dark .bp3-select.bp3-minimal select:disabled, .bp3-select.bp3-minimal .bp3-dark select:disabled, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select:disabled:hover, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover{
      background:none;
      color:rgba(167, 182, 194, 0.6);
      cursor:not-allowed; }
      .bp3-dark .bp3-html-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active{
        background:rgba(138, 155, 168, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-primary,
  .bp3-select.bp3-minimal select.bp3-intent-primary{
    color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover{
      background:rgba(19, 124, 189, 0.15);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:rgba(19, 124, 189, 0.3);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled{
      background:none;
      color:rgba(16, 107, 163, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active{
        background:rgba(19, 124, 189, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
      stroke:#106ba3; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary{
      color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.2);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(72, 175, 240, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-success,
  .bp3-select.bp3-minimal select.bp3-intent-success{
    color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover{
      background:rgba(15, 153, 96, 0.15);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:rgba(15, 153, 96, 0.3);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled{
      background:none;
      color:rgba(13, 128, 80, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active{
        background:rgba(15, 153, 96, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
      stroke:#0d8050; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success{
      color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.2);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(61, 204, 145, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-warning,
  .bp3-select.bp3-minimal select.bp3-intent-warning{
    color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover{
      background:rgba(217, 130, 43, 0.15);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:rgba(217, 130, 43, 0.3);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled{
      background:none;
      color:rgba(191, 115, 38, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active{
        background:rgba(217, 130, 43, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
      stroke:#bf7326; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning{
      color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.2);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(255, 179, 102, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-danger,
  .bp3-select.bp3-minimal select.bp3-intent-danger{
    color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover{
      background:rgba(219, 55, 55, 0.15);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:rgba(219, 55, 55, 0.3);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled{
      background:none;
      color:rgba(194, 48, 48, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active{
        background:rgba(219, 55, 55, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
      stroke:#c23030; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger{
      color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.2);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(255, 115, 115, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }

.bp3-html-select.bp3-large select,
.bp3-select.bp3-large select{
  font-size:16px;
  height:40px;
  padding-right:35px; }

.bp3-dark .bp3-html-select select, .bp3-dark .bp3-select select{
  background-color:#394b59;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
  color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover, .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    background-color:#202b33;
    background-image:none;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-html-select select:disabled, .bp3-dark .bp3-select select:disabled, .bp3-dark .bp3-html-select select.bp3-disabled, .bp3-dark .bp3-select select.bp3-disabled{
    background-color:rgba(57, 75, 89, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-html-select select:disabled.bp3-active, .bp3-dark .bp3-select select:disabled.bp3-active, .bp3-dark .bp3-html-select select.bp3-disabled.bp3-active, .bp3-dark .bp3-select select.bp3-disabled.bp3-active{
      background:rgba(57, 75, 89, 0.7); }
  .bp3-dark .bp3-html-select select .bp3-button-spinner .bp3-spinner-head, .bp3-dark .bp3-select select .bp3-button-spinner .bp3-spinner-head{
    background:rgba(16, 22, 26, 0.5);
    stroke:#8a9ba8; }

.bp3-html-select select:disabled,
.bp3-select select:disabled{
  background-color:rgba(206, 217, 224, 0.5);
  -webkit-box-shadow:none;
          box-shadow:none;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-html-select .bp3-icon,
.bp3-select .bp3-icon, .bp3-select::after{
  color:#5c7080;
  pointer-events:none;
  position:absolute;
  right:7px;
  top:7px; }
  .bp3-html-select .bp3-disabled.bp3-icon,
  .bp3-select .bp3-disabled.bp3-icon, .bp3-disabled.bp3-select::after{
    color:rgba(92, 112, 128, 0.6); }
.bp3-html-select,
.bp3-select{
  display:inline-block;
  letter-spacing:normal;
  position:relative;
  vertical-align:middle; }
  .bp3-html-select select::-ms-expand,
  .bp3-select select::-ms-expand{
    display:none; }
  .bp3-html-select .bp3-icon,
  .bp3-select .bp3-icon{
    color:#5c7080; }
    .bp3-html-select .bp3-icon:hover,
    .bp3-select .bp3-icon:hover{
      color:#182026; }
    .bp3-dark .bp3-html-select .bp3-icon, .bp3-dark
    .bp3-select .bp3-icon{
      color:#a7b6c2; }
      .bp3-dark .bp3-html-select .bp3-icon:hover, .bp3-dark
      .bp3-select .bp3-icon:hover{
        color:#f5f8fa; }
  .bp3-html-select.bp3-large::after,
  .bp3-html-select.bp3-large .bp3-icon,
  .bp3-select.bp3-large::after,
  .bp3-select.bp3-large .bp3-icon{
    right:12px;
    top:12px; }
  .bp3-html-select.bp3-fill,
  .bp3-html-select.bp3-fill select,
  .bp3-select.bp3-fill,
  .bp3-select.bp3-fill select{
    width:100%; }
  .bp3-dark .bp3-html-select option, .bp3-dark
  .bp3-select option{
    background-color:#30404d;
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select option:disabled, .bp3-dark
  .bp3-select option:disabled{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-html-select::after, .bp3-dark
  .bp3-select::after{
    color:#a7b6c2; }

.bp3-select::after{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  content:""; }
.bp3-running-text table, table.bp3-html-table{
  border-spacing:0;
  font-size:14px; }
  .bp3-running-text table th, table.bp3-html-table th,
  .bp3-running-text table td,
  table.bp3-html-table td{
    padding:11px;
    text-align:left;
    vertical-align:top; }
  .bp3-running-text table th, table.bp3-html-table th{
    color:#182026;
    font-weight:600; }
  
  .bp3-running-text table td,
  table.bp3-html-table td{
    color:#182026; }
  .bp3-running-text table tbody tr:first-child th, table.bp3-html-table tbody tr:first-child th,
  .bp3-running-text table tbody tr:first-child td,
  table.bp3-html-table tbody tr:first-child td,
  .bp3-running-text table tfoot tr:first-child th,
  table.bp3-html-table tfoot tr:first-child th,
  .bp3-running-text table tfoot tr:first-child td,
  table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-running-text table th, .bp3-running-text .bp3-dark table th, .bp3-dark table.bp3-html-table th{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table td, .bp3-running-text .bp3-dark table td, .bp3-dark table.bp3-html-table td{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table tbody tr:first-child th, .bp3-running-text .bp3-dark table tbody tr:first-child th, .bp3-dark table.bp3-html-table tbody tr:first-child th,
  .bp3-dark .bp3-running-text table tbody tr:first-child td,
  .bp3-running-text .bp3-dark table tbody tr:first-child td,
  .bp3-dark table.bp3-html-table tbody tr:first-child td,
  .bp3-dark .bp3-running-text table tfoot tr:first-child th,
  .bp3-running-text .bp3-dark table tfoot tr:first-child th,
  .bp3-dark table.bp3-html-table tfoot tr:first-child th,
  .bp3-dark .bp3-running-text table tfoot tr:first-child td,
  .bp3-running-text .bp3-dark table tfoot tr:first-child td,
  .bp3-dark table.bp3-html-table tfoot tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }

table.bp3-html-table.bp3-html-table-condensed th,
table.bp3-html-table.bp3-html-table-condensed td, table.bp3-html-table.bp3-small th,
table.bp3-html-table.bp3-small td{
  padding-bottom:6px;
  padding-top:6px; }

table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
  background:rgba(191, 204, 214, 0.15); }

table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
  -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered tbody tr td,
table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
  -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
  table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
    -webkit-box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
  -webkit-box-shadow:none;
          box-shadow:none; }
  table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-interactive tbody tr:hover td{
  background-color:rgba(191, 204, 214, 0.3);
  cursor:pointer; }

table.bp3-html-table.bp3-interactive tbody tr:active td{
  background-color:rgba(191, 204, 214, 0.4); }

.bp3-dark table.bp3-html-table{ }
  .bp3-dark table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
    background:rgba(92, 112, 128, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td,
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
      -webkit-box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15);
              box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
    -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
    .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:first-child{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:hover td{
    background-color:rgba(92, 112, 128, 0.3);
    cursor:pointer; }
  .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:active td{
    background-color:rgba(92, 112, 128, 0.4); }

.bp3-key-combo{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center; }
  .bp3-key-combo > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-key-combo > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-key-combo::before,
  .bp3-key-combo > *{
    margin-right:5px; }
  .bp3-key-combo:empty::before,
  .bp3-key-combo > :last-child{
    margin-right:0; }

.bp3-hotkey-dialog{
  padding-bottom:0;
  top:40px; }
  .bp3-hotkey-dialog .bp3-dialog-body{
    margin:0;
    padding:0; }
  .bp3-hotkey-dialog .bp3-hotkey-label{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1; }

.bp3-hotkey-column{
  margin:auto;
  max-height:80vh;
  overflow-y:auto;
  padding:30px; }
  .bp3-hotkey-column .bp3-heading{
    margin-bottom:20px; }
    .bp3-hotkey-column .bp3-heading:not(:first-child){
      margin-top:40px; }

.bp3-hotkey{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:justify;
      -ms-flex-pack:justify;
          justify-content:space-between;
  margin-left:0;
  margin-right:0; }
  .bp3-hotkey:not(:last-child){
    margin-bottom:10px; }
.bp3-icon{
  display:inline-block;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  vertical-align:text-bottom; }
  .bp3-icon:not(:empty)::before{
    content:"" !important;
    content:unset !important; }
  .bp3-icon > svg{
    display:block; }
    .bp3-icon > svg:not([fill]){
      fill:currentColor; }

.bp3-icon.bp3-intent-primary, .bp3-icon-standard.bp3-intent-primary, .bp3-icon-large.bp3-intent-primary{
  color:#106ba3; }
  .bp3-dark .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-icon-large.bp3-intent-primary{
    color:#48aff0; }

.bp3-icon.bp3-intent-success, .bp3-icon-standard.bp3-intent-success, .bp3-icon-large.bp3-intent-success{
  color:#0d8050; }
  .bp3-dark .bp3-icon.bp3-intent-success, .bp3-dark .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-icon-large.bp3-intent-success{
    color:#3dcc91; }

.bp3-icon.bp3-intent-warning, .bp3-icon-standard.bp3-intent-warning, .bp3-icon-large.bp3-intent-warning{
  color:#bf7326; }
  .bp3-dark .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-icon-large.bp3-intent-warning{
    color:#ffb366; }

.bp3-icon.bp3-intent-danger, .bp3-icon-standard.bp3-intent-danger, .bp3-icon-large.bp3-intent-danger{
  color:#c23030; }
  .bp3-dark .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-icon-large.bp3-intent-danger{
    color:#ff7373; }

span.bp3-icon-standard{
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon-large{
  font-family:"Icons20", sans-serif;
  font-size:20px;
  font-style:normal;
  font-weight:400;
  line-height:1;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon:empty{
  font-family:"Icons20";
  font-size:inherit;
  font-style:normal;
  font-weight:400;
  line-height:1; }
  span.bp3-icon:empty::before{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased; }

.bp3-icon-add::before{
  content:""; }

.bp3-icon-add-column-left::before{
  content:""; }

.bp3-icon-add-column-right::before{
  content:""; }

.bp3-icon-add-row-bottom::before{
  content:""; }

.bp3-icon-add-row-top::before{
  content:""; }

.bp3-icon-add-to-artifact::before{
  content:""; }

.bp3-icon-add-to-folder::before{
  content:""; }

.bp3-icon-airplane::before{
  content:""; }

.bp3-icon-align-center::before{
  content:""; }

.bp3-icon-align-justify::before{
  content:""; }

.bp3-icon-align-left::before{
  content:""; }

.bp3-icon-align-right::before{
  content:""; }

.bp3-icon-alignment-bottom::before{
  content:""; }

.bp3-icon-alignment-horizontal-center::before{
  content:""; }

.bp3-icon-alignment-left::before{
  content:""; }

.bp3-icon-alignment-right::before{
  content:""; }

.bp3-icon-alignment-top::before{
  content:""; }

.bp3-icon-alignment-vertical-center::before{
  content:""; }

.bp3-icon-annotation::before{
  content:""; }

.bp3-icon-application::before{
  content:""; }

.bp3-icon-applications::before{
  content:""; }

.bp3-icon-archive::before{
  content:""; }

.bp3-icon-arrow-bottom-left::before{
  content:"↙"; }

.bp3-icon-arrow-bottom-right::before{
  content:"↘"; }

.bp3-icon-arrow-down::before{
  content:"↓"; }

.bp3-icon-arrow-left::before{
  content:"←"; }

.bp3-icon-arrow-right::before{
  content:"→"; }

.bp3-icon-arrow-top-left::before{
  content:"↖"; }

.bp3-icon-arrow-top-right::before{
  content:"↗"; }

.bp3-icon-arrow-up::before{
  content:"↑"; }

.bp3-icon-arrows-horizontal::before{
  content:"↔"; }

.bp3-icon-arrows-vertical::before{
  content:"↕"; }

.bp3-icon-asterisk::before{
  content:"*"; }

.bp3-icon-automatic-updates::before{
  content:""; }

.bp3-icon-badge::before{
  content:""; }

.bp3-icon-ban-circle::before{
  content:""; }

.bp3-icon-bank-account::before{
  content:""; }

.bp3-icon-barcode::before{
  content:""; }

.bp3-icon-blank::before{
  content:""; }

.bp3-icon-blocked-person::before{
  content:""; }

.bp3-icon-bold::before{
  content:""; }

.bp3-icon-book::before{
  content:""; }

.bp3-icon-bookmark::before{
  content:""; }

.bp3-icon-box::before{
  content:""; }

.bp3-icon-briefcase::before{
  content:""; }

.bp3-icon-bring-data::before{
  content:""; }

.bp3-icon-build::before{
  content:""; }

.bp3-icon-calculator::before{
  content:""; }

.bp3-icon-calendar::before{
  content:""; }

.bp3-icon-camera::before{
  content:""; }

.bp3-icon-caret-down::before{
  content:"⌄"; }

.bp3-icon-caret-left::before{
  content:"〈"; }

.bp3-icon-caret-right::before{
  content:"〉"; }

.bp3-icon-caret-up::before{
  content:"⌃"; }

.bp3-icon-cell-tower::before{
  content:""; }

.bp3-icon-changes::before{
  content:""; }

.bp3-icon-chart::before{
  content:""; }

.bp3-icon-chat::before{
  content:""; }

.bp3-icon-chevron-backward::before{
  content:""; }

.bp3-icon-chevron-down::before{
  content:""; }

.bp3-icon-chevron-forward::before{
  content:""; }

.bp3-icon-chevron-left::before{
  content:""; }

.bp3-icon-chevron-right::before{
  content:""; }

.bp3-icon-chevron-up::before{
  content:""; }

.bp3-icon-circle::before{
  content:""; }

.bp3-icon-circle-arrow-down::before{
  content:""; }

.bp3-icon-circle-arrow-left::before{
  content:""; }

.bp3-icon-circle-arrow-right::before{
  content:""; }

.bp3-icon-circle-arrow-up::before{
  content:""; }

.bp3-icon-citation::before{
  content:""; }

.bp3-icon-clean::before{
  content:""; }

.bp3-icon-clipboard::before{
  content:""; }

.bp3-icon-cloud::before{
  content:"☁"; }

.bp3-icon-cloud-download::before{
  content:""; }

.bp3-icon-cloud-upload::before{
  content:""; }

.bp3-icon-code::before{
  content:""; }

.bp3-icon-code-block::before{
  content:""; }

.bp3-icon-cog::before{
  content:""; }

.bp3-icon-collapse-all::before{
  content:""; }

.bp3-icon-column-layout::before{
  content:""; }

.bp3-icon-comment::before{
  content:""; }

.bp3-icon-comparison::before{
  content:""; }

.bp3-icon-compass::before{
  content:""; }

.bp3-icon-compressed::before{
  content:""; }

.bp3-icon-confirm::before{
  content:""; }

.bp3-icon-console::before{
  content:""; }

.bp3-icon-contrast::before{
  content:""; }

.bp3-icon-control::before{
  content:""; }

.bp3-icon-credit-card::before{
  content:""; }

.bp3-icon-cross::before{
  content:"✗"; }

.bp3-icon-crown::before{
  content:""; }

.bp3-icon-cube::before{
  content:""; }

.bp3-icon-cube-add::before{
  content:""; }

.bp3-icon-cube-remove::before{
  content:""; }

.bp3-icon-curved-range-chart::before{
  content:""; }

.bp3-icon-cut::before{
  content:""; }

.bp3-icon-dashboard::before{
  content:""; }

.bp3-icon-data-lineage::before{
  content:""; }

.bp3-icon-database::before{
  content:""; }

.bp3-icon-delete::before{
  content:""; }

.bp3-icon-delta::before{
  content:"Δ"; }

.bp3-icon-derive-column::before{
  content:""; }

.bp3-icon-desktop::before{
  content:""; }

.bp3-icon-diagnosis::before{
  content:""; }

.bp3-icon-diagram-tree::before{
  content:""; }

.bp3-icon-direction-left::before{
  content:""; }

.bp3-icon-direction-right::before{
  content:""; }

.bp3-icon-disable::before{
  content:""; }

.bp3-icon-document::before{
  content:""; }

.bp3-icon-document-open::before{
  content:""; }

.bp3-icon-document-share::before{
  content:""; }

.bp3-icon-dollar::before{
  content:"$"; }

.bp3-icon-dot::before{
  content:"•"; }

.bp3-icon-double-caret-horizontal::before{
  content:""; }

.bp3-icon-double-caret-vertical::before{
  content:""; }

.bp3-icon-double-chevron-down::before{
  content:""; }

.bp3-icon-double-chevron-left::before{
  content:""; }

.bp3-icon-double-chevron-right::before{
  content:""; }

.bp3-icon-double-chevron-up::before{
  content:""; }

.bp3-icon-doughnut-chart::before{
  content:""; }

.bp3-icon-download::before{
  content:""; }

.bp3-icon-drag-handle-horizontal::before{
  content:""; }

.bp3-icon-drag-handle-vertical::before{
  content:""; }

.bp3-icon-draw::before{
  content:""; }

.bp3-icon-drive-time::before{
  content:""; }

.bp3-icon-duplicate::before{
  content:""; }

.bp3-icon-edit::before{
  content:"✎"; }

.bp3-icon-eject::before{
  content:"⏏"; }

.bp3-icon-endorsed::before{
  content:""; }

.bp3-icon-envelope::before{
  content:"✉"; }

.bp3-icon-equals::before{
  content:""; }

.bp3-icon-eraser::before{
  content:""; }

.bp3-icon-error::before{
  content:""; }

.bp3-icon-euro::before{
  content:"€"; }

.bp3-icon-exchange::before{
  content:""; }

.bp3-icon-exclude-row::before{
  content:""; }

.bp3-icon-expand-all::before{
  content:""; }

.bp3-icon-export::before{
  content:""; }

.bp3-icon-eye-off::before{
  content:""; }

.bp3-icon-eye-on::before{
  content:""; }

.bp3-icon-eye-open::before{
  content:""; }

.bp3-icon-fast-backward::before{
  content:""; }

.bp3-icon-fast-forward::before{
  content:""; }

.bp3-icon-feed::before{
  content:""; }

.bp3-icon-feed-subscribed::before{
  content:""; }

.bp3-icon-film::before{
  content:""; }

.bp3-icon-filter::before{
  content:""; }

.bp3-icon-filter-keep::before{
  content:""; }

.bp3-icon-filter-list::before{
  content:""; }

.bp3-icon-filter-open::before{
  content:""; }

.bp3-icon-filter-remove::before{
  content:""; }

.bp3-icon-flag::before{
  content:"⚑"; }

.bp3-icon-flame::before{
  content:""; }

.bp3-icon-flash::before{
  content:""; }

.bp3-icon-floppy-disk::before{
  content:""; }

.bp3-icon-flow-branch::before{
  content:""; }

.bp3-icon-flow-end::before{
  content:""; }

.bp3-icon-flow-linear::before{
  content:""; }

.bp3-icon-flow-review::before{
  content:""; }

.bp3-icon-flow-review-branch::before{
  content:""; }

.bp3-icon-flows::before{
  content:""; }

.bp3-icon-folder-close::before{
  content:""; }

.bp3-icon-folder-new::before{
  content:""; }

.bp3-icon-folder-open::before{
  content:""; }

.bp3-icon-folder-shared::before{
  content:""; }

.bp3-icon-folder-shared-open::before{
  content:""; }

.bp3-icon-follower::before{
  content:""; }

.bp3-icon-following::before{
  content:""; }

.bp3-icon-font::before{
  content:""; }

.bp3-icon-fork::before{
  content:""; }

.bp3-icon-form::before{
  content:""; }

.bp3-icon-full-circle::before{
  content:""; }

.bp3-icon-full-stacked-chart::before{
  content:""; }

.bp3-icon-fullscreen::before{
  content:""; }

.bp3-icon-function::before{
  content:""; }

.bp3-icon-gantt-chart::before{
  content:""; }

.bp3-icon-geolocation::before{
  content:""; }

.bp3-icon-geosearch::before{
  content:""; }

.bp3-icon-git-branch::before{
  content:""; }

.bp3-icon-git-commit::before{
  content:""; }

.bp3-icon-git-merge::before{
  content:""; }

.bp3-icon-git-new-branch::before{
  content:""; }

.bp3-icon-git-pull::before{
  content:""; }

.bp3-icon-git-push::before{
  content:""; }

.bp3-icon-git-repo::before{
  content:""; }

.bp3-icon-glass::before{
  content:""; }

.bp3-icon-globe::before{
  content:""; }

.bp3-icon-globe-network::before{
  content:""; }

.bp3-icon-graph::before{
  content:""; }

.bp3-icon-graph-remove::before{
  content:""; }

.bp3-icon-greater-than::before{
  content:""; }

.bp3-icon-greater-than-or-equal-to::before{
  content:""; }

.bp3-icon-grid::before{
  content:""; }

.bp3-icon-grid-view::before{
  content:""; }

.bp3-icon-group-objects::before{
  content:""; }

.bp3-icon-grouped-bar-chart::before{
  content:""; }

.bp3-icon-hand::before{
  content:""; }

.bp3-icon-hand-down::before{
  content:""; }

.bp3-icon-hand-left::before{
  content:""; }

.bp3-icon-hand-right::before{
  content:""; }

.bp3-icon-hand-up::before{
  content:""; }

.bp3-icon-header::before{
  content:""; }

.bp3-icon-header-one::before{
  content:""; }

.bp3-icon-header-two::before{
  content:""; }

.bp3-icon-headset::before{
  content:""; }

.bp3-icon-heart::before{
  content:"♥"; }

.bp3-icon-heart-broken::before{
  content:""; }

.bp3-icon-heat-grid::before{
  content:""; }

.bp3-icon-heatmap::before{
  content:""; }

.bp3-icon-help::before{
  content:"?"; }

.bp3-icon-helper-management::before{
  content:""; }

.bp3-icon-highlight::before{
  content:""; }

.bp3-icon-history::before{
  content:""; }

.bp3-icon-home::before{
  content:"⌂"; }

.bp3-icon-horizontal-bar-chart::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-asc::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-desc::before{
  content:""; }

.bp3-icon-horizontal-distribution::before{
  content:""; }

.bp3-icon-id-number::before{
  content:""; }

.bp3-icon-image-rotate-left::before{
  content:""; }

.bp3-icon-image-rotate-right::before{
  content:""; }

.bp3-icon-import::before{
  content:""; }

.bp3-icon-inbox::before{
  content:""; }

.bp3-icon-inbox-filtered::before{
  content:""; }

.bp3-icon-inbox-geo::before{
  content:""; }

.bp3-icon-inbox-search::before{
  content:""; }

.bp3-icon-inbox-update::before{
  content:""; }

.bp3-icon-info-sign::before{
  content:"ℹ"; }

.bp3-icon-inheritance::before{
  content:""; }

.bp3-icon-inner-join::before{
  content:""; }

.bp3-icon-insert::before{
  content:""; }

.bp3-icon-intersection::before{
  content:""; }

.bp3-icon-ip-address::before{
  content:""; }

.bp3-icon-issue::before{
  content:""; }

.bp3-icon-issue-closed::before{
  content:""; }

.bp3-icon-issue-new::before{
  content:""; }

.bp3-icon-italic::before{
  content:""; }

.bp3-icon-join-table::before{
  content:""; }

.bp3-icon-key::before{
  content:""; }

.bp3-icon-key-backspace::before{
  content:""; }

.bp3-icon-key-command::before{
  content:""; }

.bp3-icon-key-control::before{
  content:""; }

.bp3-icon-key-delete::before{
  content:""; }

.bp3-icon-key-enter::before{
  content:""; }

.bp3-icon-key-escape::before{
  content:""; }

.bp3-icon-key-option::before{
  content:""; }

.bp3-icon-key-shift::before{
  content:""; }

.bp3-icon-key-tab::before{
  content:""; }

.bp3-icon-known-vehicle::before{
  content:""; }

.bp3-icon-lab-test::before{
  content:""; }

.bp3-icon-label::before{
  content:""; }

.bp3-icon-layer::before{
  content:""; }

.bp3-icon-layers::before{
  content:""; }

.bp3-icon-layout::before{
  content:""; }

.bp3-icon-layout-auto::before{
  content:""; }

.bp3-icon-layout-balloon::before{
  content:""; }

.bp3-icon-layout-circle::before{
  content:""; }

.bp3-icon-layout-grid::before{
  content:""; }

.bp3-icon-layout-group-by::before{
  content:""; }

.bp3-icon-layout-hierarchy::before{
  content:""; }

.bp3-icon-layout-linear::before{
  content:""; }

.bp3-icon-layout-skew-grid::before{
  content:""; }

.bp3-icon-layout-sorted-clusters::before{
  content:""; }

.bp3-icon-learning::before{
  content:""; }

.bp3-icon-left-join::before{
  content:""; }

.bp3-icon-less-than::before{
  content:""; }

.bp3-icon-less-than-or-equal-to::before{
  content:""; }

.bp3-icon-lifesaver::before{
  content:""; }

.bp3-icon-lightbulb::before{
  content:""; }

.bp3-icon-link::before{
  content:""; }

.bp3-icon-list::before{
  content:"☰"; }

.bp3-icon-list-columns::before{
  content:""; }

.bp3-icon-list-detail-view::before{
  content:""; }

.bp3-icon-locate::before{
  content:""; }

.bp3-icon-lock::before{
  content:""; }

.bp3-icon-log-in::before{
  content:""; }

.bp3-icon-log-out::before{
  content:""; }

.bp3-icon-manual::before{
  content:""; }

.bp3-icon-manually-entered-data::before{
  content:""; }

.bp3-icon-map::before{
  content:""; }

.bp3-icon-map-create::before{
  content:""; }

.bp3-icon-map-marker::before{
  content:""; }

.bp3-icon-maximize::before{
  content:""; }

.bp3-icon-media::before{
  content:""; }

.bp3-icon-menu::before{
  content:""; }

.bp3-icon-menu-closed::before{
  content:""; }

.bp3-icon-menu-open::before{
  content:""; }

.bp3-icon-merge-columns::before{
  content:""; }

.bp3-icon-merge-links::before{
  content:""; }

.bp3-icon-minimize::before{
  content:""; }

.bp3-icon-minus::before{
  content:"−"; }

.bp3-icon-mobile-phone::before{
  content:""; }

.bp3-icon-mobile-video::before{
  content:""; }

.bp3-icon-moon::before{
  content:""; }

.bp3-icon-more::before{
  content:""; }

.bp3-icon-mountain::before{
  content:""; }

.bp3-icon-move::before{
  content:""; }

.bp3-icon-mugshot::before{
  content:""; }

.bp3-icon-multi-select::before{
  content:""; }

.bp3-icon-music::before{
  content:""; }

.bp3-icon-new-drawing::before{
  content:""; }

.bp3-icon-new-grid-item::before{
  content:""; }

.bp3-icon-new-layer::before{
  content:""; }

.bp3-icon-new-layers::before{
  content:""; }

.bp3-icon-new-link::before{
  content:""; }

.bp3-icon-new-object::before{
  content:""; }

.bp3-icon-new-person::before{
  content:""; }

.bp3-icon-new-prescription::before{
  content:""; }

.bp3-icon-new-text-box::before{
  content:""; }

.bp3-icon-ninja::before{
  content:""; }

.bp3-icon-not-equal-to::before{
  content:""; }

.bp3-icon-notifications::before{
  content:""; }

.bp3-icon-notifications-updated::before{
  content:""; }

.bp3-icon-numbered-list::before{
  content:""; }

.bp3-icon-numerical::before{
  content:""; }

.bp3-icon-office::before{
  content:""; }

.bp3-icon-offline::before{
  content:""; }

.bp3-icon-oil-field::before{
  content:""; }

.bp3-icon-one-column::before{
  content:""; }

.bp3-icon-outdated::before{
  content:""; }

.bp3-icon-page-layout::before{
  content:""; }

.bp3-icon-panel-stats::before{
  content:""; }

.bp3-icon-panel-table::before{
  content:""; }

.bp3-icon-paperclip::before{
  content:""; }

.bp3-icon-paragraph::before{
  content:""; }

.bp3-icon-path::before{
  content:""; }

.bp3-icon-path-search::before{
  content:""; }

.bp3-icon-pause::before{
  content:""; }

.bp3-icon-people::before{
  content:""; }

.bp3-icon-percentage::before{
  content:""; }

.bp3-icon-person::before{
  content:""; }

.bp3-icon-phone::before{
  content:"☎"; }

.bp3-icon-pie-chart::before{
  content:""; }

.bp3-icon-pin::before{
  content:""; }

.bp3-icon-pivot::before{
  content:""; }

.bp3-icon-pivot-table::before{
  content:""; }

.bp3-icon-play::before{
  content:""; }

.bp3-icon-plus::before{
  content:"+"; }

.bp3-icon-polygon-filter::before{
  content:""; }

.bp3-icon-power::before{
  content:""; }

.bp3-icon-predictive-analysis::before{
  content:""; }

.bp3-icon-prescription::before{
  content:""; }

.bp3-icon-presentation::before{
  content:""; }

.bp3-icon-print::before{
  content:"⎙"; }

.bp3-icon-projects::before{
  content:""; }

.bp3-icon-properties::before{
  content:""; }

.bp3-icon-property::before{
  content:""; }

.bp3-icon-publish-function::before{
  content:""; }

.bp3-icon-pulse::before{
  content:""; }

.bp3-icon-random::before{
  content:""; }

.bp3-icon-record::before{
  content:""; }

.bp3-icon-redo::before{
  content:""; }

.bp3-icon-refresh::before{
  content:""; }

.bp3-icon-regression-chart::before{
  content:""; }

.bp3-icon-remove::before{
  content:""; }

.bp3-icon-remove-column::before{
  content:""; }

.bp3-icon-remove-column-left::before{
  content:""; }

.bp3-icon-remove-column-right::before{
  content:""; }

.bp3-icon-remove-row-bottom::before{
  content:""; }

.bp3-icon-remove-row-top::before{
  content:""; }

.bp3-icon-repeat::before{
  content:""; }

.bp3-icon-reset::before{
  content:""; }

.bp3-icon-resolve::before{
  content:""; }

.bp3-icon-rig::before{
  content:""; }

.bp3-icon-right-join::before{
  content:""; }

.bp3-icon-ring::before{
  content:""; }

.bp3-icon-rotate-document::before{
  content:""; }

.bp3-icon-rotate-page::before{
  content:""; }

.bp3-icon-satellite::before{
  content:""; }

.bp3-icon-saved::before{
  content:""; }

.bp3-icon-scatter-plot::before{
  content:""; }

.bp3-icon-search::before{
  content:""; }

.bp3-icon-search-around::before{
  content:""; }

.bp3-icon-search-template::before{
  content:""; }

.bp3-icon-search-text::before{
  content:""; }

.bp3-icon-segmented-control::before{
  content:""; }

.bp3-icon-select::before{
  content:""; }

.bp3-icon-selection::before{
  content:"⦿"; }

.bp3-icon-send-to::before{
  content:""; }

.bp3-icon-send-to-graph::before{
  content:""; }

.bp3-icon-send-to-map::before{
  content:""; }

.bp3-icon-series-add::before{
  content:""; }

.bp3-icon-series-configuration::before{
  content:""; }

.bp3-icon-series-derived::before{
  content:""; }

.bp3-icon-series-filtered::before{
  content:""; }

.bp3-icon-series-search::before{
  content:""; }

.bp3-icon-settings::before{
  content:""; }

.bp3-icon-share::before{
  content:""; }

.bp3-icon-shield::before{
  content:""; }

.bp3-icon-shop::before{
  content:""; }

.bp3-icon-shopping-cart::before{
  content:""; }

.bp3-icon-signal-search::before{
  content:""; }

.bp3-icon-sim-card::before{
  content:""; }

.bp3-icon-slash::before{
  content:""; }

.bp3-icon-small-cross::before{
  content:""; }

.bp3-icon-small-minus::before{
  content:""; }

.bp3-icon-small-plus::before{
  content:""; }

.bp3-icon-small-tick::before{
  content:""; }

.bp3-icon-snowflake::before{
  content:""; }

.bp3-icon-social-media::before{
  content:""; }

.bp3-icon-sort::before{
  content:""; }

.bp3-icon-sort-alphabetical::before{
  content:""; }

.bp3-icon-sort-alphabetical-desc::before{
  content:""; }

.bp3-icon-sort-asc::before{
  content:""; }

.bp3-icon-sort-desc::before{
  content:""; }

.bp3-icon-sort-numerical::before{
  content:""; }

.bp3-icon-sort-numerical-desc::before{
  content:""; }

.bp3-icon-split-columns::before{
  content:""; }

.bp3-icon-square::before{
  content:""; }

.bp3-icon-stacked-chart::before{
  content:""; }

.bp3-icon-star::before{
  content:"★"; }

.bp3-icon-star-empty::before{
  content:"☆"; }

.bp3-icon-step-backward::before{
  content:""; }

.bp3-icon-step-chart::before{
  content:""; }

.bp3-icon-step-forward::before{
  content:""; }

.bp3-icon-stop::before{
  content:""; }

.bp3-icon-stopwatch::before{
  content:""; }

.bp3-icon-strikethrough::before{
  content:""; }

.bp3-icon-style::before{
  content:""; }

.bp3-icon-swap-horizontal::before{
  content:""; }

.bp3-icon-swap-vertical::before{
  content:""; }

.bp3-icon-symbol-circle::before{
  content:""; }

.bp3-icon-symbol-cross::before{
  content:""; }

.bp3-icon-symbol-diamond::before{
  content:""; }

.bp3-icon-symbol-square::before{
  content:""; }

.bp3-icon-symbol-triangle-down::before{
  content:""; }

.bp3-icon-symbol-triangle-up::before{
  content:""; }

.bp3-icon-tag::before{
  content:""; }

.bp3-icon-take-action::before{
  content:""; }

.bp3-icon-taxi::before{
  content:""; }

.bp3-icon-text-highlight::before{
  content:""; }

.bp3-icon-th::before{
  content:""; }

.bp3-icon-th-derived::before{
  content:""; }

.bp3-icon-th-disconnect::before{
  content:""; }

.bp3-icon-th-filtered::before{
  content:""; }

.bp3-icon-th-list::before{
  content:""; }

.bp3-icon-thumbs-down::before{
  content:""; }

.bp3-icon-thumbs-up::before{
  content:""; }

.bp3-icon-tick::before{
  content:"✓"; }

.bp3-icon-tick-circle::before{
  content:""; }

.bp3-icon-time::before{
  content:"⏲"; }

.bp3-icon-timeline-area-chart::before{
  content:""; }

.bp3-icon-timeline-bar-chart::before{
  content:""; }

.bp3-icon-timeline-events::before{
  content:""; }

.bp3-icon-timeline-line-chart::before{
  content:""; }

.bp3-icon-tint::before{
  content:""; }

.bp3-icon-torch::before{
  content:""; }

.bp3-icon-tractor::before{
  content:""; }

.bp3-icon-train::before{
  content:""; }

.bp3-icon-translate::before{
  content:""; }

.bp3-icon-trash::before{
  content:""; }

.bp3-icon-tree::before{
  content:""; }

.bp3-icon-trending-down::before{
  content:""; }

.bp3-icon-trending-up::before{
  content:""; }

.bp3-icon-truck::before{
  content:""; }

.bp3-icon-two-columns::before{
  content:""; }

.bp3-icon-unarchive::before{
  content:""; }

.bp3-icon-underline::before{
  content:"⎁"; }

.bp3-icon-undo::before{
  content:"⎌"; }

.bp3-icon-ungroup-objects::before{
  content:""; }

.bp3-icon-unknown-vehicle::before{
  content:""; }

.bp3-icon-unlock::before{
  content:""; }

.bp3-icon-unpin::before{
  content:""; }

.bp3-icon-unresolve::before{
  content:""; }

.bp3-icon-updated::before{
  content:""; }

.bp3-icon-upload::before{
  content:""; }

.bp3-icon-user::before{
  content:""; }

.bp3-icon-variable::before{
  content:""; }

.bp3-icon-vertical-bar-chart-asc::before{
  content:""; }

.bp3-icon-vertical-bar-chart-desc::before{
  content:""; }

.bp3-icon-vertical-distribution::before{
  content:""; }

.bp3-icon-video::before{
  content:""; }

.bp3-icon-volume-down::before{
  content:""; }

.bp3-icon-volume-off::before{
  content:""; }

.bp3-icon-volume-up::before{
  content:""; }

.bp3-icon-walk::before{
  content:""; }

.bp3-icon-warning-sign::before{
  content:""; }

.bp3-icon-waterfall-chart::before{
  content:""; }

.bp3-icon-widget::before{
  content:""; }

.bp3-icon-widget-button::before{
  content:""; }

.bp3-icon-widget-footer::before{
  content:""; }

.bp3-icon-widget-header::before{
  content:""; }

.bp3-icon-wrench::before{
  content:""; }

.bp3-icon-zoom-in::before{
  content:""; }

.bp3-icon-zoom-out::before{
  content:""; }

.bp3-icon-zoom-to-fit::before{
  content:""; }
.bp3-submenu > .bp3-popover-wrapper{
  display:block; }

.bp3-submenu .bp3-popover-target{
  display:block; }
  .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{ }

.bp3-submenu.bp3-popover{
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0 5px; }
  .bp3-submenu.bp3-popover > .bp3-popover-content{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-submenu.bp3-popover, .bp3-submenu.bp3-popover.bp3-dark{
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-dark .bp3-submenu.bp3-popover > .bp3-popover-content, .bp3-submenu.bp3-popover.bp3-dark > .bp3-popover-content{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
.bp3-menu{
  background:#ffffff;
  border-radius:3px;
  color:#182026;
  list-style:none;
  margin:0;
  min-width:180px;
  padding:5px;
  text-align:left; }

.bp3-menu-divider{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px; }
  .bp3-dark .bp3-menu-divider{
    border-top-color:rgba(255, 255, 255, 0.15); }

.bp3-menu-item{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  border-radius:2px;
  color:inherit;
  line-height:20px;
  padding:5px 7px;
  text-decoration:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-menu-item > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-menu-item > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-menu-item::before,
  .bp3-menu-item > *{
    margin-right:7px; }
  .bp3-menu-item:empty::before,
  .bp3-menu-item > :last-child{
    margin-right:0; }
  .bp3-menu-item > .bp3-fill{
    word-break:break-word; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    background-color:rgba(167, 182, 194, 0.3);
    cursor:pointer;
    text-decoration:none; }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-dark .bp3-menu-item{
    color:inherit; }
    .bp3-dark .bp3-menu-item:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
      background-color:rgba(138, 155, 168, 0.15);
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-disabled{
      background-color:inherit;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-menu-item.bp3-intent-primary{
    color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-primary::before, .bp3-menu-item.bp3-intent-primary::after,
    .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary:active, .bp3-menu-item.bp3-intent-primary:active::before, .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-success{
    color:#0d8050; }
    .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-success::before, .bp3-menu-item.bp3-intent-success::after,
    .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-menu-item.bp3-intent-success:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success:active, .bp3-menu-item.bp3-intent-success:active::before, .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-warning{
    color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-warning::before, .bp3-menu-item.bp3-intent-warning::after,
    .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning:active, .bp3-menu-item.bp3-intent-warning:active::before, .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-danger{
    color:#c23030; }
    .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-danger::before, .bp3-menu-item.bp3-intent-danger::after,
    .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger:active, .bp3-menu-item.bp3-intent-danger:active::before, .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    margin-right:7px; }
  .bp3-menu-item::before,
  .bp3-menu-item > .bp3-icon{
    color:#5c7080;
    margin-top:2px; }
  .bp3-menu-item .bp3-menu-item-label{
    color:#5c7080; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    color:inherit; }
  .bp3-menu-item.bp3-active, .bp3-menu-item:active{
    background-color:rgba(115, 134, 148, 0.3); }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit !important;
    color:rgba(92, 112, 128, 0.6) !important;
    cursor:not-allowed !important;
    outline:none !important; }
    .bp3-menu-item.bp3-disabled::before,
    .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-large .bp3-menu-item{
    font-size:16px;
    line-height:22px;
    padding:9px 7px; }
    .bp3-large .bp3-menu-item .bp3-icon{
      margin-top:3px; }
    .bp3-large .bp3-menu-item::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      margin-right:10px;
      margin-top:1px; }

button.bp3-menu-item{
  background:none;
  border:none;
  text-align:left;
  width:100%; }
.bp3-menu-header{
  border-top:1px solid rgba(16, 22, 26, 0.15);
  display:block;
  margin:5px;
  cursor:default;
  padding-left:2px; }
  .bp3-dark .bp3-menu-header{
    border-top-color:rgba(255, 255, 255, 0.15); }
  .bp3-menu-header:first-of-type{
    border-top:none; }
  .bp3-menu-header > h6{
    color:#182026;
    font-weight:600;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    line-height:17px;
    margin:0;
    padding:10px 7px 0 1px; }
    .bp3-dark .bp3-menu-header > h6{
      color:#f5f8fa; }
  .bp3-menu-header:first-of-type > h6{
    padding-top:0; }
  .bp3-large .bp3-menu-header > h6{
    font-size:18px;
    padding-bottom:5px;
    padding-top:15px; }
  .bp3-large .bp3-menu-header:first-of-type > h6{
    padding-top:0; }

.bp3-dark .bp3-menu{
  background:#30404d;
  color:#f5f8fa; }

.bp3-dark .bp3-menu-item{ }
  .bp3-dark .bp3-menu-item.bp3-intent-primary{
    color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary::before, .bp3-dark .bp3-menu-item.bp3-intent-primary::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#48aff0; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary:active, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-success{
    color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-success::before, .bp3-dark .bp3-menu-item.bp3-intent-success::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#3dcc91; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success:active, .bp3-dark .bp3-menu-item.bp3-intent-success:active::before, .bp3-dark .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning{
    color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning::before, .bp3-dark .bp3-menu-item.bp3-intent-warning::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#ffb366; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning:active, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger{
    color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger::before, .bp3-dark .bp3-menu-item.bp3-intent-danger::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#ff7373; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label,
    .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger:active, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-dark .bp3-menu-item::before,
  .bp3-dark .bp3-menu-item > .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item .bp3-menu-item-label{
    color:#a7b6c2; }
  .bp3-dark .bp3-menu-item.bp3-active, .bp3-dark .bp3-menu-item:active{
    background-color:rgba(138, 155, 168, 0.3); }
  .bp3-dark .bp3-menu-item.bp3-disabled{
    color:rgba(167, 182, 194, 0.6) !important; }
    .bp3-dark .bp3-menu-item.bp3-disabled::before,
    .bp3-dark .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-dark .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(167, 182, 194, 0.6) !important; }

.bp3-dark .bp3-menu-divider,
.bp3-dark .bp3-menu-header{
  border-color:rgba(255, 255, 255, 0.15); }

.bp3-dark .bp3-menu-header > h6{
  color:#f5f8fa; }

.bp3-label .bp3-menu{
  margin-top:5px; }
.bp3-navbar{
  background-color:#ffffff;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  height:50px;
  padding:0 15px;
  position:relative;
  width:100%;
  z-index:10; }
  .bp3-navbar.bp3-dark,
  .bp3-dark .bp3-navbar{
    background-color:#394b59; }
  .bp3-navbar.bp3-dark{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-navbar{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-navbar.bp3-fixed-top{
    left:0;
    position:fixed;
    right:0;
    top:0; }

.bp3-navbar-heading{
  font-size:16px;
  margin-right:15px; }

.bp3-navbar-group{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:50px; }
  .bp3-navbar-group.bp3-align-left{
    float:left; }
  .bp3-navbar-group.bp3-align-right{
    float:right; }

.bp3-navbar-divider{
  border-left:1px solid rgba(16, 22, 26, 0.15);
  height:20px;
  margin:0 10px; }
  .bp3-dark .bp3-navbar-divider{
    border-left-color:rgba(255, 255, 255, 0.15); }
.bp3-non-ideal-state{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  height:100%;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  text-align:center;
  width:100%; }
  .bp3-non-ideal-state > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-non-ideal-state > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-non-ideal-state::before,
  .bp3-non-ideal-state > *{
    margin-bottom:20px; }
  .bp3-non-ideal-state:empty::before,
  .bp3-non-ideal-state > :last-child{
    margin-bottom:0; }
  .bp3-non-ideal-state > *{
    max-width:400px; }

.bp3-non-ideal-state-visual{
  color:rgba(92, 112, 128, 0.6);
  font-size:60px; }
  .bp3-dark .bp3-non-ideal-state-visual{
    color:rgba(167, 182, 194, 0.6); }

.bp3-overflow-list{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:nowrap;
      flex-wrap:nowrap;
  min-width:0; }

.bp3-overflow-list-spacer{
  -ms-flex-negative:1;
      flex-shrink:1;
  width:1px; }

body.bp3-overlay-open{
  overflow:hidden; }

.bp3-overlay{
  bottom:0;
  left:0;
  position:static;
  right:0;
  top:0;
  z-index:20; }
  .bp3-overlay:not(.bp3-overlay-open){
    pointer-events:none; }
  .bp3-overlay.bp3-overlay-container{
    overflow:hidden;
    position:fixed; }
    .bp3-overlay.bp3-overlay-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-scroll-container{
    overflow:auto;
    position:fixed; }
    .bp3-overlay.bp3-overlay-scroll-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-inline{
    display:inline;
    overflow:visible; }

.bp3-overlay-content{
  position:fixed;
  z-index:20; }
  .bp3-overlay-inline .bp3-overlay-content,
  .bp3-overlay-scroll-container .bp3-overlay-content{
    position:absolute; }

.bp3-overlay-backdrop{
  bottom:0;
  left:0;
  position:fixed;
  right:0;
  top:0;
  opacity:1;
  background-color:rgba(16, 22, 26, 0.7);
  overflow:auto;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none;
  z-index:20; }
  .bp3-overlay-backdrop.bp3-overlay-enter, .bp3-overlay-backdrop.bp3-overlay-appear{
    opacity:0; }
  .bp3-overlay-backdrop.bp3-overlay-enter-active, .bp3-overlay-backdrop.bp3-overlay-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop.bp3-overlay-exit{
    opacity:1; }
  .bp3-overlay-backdrop.bp3-overlay-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-overlay-backdrop:focus{
    outline:none; }
  .bp3-overlay-inline .bp3-overlay-backdrop{
    position:absolute; }
.bp3-panel-stack{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack-view{
    background-color:#30404d; }
  .bp3-panel-stack-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack-push .bp3-panel-stack-enter, .bp3-panel-stack-push .bp3-panel-stack-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack-push .bp3-panel-stack-enter-active, .bp3-panel-stack-push .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-push .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-push .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-enter, .bp3-panel-stack-pop .bp3-panel-stack-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter-active, .bp3-panel-stack-pop .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-pop .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-panel-stack2{
  overflow:hidden;
  position:relative; }

.bp3-panel-stack2-header{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  height:30px;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack2-header > span{
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1; }
  .bp3-panel-stack2-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack2-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack2-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack2-view{
  bottom:0;
  left:0;
  position:absolute;
  right:0;
  top:0;
  background-color:#ffffff;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  overflow-y:auto;
  z-index:1; }
  .bp3-dark .bp3-panel-stack2-view{
    background-color:#30404d; }
  .bp3-panel-stack2-view:nth-last-child(n + 4){
    display:none; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter, .bp3-panel-stack2-push .bp3-panel-stack2-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter-active, .bp3-panel-stack2-push .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter, .bp3-panel-stack2-pop .bp3-panel-stack2-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter-active, .bp3-panel-stack2-pop .bp3-panel-stack2-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-delay:0;
          transition-delay:0;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease; }
.bp3-popover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1);
  border-radius:3px;
  display:inline-block;
  z-index:20; }
  .bp3-popover .bp3-popover-arrow{
    height:30px;
    position:absolute;
    width:30px; }
    .bp3-popover .bp3-popover-arrow::before{
      height:20px;
      margin:5px;
      width:20px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover{
    margin-bottom:17px;
    margin-top:-17px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
      bottom:-11px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover{
    margin-left:17px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
      left:-11px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover{
    margin-top:17px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
      top:-11px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover{
    margin-left:-17px;
    margin-right:17px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
      right:-11px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-popover > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-popover > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
    top:-0.3934px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
    right:-0.3934px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
    left:-0.3934px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
    bottom:-0.3934px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-popover .bp3-popover-content{
    background:#ffffff;
    color:inherit; }
  .bp3-popover .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-popover .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-popover .bp3-popover-arrow-fill{
    fill:#ffffff; }
  .bp3-popover-enter > .bp3-popover, .bp3-popover-appear > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3); }
  .bp3-popover-enter-active > .bp3-popover, .bp3-popover-appear-active > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover-exit > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-popover .bp3-popover-content{
    border-radius:3px;
    position:relative; }
  .bp3-popover.bp3-popover-content-sizing .bp3-popover-content{
    max-width:350px;
    padding:20px; }
  .bp3-popover-target + .bp3-overlay .bp3-popover.bp3-popover-content-sizing{
    width:350px; }
  .bp3-popover.bp3-minimal{
    margin:0 !important; }
    .bp3-popover.bp3-minimal .bp3-popover-arrow{
      display:none; }
    .bp3-popover.bp3-minimal.bp3-popover{
      -webkit-transform:scale(1);
              transform:scale(1); }
      .bp3-popover-enter > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-enter-active > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
      .bp3-popover-exit > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-exit-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-delay:0;
                transition-delay:0;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover.bp3-dark,
  .bp3-dark .bp3-popover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-popover .bp3-popover-content{
      background:#30404d;
      color:inherit; }
    .bp3-popover.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-popover .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-popover .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-popover.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-popover .bp3-popover-arrow-fill{
      fill:#30404d; }

.bp3-popover-arrow::before{
  border-radius:2px;
  content:"";
  display:block;
  position:absolute;
  -webkit-transform:rotate(45deg);
          transform:rotate(45deg); }

.bp3-tether-pinned .bp3-popover-arrow{
  display:none; }

.bp3-popover-backdrop{
  background:rgba(255, 255, 255, 0); }

.bp3-transition-container{
  opacity:1;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  z-index:20; }
  .bp3-transition-container.bp3-popover-enter, .bp3-transition-container.bp3-popover-appear{
    opacity:0; }
  .bp3-transition-container.bp3-popover-enter-active, .bp3-transition-container.bp3-popover-appear-active{
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container.bp3-popover-exit{
    opacity:1; }
  .bp3-transition-container.bp3-popover-exit-active{
    opacity:0;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-transition-container:focus{
    outline:none; }
  .bp3-transition-container.bp3-popover-leave .bp3-popover-content{
    pointer-events:none; }
  .bp3-transition-container[data-x-out-of-boundaries]{
    display:none; }

span.bp3-popover-target{
  display:inline-block; }

.bp3-popover-wrapper.bp3-fill{
  width:100%; }

.bp3-portal{
  left:0;
  position:absolute;
  right:0;
  top:0; }
@-webkit-keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }
@keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }

.bp3-progress-bar{
  background:rgba(92, 112, 128, 0.2);
  border-radius:40px;
  display:block;
  height:8px;
  overflow:hidden;
  position:relative;
  width:100%; }
  .bp3-progress-bar .bp3-progress-meter{
    background:linear-gradient(-45deg, rgba(255, 255, 255, 0.2) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.2) 50%, rgba(255, 255, 255, 0.2) 75%, transparent 75%);
    background-color:rgba(92, 112, 128, 0.8);
    background-size:30px 30px;
    border-radius:40px;
    height:100%;
    position:absolute;
    -webkit-transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    width:100%; }
  .bp3-progress-bar:not(.bp3-no-animation):not(.bp3-no-stripes) .bp3-progress-meter{
    animation:linear-progress-bar-stripes 300ms linear infinite reverse; }
  .bp3-progress-bar.bp3-no-stripes .bp3-progress-meter{
    background-image:none; }

.bp3-dark .bp3-progress-bar{
  background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-progress-bar .bp3-progress-meter{
    background-color:#8a9ba8; }

.bp3-progress-bar.bp3-intent-primary .bp3-progress-meter{
  background-color:#137cbd; }

.bp3-progress-bar.bp3-intent-success .bp3-progress-meter{
  background-color:#0f9960; }

.bp3-progress-bar.bp3-intent-warning .bp3-progress-meter{
  background-color:#d9822b; }

.bp3-progress-bar.bp3-intent-danger .bp3-progress-meter{
  background-color:#db3737; }
@-webkit-keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
@keyframes skeleton-glow{
  from{
    background:rgba(206, 217, 224, 0.2);
    border-color:rgba(206, 217, 224, 0.2); }
  to{
    background:rgba(92, 112, 128, 0.2);
    border-color:rgba(92, 112, 128, 0.2); } }
.bp3-skeleton{
  -webkit-animation:1000ms linear infinite alternate skeleton-glow;
          animation:1000ms linear infinite alternate skeleton-glow;
  background:rgba(206, 217, 224, 0.2);
  background-clip:padding-box !important;
  border-color:rgba(206, 217, 224, 0.2) !important;
  border-radius:2px;
  -webkit-box-shadow:none !important;
          box-shadow:none !important;
  color:transparent !important;
  cursor:default;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-skeleton::before, .bp3-skeleton::after,
  .bp3-skeleton *{
    visibility:hidden !important; }
.bp3-slider{
  height:40px;
  min-width:150px;
  width:100%;
  cursor:default;
  outline:none;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-slider:hover{
    cursor:pointer; }
  .bp3-slider:active{
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-slider.bp3-disabled{
    cursor:not-allowed;
    opacity:0.5; }
  .bp3-slider.bp3-slider-unlabeled{
    height:16px; }

.bp3-slider-track,
.bp3-slider-progress{
  height:6px;
  left:0;
  right:0;
  top:5px;
  position:absolute; }

.bp3-slider-track{
  border-radius:3px;
  overflow:hidden; }

.bp3-slider-progress{
  background:rgba(92, 112, 128, 0.2); }
  .bp3-dark .bp3-slider-progress{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-slider-progress.bp3-intent-primary{
    background-color:#137cbd; }
  .bp3-slider-progress.bp3-intent-success{
    background-color:#0f9960; }
  .bp3-slider-progress.bp3-intent-warning{
    background-color:#d9822b; }
  .bp3-slider-progress.bp3-intent-danger{
    background-color:#db3737; }

.bp3-slider-handle{
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  color:#182026;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
  cursor:pointer;
  height:16px;
  left:0;
  position:absolute;
  top:0;
  width:16px; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
  .bp3-slider-handle:active, .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
  .bp3-slider-handle:disabled, .bp3-slider-handle.bp3-disabled{
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed;
    outline:none; }
    .bp3-slider-handle:disabled.bp3-active, .bp3-slider-handle:disabled.bp3-active:hover, .bp3-slider-handle.bp3-disabled.bp3-active, .bp3-slider-handle.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }
  .bp3-slider-handle:focus{
    z-index:1; }
  .bp3-slider-handle:hover{
    background-clip:padding-box;
    background-color:#ebf1f5;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
    cursor:-webkit-grab;
    cursor:grab;
    z-index:2; }
  .bp3-slider-handle.bp3-active{
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-disabled .bp3-slider-handle{
    background:#bfccd6;
    -webkit-box-shadow:none;
            box-shadow:none;
    pointer-events:none; }
  .bp3-dark .bp3-slider-handle{
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover, .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover{
      background-color:#30404d;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#202b33;
      background-image:none;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-slider-handle:disabled, .bp3-dark .bp3-slider-handle.bp3-disabled{
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-slider-handle:disabled.bp3-active, .bp3-dark .bp3-slider-handle.bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-slider-handle .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-slider-handle, .bp3-dark .bp3-slider-handle:hover{
      background-color:#394b59; }
    .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#293742; }
  .bp3-dark .bp3-disabled .bp3-slider-handle{
    background:#5c7080;
    border-color:#5c7080;
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-slider-handle .bp3-slider-label{
    background:#394b59;
    border-radius:3px;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
    color:#f5f8fa;
    margin-left:8px; }
    .bp3-dark .bp3-slider-handle .bp3-slider-label{
      background:#e1e8ed;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
      color:#394b59; }
    .bp3-disabled .bp3-slider-handle .bp3-slider-label{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-slider-handle.bp3-start, .bp3-slider-handle.bp3-end{
    width:8px; }
  .bp3-slider-handle.bp3-start{
    border-bottom-right-radius:0;
    border-top-right-radius:0; }
  .bp3-slider-handle.bp3-end{
    border-bottom-left-radius:0;
    border-top-left-radius:0;
    margin-left:8px; }
    .bp3-slider-handle.bp3-end .bp3-slider-label{
      margin-left:0; }

.bp3-slider-label{
  -webkit-transform:translate(-50%, 20px);
          transform:translate(-50%, 20px);
  display:inline-block;
  font-size:12px;
  line-height:1;
  padding:2px 5px;
  position:absolute;
  vertical-align:top; }

.bp3-slider.bp3-vertical{
  height:150px;
  min-width:40px;
  width:40px; }
  .bp3-slider.bp3-vertical .bp3-slider-track,
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    bottom:0;
    height:auto;
    left:5px;
    top:0;
    width:6px; }
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    top:auto; }
  .bp3-slider.bp3-vertical .bp3-slider-label{
    -webkit-transform:translate(20px, 50%);
            transform:translate(20px, 50%); }
  .bp3-slider.bp3-vertical .bp3-slider-handle{
    top:auto; }
    .bp3-slider.bp3-vertical .bp3-slider-handle .bp3-slider-label{
      margin-left:0;
      margin-top:-8px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end, .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      height:8px;
      margin-left:0;
      width:16px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      border-bottom-right-radius:3px;
      border-top-left-radius:0; }
      .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start .bp3-slider-label{
        -webkit-transform:translate(20px);
                transform:translate(20px); }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end{
      border-bottom-left-radius:0;
      border-bottom-right-radius:0;
      border-top-left-radius:3px;
      margin-bottom:8px; }

@-webkit-keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

@keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

.bp3-spinner{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  overflow:visible;
  vertical-align:middle; }
  .bp3-spinner svg{
    display:block; }
  .bp3-spinner path{
    fill-opacity:0; }
  .bp3-spinner .bp3-spinner-head{
    stroke:rgba(92, 112, 128, 0.8);
    stroke-linecap:round;
    -webkit-transform-origin:center;
            transform-origin:center;
    -webkit-transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-spinner .bp3-spinner-track{
    stroke:rgba(92, 112, 128, 0.2); }

.bp3-spinner-animation{
  -webkit-animation:pt-spinner-animation 500ms linear infinite;
          animation:pt-spinner-animation 500ms linear infinite; }
  .bp3-no-spin > .bp3-spinner-animation{
    -webkit-animation:none;
            animation:none; }

.bp3-dark .bp3-spinner .bp3-spinner-head{
  stroke:#8a9ba8; }

.bp3-dark .bp3-spinner .bp3-spinner-track{
  stroke:rgba(16, 22, 26, 0.5); }

.bp3-spinner.bp3-intent-primary .bp3-spinner-head{
  stroke:#137cbd; }

.bp3-spinner.bp3-intent-success .bp3-spinner-head{
  stroke:#0f9960; }

.bp3-spinner.bp3-intent-warning .bp3-spinner-head{
  stroke:#d9822b; }

.bp3-spinner.bp3-intent-danger .bp3-spinner-head{
  stroke:#db3737; }
.bp3-tabs.bp3-vertical{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-tabs.bp3-vertical > .bp3-tab-list{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start;
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab{
      border-radius:3px;
      padding:0 10px;
      width:100%; }
      .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab[aria-selected="true"]{
        background-color:rgba(19, 124, 189, 0.2);
        -webkit-box-shadow:none;
                box-shadow:none; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab-indicator-wrapper .bp3-tab-indicator{
      background-color:rgba(19, 124, 189, 0.2);
      border-radius:3px;
      bottom:0;
      height:auto;
      left:0;
      right:0;
      top:0; }
  .bp3-tabs.bp3-vertical > .bp3-tab-panel{
    margin-top:0;
    padding-left:20px; }

.bp3-tab-list{
  -webkit-box-align:end;
      -ms-flex-align:end;
          align-items:flex-end;
  border:none;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  list-style:none;
  margin:0;
  padding:0;
  position:relative; }
  .bp3-tab-list > *:not(:last-child){
    margin-right:20px; }

.bp3-tab{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  color:#182026;
  cursor:pointer;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  font-size:14px;
  line-height:30px;
  max-width:100%;
  position:relative;
  vertical-align:top; }
  .bp3-tab a{
    color:inherit;
    display:block;
    text-decoration:none; }
  .bp3-tab-indicator-wrapper ~ .bp3-tab{
    background-color:transparent !important;
    -webkit-box-shadow:none !important;
            box-shadow:none !important; }
  .bp3-tab[aria-disabled="true"]{
    color:rgba(92, 112, 128, 0.6);
    cursor:not-allowed; }
  .bp3-tab[aria-selected="true"]{
    border-radius:0;
    -webkit-box-shadow:inset 0 -3px 0 #106ba3;
            box-shadow:inset 0 -3px 0 #106ba3; }
  .bp3-tab[aria-selected="true"], .bp3-tab:not([aria-disabled="true"]):hover{
    color:#106ba3; }
  .bp3-tab:focus{
    -moz-outline-radius:0; }
  .bp3-large > .bp3-tab{
    font-size:16px;
    line-height:40px; }

.bp3-tab-panel{
  margin-top:20px; }
  .bp3-tab-panel[aria-hidden="true"]{
    display:none; }

.bp3-tab-indicator-wrapper{
  left:0;
  pointer-events:none;
  position:absolute;
  top:0;
  -webkit-transform:translateX(0), translateY(0);
          transform:translateX(0), translateY(0);
  -webkit-transition:height, width, -webkit-transform;
  transition:height, width, -webkit-transform;
  transition:height, transform, width;
  transition:height, transform, width, -webkit-transform;
  -webkit-transition-duration:200ms;
          transition-duration:200ms;
  -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
          transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tab-indicator-wrapper .bp3-tab-indicator{
    background-color:#106ba3;
    bottom:0;
    height:3px;
    left:0;
    position:absolute;
    right:0; }
  .bp3-tab-indicator-wrapper.bp3-no-animation{
    -webkit-transition:none;
    transition:none; }

.bp3-dark .bp3-tab{
  color:#f5f8fa; }
  .bp3-dark .bp3-tab[aria-disabled="true"]{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tab[aria-selected="true"]{
    -webkit-box-shadow:inset 0 -3px 0 #48aff0;
            box-shadow:inset 0 -3px 0 #48aff0; }
  .bp3-dark .bp3-tab[aria-selected="true"], .bp3-dark .bp3-tab:not([aria-disabled="true"]):hover{
    color:#48aff0; }

.bp3-dark .bp3-tab-indicator{
  background-color:#48aff0; }

.bp3-flex-expander{
  -webkit-box-flex:1;
      -ms-flex:1 1;
          flex:1 1; }
.bp3-tag{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  background-color:#5c7080;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:none;
          box-shadow:none;
  color:#f5f8fa;
  font-size:12px;
  line-height:16px;
  max-width:100%;
  min-height:20px;
  min-width:20px;
  padding:2px 6px;
  position:relative; }
  .bp3-tag.bp3-interactive{
    cursor:pointer; }
    .bp3-tag.bp3-interactive:hover{
      background-color:rgba(92, 112, 128, 0.85); }
    .bp3-tag.bp3-interactive.bp3-active, .bp3-tag.bp3-interactive:active{
      background-color:rgba(92, 112, 128, 0.7); }
  .bp3-tag > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag::before,
  .bp3-tag > *{
    margin-right:4px; }
  .bp3-tag:empty::before,
  .bp3-tag > :last-child{
    margin-right:0; }
  .bp3-tag:focus{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:0;
    -moz-outline-radius:6px; }
  .bp3-tag.bp3-round{
    border-radius:30px;
    padding-left:8px;
    padding-right:8px; }
  .bp3-dark .bp3-tag{
    background-color:#bfccd6;
    color:#182026; }
    .bp3-dark .bp3-tag.bp3-interactive{
      cursor:pointer; }
      .bp3-dark .bp3-tag.bp3-interactive:hover{
        background-color:rgba(191, 204, 214, 0.85); }
      .bp3-dark .bp3-tag.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-interactive:active{
        background-color:rgba(191, 204, 214, 0.7); }
    .bp3-dark .bp3-tag > .bp3-icon, .bp3-dark .bp3-tag .bp3-icon-standard, .bp3-dark .bp3-tag .bp3-icon-large{
      fill:currentColor; }
  .bp3-tag > .bp3-icon, .bp3-tag .bp3-icon-standard, .bp3-tag .bp3-icon-large{
    fill:#ffffff; }
  .bp3-tag.bp3-large,
  .bp3-large .bp3-tag{
    font-size:14px;
    line-height:20px;
    min-height:30px;
    min-width:30px;
    padding:5px 10px; }
    .bp3-tag.bp3-large::before,
    .bp3-tag.bp3-large > *,
    .bp3-large .bp3-tag::before,
    .bp3-large .bp3-tag > *{
      margin-right:7px; }
    .bp3-tag.bp3-large:empty::before,
    .bp3-tag.bp3-large > :last-child,
    .bp3-large .bp3-tag:empty::before,
    .bp3-large .bp3-tag > :last-child{
      margin-right:0; }
    .bp3-tag.bp3-large.bp3-round,
    .bp3-large .bp3-tag.bp3-round{
      padding-left:12px;
      padding-right:12px; }
  .bp3-tag.bp3-intent-primary{
    background:#137cbd;
    color:#ffffff; }
    .bp3-tag.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.85); }
      .bp3-tag.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.7); }
  .bp3-tag.bp3-intent-success{
    background:#0f9960;
    color:#ffffff; }
    .bp3-tag.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.85); }
      .bp3-tag.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.7); }
  .bp3-tag.bp3-intent-warning{
    background:#d9822b;
    color:#ffffff; }
    .bp3-tag.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.85); }
      .bp3-tag.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.7); }
  .bp3-tag.bp3-intent-danger{
    background:#db3737;
    color:#ffffff; }
    .bp3-tag.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.85); }
      .bp3-tag.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.7); }
  .bp3-tag.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-tag.bp3-minimal > .bp3-icon, .bp3-tag.bp3-minimal .bp3-icon-standard, .bp3-tag.bp3-minimal .bp3-icon-large{
    fill:#5c7080; }
  .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
    background-color:rgba(138, 155, 168, 0.2);
    color:#182026; }
    .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
        background-color:rgba(92, 112, 128, 0.3); }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
        background-color:rgba(92, 112, 128, 0.4); }
    .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
      color:#f5f8fa; }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
          background-color:rgba(191, 204, 214, 0.3); }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
          background-color:rgba(191, 204, 214, 0.4); }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) > .bp3-icon, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-large{
        fill:#a7b6c2; }
  .bp3-tag.bp3-minimal.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15);
    color:#106ba3; }
    .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-primary > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-large{
      fill:#137cbd; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25);
      color:#48aff0; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
          background-color:rgba(19, 124, 189, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
          background-color:rgba(19, 124, 189, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15);
    color:#0d8050; }
    .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-success > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-large{
      fill:#0f9960; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25);
      color:#3dcc91; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
          background-color:rgba(15, 153, 96, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
          background-color:rgba(15, 153, 96, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15);
    color:#bf7326; }
    .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-warning > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-large{
      fill:#d9822b; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25);
      color:#ffb366; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
          background-color:rgba(217, 130, 43, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
          background-color:rgba(217, 130, 43, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15);
    color:#c23030; }
    .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-danger > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-large{
      fill:#db3737; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25);
      color:#ff7373; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
          background-color:rgba(219, 55, 55, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
          background-color:rgba(219, 55, 55, 0.45); }

.bp3-tag-remove{
  background:none;
  border:none;
  color:inherit;
  cursor:pointer;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin-bottom:-2px;
  margin-right:-6px !important;
  margin-top:-2px;
  opacity:0.5;
  padding:2px;
  padding-left:0; }
  .bp3-tag-remove:hover{
    background:none;
    opacity:0.8;
    text-decoration:none; }
  .bp3-tag-remove:active{
    opacity:1; }
  .bp3-tag-remove:empty::before{
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-style:normal;
    font-weight:400;
    line-height:1;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    content:""; }
  .bp3-large .bp3-tag-remove{
    margin-right:-10px !important;
    padding:0 5px 0 0; }
    .bp3-large .bp3-tag-remove:empty::before{
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-style:normal;
      font-weight:400;
      line-height:1; }
.bp3-tag-input{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  cursor:text;
  height:auto;
  line-height:inherit;
  min-height:30px;
  padding-left:5px;
  padding-right:0; }
  .bp3-tag-input > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag-input > .bp3-tag-input-values{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag-input .bp3-tag-input-icon{
    color:#5c7080;
    margin-left:2px;
    margin-right:7px;
    margin-top:7px; }
  .bp3-tag-input .bp3-tag-input-values{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    -ms-flex-item-align:stretch;
        align-self:stretch;
    -ms-flex-wrap:wrap;
        flex-wrap:wrap;
    margin-right:7px;
    margin-top:5px;
    min-width:0; }
    .bp3-tag-input .bp3-tag-input-values > *{
      -webkit-box-flex:0;
          -ms-flex-positive:0;
              flex-grow:0;
      -ms-flex-negative:0;
          flex-shrink:0; }
    .bp3-tag-input .bp3-tag-input-values > .bp3-fill{
      -webkit-box-flex:1;
          -ms-flex-positive:1;
              flex-grow:1;
      -ms-flex-negative:1;
          flex-shrink:1; }
    .bp3-tag-input .bp3-tag-input-values::before,
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-right:5px; }
    .bp3-tag-input .bp3-tag-input-values:empty::before,
    .bp3-tag-input .bp3-tag-input-values > :last-child{
      margin-right:0; }
    .bp3-tag-input .bp3-tag-input-values:first-child .bp3-input-ghost:first-child{
      padding-left:5px; }
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-bottom:5px; }
  .bp3-tag-input .bp3-tag{
    overflow-wrap:break-word; }
    .bp3-tag-input .bp3-tag.bp3-active{
      outline:rgba(19, 124, 189, 0.6) auto 2px;
      outline-offset:0;
      -moz-outline-radius:6px; }
  .bp3-tag-input .bp3-input-ghost{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    line-height:20px;
    width:80px; }
    .bp3-tag-input .bp3-input-ghost:disabled, .bp3-tag-input .bp3-input-ghost.bp3-disabled{
      cursor:not-allowed; }
  .bp3-tag-input .bp3-button,
  .bp3-tag-input .bp3-spinner{
    margin:3px;
    margin-left:0; }
  .bp3-tag-input .bp3-button{
    min-height:24px;
    min-width:24px;
    padding:0 7px; }
  .bp3-tag-input.bp3-large{
    height:auto;
    min-height:40px; }
    .bp3-tag-input.bp3-large::before,
    .bp3-tag-input.bp3-large > *{
      margin-right:10px; }
    .bp3-tag-input.bp3-large:empty::before,
    .bp3-tag-input.bp3-large > :last-child{
      margin-right:0; }
    .bp3-tag-input.bp3-large .bp3-tag-input-icon{
      margin-left:5px;
      margin-top:10px; }
    .bp3-tag-input.bp3-large .bp3-input-ghost{
      line-height:30px; }
    .bp3-tag-input.bp3-large .bp3-button{
      min-height:30px;
      min-width:30px;
      padding:5px 10px;
      margin:5px;
      margin-left:0; }
    .bp3-tag-input.bp3-large .bp3-spinner{
      margin:8px;
      margin-left:0; }
  .bp3-tag-input.bp3-active{
    background-color:#ffffff;
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-tag-input .bp3-tag-input-icon, .bp3-tag-input.bp3-dark .bp3-tag-input-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-tag-input .bp3-input-ghost, .bp3-tag-input.bp3-dark .bp3-input-ghost{
    color:#f5f8fa; }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-webkit-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-moz-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost:-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::placeholder{
      color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tag-input.bp3-active, .bp3-tag-input.bp3-dark.bp3-active{
    background-color:rgba(16, 22, 26, 0.3);
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-primary, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-success, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-warning, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-danger, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-input-ghost{
  background:none;
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0; }
  .bp3-input-ghost::-webkit-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-moz-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::-ms-input-placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost::placeholder{
    color:rgba(92, 112, 128, 0.6);
    opacity:1; }
  .bp3-input-ghost:focus{
    outline:none !important; }
.bp3-toast{
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  margin:20px 0 0;
  max-width:500px;
  min-width:300px;
  pointer-events:all;
  position:relative !important; }
  .bp3-toast.bp3-toast-enter, .bp3-toast.bp3-toast-appear{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active, .bp3-toast.bp3-toast-appear-active{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-enter ~ .bp3-toast, .bp3-toast.bp3-toast-appear ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active ~ .bp3-toast, .bp3-toast.bp3-toast-appear-active ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
  .bp3-toast.bp3-toast-exit{
    opacity:1;
    -webkit-filter:blur(0);
            filter:blur(0); }
  .bp3-toast.bp3-toast-exit-active{
    opacity:0;
    -webkit-filter:blur(10px);
            filter:blur(10px);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:opacity, filter;
    transition-property:opacity, filter, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast.bp3-toast-exit ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0); }
  .bp3-toast.bp3-toast-exit-active ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px);
    -webkit-transition-delay:50ms;
            transition-delay:50ms;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-toast .bp3-button-group{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    padding:5px;
    padding-left:0; }
  .bp3-toast > .bp3-icon{
    color:#5c7080;
    margin:12px;
    margin-right:0; }
  .bp3-toast.bp3-dark,
  .bp3-dark .bp3-toast{
    background-color:#394b59;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-toast.bp3-dark > .bp3-icon,
    .bp3-dark .bp3-toast > .bp3-icon{
      color:#a7b6c2; }
  .bp3-toast[class*="bp3-intent-"] a{
    color:rgba(255, 255, 255, 0.7); }
    .bp3-toast[class*="bp3-intent-"] a:hover{
      color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] > .bp3-icon{
    color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button, .bp3-toast[class*="bp3-intent-"] .bp3-button::before,
  .bp3-toast[class*="bp3-intent-"] .bp3-button .bp3-icon, .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    color:rgba(255, 255, 255, 0.7) !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:focus{
    outline-color:rgba(255, 255, 255, 0.5); }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:hover{
    background-color:rgba(255, 255, 255, 0.15) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    background-color:rgba(255, 255, 255, 0.3) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button::after{
    background:rgba(255, 255, 255, 0.3) !important; }
  .bp3-toast.bp3-intent-primary{
    background-color:#137cbd;
    color:#ffffff; }
  .bp3-toast.bp3-intent-success{
    background-color:#0f9960;
    color:#ffffff; }
  .bp3-toast.bp3-intent-warning{
    background-color:#d9822b;
    color:#ffffff; }
  .bp3-toast.bp3-intent-danger{
    background-color:#db3737;
    color:#ffffff; }

.bp3-toast-message{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  padding:11px;
  word-break:break-word; }

.bp3-toast-container{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box !important;
  display:-ms-flexbox !important;
  display:flex !important;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  left:0;
  overflow:hidden;
  padding:0 20px 20px;
  pointer-events:none;
  right:0;
  z-index:40; }
  .bp3-toast-container.bp3-toast-container-in-portal{
    position:fixed; }
  .bp3-toast-container.bp3-toast-container-inline{
    position:absolute; }
  .bp3-toast-container.bp3-toast-container-top{
    top:0; }
  .bp3-toast-container.bp3-toast-container-bottom{
    bottom:0;
    -webkit-box-orient:vertical;
    -webkit-box-direction:reverse;
        -ms-flex-direction:column-reverse;
            flex-direction:column-reverse;
    top:auto; }
  .bp3-toast-container.bp3-toast-container-left{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
  .bp3-toast-container.bp3-toast-container-right{
    -webkit-box-align:end;
        -ms-flex-align:end;
            align-items:flex-end; }

.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active) ~ .bp3-toast, .bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active) ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-exit-active ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-leave-active ~ .bp3-toast{
  -webkit-transform:translateY(60px);
          transform:translateY(60px); }
.bp3-tooltip{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1); }
  .bp3-tooltip .bp3-popover-arrow{
    height:22px;
    position:absolute;
    width:22px; }
    .bp3-tooltip .bp3-popover-arrow::before{
      height:14px;
      margin:4px;
      width:14px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip{
    margin-bottom:11px;
    margin-top:-11px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
      bottom:-8px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip{
    margin-left:11px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
      left:-8px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip{
    margin-top:11px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
      top:-8px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip{
    margin-left:-11px;
    margin-right:11px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
      right:-8px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-tooltip > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-tooltip > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
    top:-0.22183px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
    right:-0.22183px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
    left:-0.22183px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
    bottom:-0.22183px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-tooltip .bp3-popover-content{
    background:#394b59;
    color:#f5f8fa; }
  .bp3-tooltip .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-tooltip .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-tooltip .bp3-popover-arrow-fill{
    fill:#394b59; }
  .bp3-popover-enter > .bp3-tooltip, .bp3-popover-appear > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8); }
  .bp3-popover-enter-active > .bp3-tooltip, .bp3-popover-appear-active > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-popover-exit > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8);
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tooltip .bp3-popover-content{
    padding:10px 12px; }
  .bp3-tooltip.bp3-dark,
  .bp3-dark .bp3-tooltip{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-tooltip .bp3-popover-content{
      background:#e1e8ed;
      color:#394b59; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-fill{
      fill:#e1e8ed; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-content{
    background:#137cbd;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-arrow-fill{
    fill:#137cbd; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-content{
    background:#0f9960;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-arrow-fill{
    fill:#0f9960; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-content{
    background:#d9822b;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-arrow-fill{
    fill:#d9822b; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-content{
    background:#db3737;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-arrow-fill{
    fill:#db3737; }

.bp3-tooltip-indicator{
  border-bottom:dotted 1px;
  cursor:help; }
.bp3-tree .bp3-icon, .bp3-tree .bp3-icon-standard, .bp3-tree .bp3-icon-large{
  color:#5c7080; }
  .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-tree .bp3-icon.bp3-intent-success, .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-tree-node-list{
  list-style:none;
  margin:0;
  padding-left:0; }

.bp3-tree-root{
  background-color:transparent;
  cursor:default;
  padding-left:0;
  position:relative; }

.bp3-tree-node-content-0{
  padding-left:0px; }

.bp3-tree-node-content-1{
  padding-left:23px; }

.bp3-tree-node-content-2{
  padding-left:46px; }

.bp3-tree-node-content-3{
  padding-left:69px; }

.bp3-tree-node-content-4{
  padding-left:92px; }

.bp3-tree-node-content-5{
  padding-left:115px; }

.bp3-tree-node-content-6{
  padding-left:138px; }

.bp3-tree-node-content-7{
  padding-left:161px; }

.bp3-tree-node-content-8{
  padding-left:184px; }

.bp3-tree-node-content-9{
  padding-left:207px; }

.bp3-tree-node-content-10{
  padding-left:230px; }

.bp3-tree-node-content-11{
  padding-left:253px; }

.bp3-tree-node-content-12{
  padding-left:276px; }

.bp3-tree-node-content-13{
  padding-left:299px; }

.bp3-tree-node-content-14{
  padding-left:322px; }

.bp3-tree-node-content-15{
  padding-left:345px; }

.bp3-tree-node-content-16{
  padding-left:368px; }

.bp3-tree-node-content-17{
  padding-left:391px; }

.bp3-tree-node-content-18{
  padding-left:414px; }

.bp3-tree-node-content-19{
  padding-left:437px; }

.bp3-tree-node-content-20{
  padding-left:460px; }

.bp3-tree-node-content{
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  height:30px;
  padding-right:5px;
  width:100%; }
  .bp3-tree-node-content:hover{
    background-color:rgba(191, 204, 214, 0.4); }

.bp3-tree-node-caret,
.bp3-tree-node-caret-none{
  min-width:30px; }

.bp3-tree-node-caret{
  color:#5c7080;
  cursor:pointer;
  padding:7px;
  -webkit-transform:rotate(0deg);
          transform:rotate(0deg);
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tree-node-caret:hover{
    color:#182026; }
  .bp3-dark .bp3-tree-node-caret{
    color:#a7b6c2; }
    .bp3-dark .bp3-tree-node-caret:hover{
      color:#f5f8fa; }
  .bp3-tree-node-caret.bp3-tree-node-caret-open{
    -webkit-transform:rotate(90deg);
            transform:rotate(90deg); }
  .bp3-tree-node-caret.bp3-icon-standard::before{
    content:""; }

.bp3-tree-node-icon{
  margin-right:7px;
  position:relative; }

.bp3-tree-node-label{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-label span{
    display:inline; }

.bp3-tree-node-secondary-label{
  padding:0 5px;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-secondary-label .bp3-popover-wrapper,
  .bp3-tree-node-secondary-label .bp3-popover-target{
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-content{
  background-color:inherit;
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-caret,
.bp3-tree-node.bp3-disabled .bp3-tree-node-icon{
  color:rgba(92, 112, 128, 0.6);
  cursor:not-allowed; }

.bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content,
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-standard, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-large{
    color:#ffffff; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret::before{
    color:rgba(255, 255, 255, 0.7); }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret:hover::before{
    color:#ffffff; }

.bp3-dark .bp3-tree-node-content:hover{
  background-color:rgba(92, 112, 128, 0.3); }

.bp3-dark .bp3-tree .bp3-icon, .bp3-dark .bp3-tree .bp3-icon-standard, .bp3-dark .bp3-tree .bp3-icon-large{
  color:#a7b6c2; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-dark .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
.bp3-omnibar{
  -webkit-filter:blur(0);
          filter:blur(0);
  opacity:1;
  background-color:#ffffff;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  left:calc(50% - 250px);
  top:20vh;
  width:500px;
  z-index:21; }
  .bp3-omnibar.bp3-overlay-enter, .bp3-omnibar.bp3-overlay-appear{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2; }
  .bp3-omnibar.bp3-overlay-enter-active, .bp3-omnibar.bp3-overlay-appear-active{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar.bp3-overlay-exit{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1; }
  .bp3-omnibar.bp3-overlay-exit-active{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2;
    -webkit-transition-delay:0;
            transition-delay:0;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-omnibar .bp3-input{
    background-color:transparent;
    border-radius:0; }
    .bp3-omnibar .bp3-input, .bp3-omnibar .bp3-input:focus{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-omnibar .bp3-menu{
    background-color:transparent;
    border-radius:0;
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
    max-height:calc(60vh - 40px);
    overflow:auto; }
    .bp3-omnibar .bp3-menu:empty{
      display:none; }
  .bp3-dark .bp3-omnibar, .bp3-omnibar.bp3-dark{
    background-color:#30404d;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-omnibar-overlay .bp3-overlay-backdrop{
  background-color:rgba(16, 22, 26, 0.2); }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }

.bp3-multi-select{
  min-width:150px; }

.bp3-multi-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto; }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-height:300px;
  max-width:400px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1pY29uLWJyYW5kMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNmZmYiPgogICAgPHBhdGggZD0iTTEwNSAxMjcuM2g0MHYxMi44aC00MHpNNTEuMSA3N0w3NCA5OS45bC0yMy4zIDIzLjMgMTAuNSAxMC41IDIzLjMtMjMuM0w5NSA5OS45IDg0LjUgODkuNCA2MS42IDY2LjV6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNGOUE4MjUiPgogICAgPHBhdGggZD0iTTIwLjIgMTEuOGMtMS42IDAtMS43LjUtMS43IDEgMCAuNC4xLjkuMSAxLjMuMS41LjEuOS4xIDEuMyAwIDEuNy0xLjQgMi4zLTMuNSAyLjNoLS45di0xLjloLjVjMS4xIDAgMS40IDAgMS40LS44IDAtLjMgMC0uNi0uMS0xIDAtLjQtLjEtLjgtLjEtMS4yIDAtMS4zIDAtMS44IDEuMy0yLTEuMy0uMi0xLjMtLjctMS4zLTIgMC0uNC4xLS44LjEtMS4yLjEtLjQuMS0uNy4xLTEgMC0uOC0uNC0uNy0xLjQtLjhoLS41VjQuMWguOWMyLjIgMCAzLjUuNyAzLjUgMi4zIDAgLjQtLjEuOS0uMSAxLjMtLjEuNS0uMS45LS4xIDEuMyAwIC41LjIgMSAxLjcgMXYxLjh6TTEuOCAxMC4xYzEuNiAwIDEuNy0uNSAxLjctMSAwLS40LS4xLS45LS4xLTEuMy0uMS0uNS0uMS0uOS0uMS0xLjMgMC0xLjYgMS40LTIuMyAzLjUtMi4zaC45djEuOWgtLjVjLTEgMC0xLjQgMC0xLjQuOCAwIC4zIDAgLjYuMSAxIDAgLjIuMS42LjEgMSAwIDEuMyAwIDEuOC0xLjMgMkM2IDExLjIgNiAxMS43IDYgMTNjMCAuNC0uMS44LS4xIDEuMi0uMS4zLS4xLjctLjEgMSAwIC44LjMuOCAxLjQuOGguNXYxLjloLS45Yy0yLjEgMC0zLjUtLjYtMy41LTIuMyAwLS40LjEtLjkuMS0xLjMuMS0uNS4xLS45LjEtMS4zIDAtLjUtLjItMS0xLjctMXYtMS45eiIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSIxMy44IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY3g9IjExIiBjeT0iOC4yIiByPSIyLjEiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgPGcgY2xhc3M9ImpwLWljb24td2FybjAiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4=);
  --jp-icon-listings-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MC45NzggNTAuOTc4IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA1MC45NzggNTAuOTc4OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+Cgk8Zz4KCQk8cGF0aCBzdHlsZT0iZmlsbDojMDEwMDAyOyIgZD0iTTQzLjUyLDcuNDU4QzM4LjcxMSwyLjY0OCwzMi4zMDcsMCwyNS40ODksMEMxOC42NywwLDEyLjI2NiwyLjY0OCw3LjQ1OCw3LjQ1OAoJCQljLTkuOTQzLDkuOTQxLTkuOTQzLDI2LjExOSwwLDM2LjA2MmM0LjgwOSw0LjgwOSwxMS4yMTIsNy40NTYsMTguMDMxLDcuNDU4YzAsMCwwLjAwMSwwLDAuMDAyLDAKCQkJYzYuODE2LDAsMTMuMjIxLTIuNjQ4LDE4LjAyOS03LjQ1OGM0LjgwOS00LjgwOSw3LjQ1Ny0xMS4yMTIsNy40NTctMTguMDNDNTAuOTc3LDE4LjY3LDQ4LjMyOCwxMi4yNjYsNDMuNTIsNy40NTh6CgkJCSBNNDIuMTA2LDQyLjEwNWMtNC40MzIsNC40MzEtMTAuMzMyLDYuODcyLTE2LjYxNSw2Ljg3MmgtMC4wMDJjLTYuMjg1LTAuMDAxLTEyLjE4Ny0yLjQ0MS0xNi42MTctNi44NzIKCQkJYy05LjE2Mi05LjE2My05LjE2Mi0yNC4wNzEsMC0zMy4yMzNDMTMuMzAzLDQuNDQsMTkuMjA0LDIsMjUuNDg5LDJjNi4yODQsMCwxMi4xODYsMi40NCwxNi42MTcsNi44NzIKCQkJYzQuNDMxLDQuNDMxLDYuODcxLDEwLjMzMiw2Ljg3MSwxNi42MTdDNDguOTc3LDMxLjc3Miw0Ni41MzYsMzcuNjc1LDQyLjEwNiw0Mi4xMDV6Ii8+CgkJPHBhdGggc3R5bGU9ImZpbGw6IzAxMDAwMjsiIGQ9Ik0yMy41NzgsMzIuMjE4Yy0wLjAyMy0xLjczNCwwLjE0My0zLjA1OSwwLjQ5Ni0zLjk3MmMwLjM1My0wLjkxMywxLjExLTEuOTk3LDIuMjcyLTMuMjUzCgkJCWMwLjQ2OC0wLjUzNiwwLjkyMy0xLjA2MiwxLjM2Ny0xLjU3NWMwLjYyNi0wLjc1MywxLjEwNC0xLjQ3OCwxLjQzNi0yLjE3NWMwLjMzMS0wLjcwNywwLjQ5NS0xLjU0MSwwLjQ5NS0yLjUKCQkJYzAtMS4wOTYtMC4yNi0yLjA4OC0wLjc3OS0yLjk3OWMtMC41NjUtMC44NzktMS41MDEtMS4zMzYtMi44MDYtMS4zNjljLTEuODAyLDAuMDU3LTIuOTg1LDAuNjY3LTMuNTUsMS44MzIKCQkJYy0wLjMwMSwwLjUzNS0wLjUwMywxLjE0MS0wLjYwNywxLjgxNGMtMC4xMzksMC43MDctMC4yMDcsMS40MzItMC4yMDcsMi4xNzRoLTIuOTM3Yy0wLjA5MS0yLjIwOCwwLjQwNy00LjExNCwxLjQ5My01LjcxOQoJCQljMS4wNjItMS42NCwyLjg1NS0yLjQ4MSw1LjM3OC0yLjUyN2MyLjE2LDAuMDIzLDMuODc0LDAuNjA4LDUuMTQxLDEuNzU4YzEuMjc4LDEuMTYsMS45MjksMi43NjQsMS45NSw0LjgxMQoJCQljMCwxLjE0Mi0wLjEzNywyLjExMS0wLjQxLDIuOTExYy0wLjMwOSwwLjg0NS0wLjczMSwxLjU5My0xLjI2OCwyLjI0M2MtMC40OTIsMC42NS0xLjA2OCwxLjMxOC0xLjczLDIuMDAyCgkJCWMtMC42NSwwLjY5Ny0xLjMxMywxLjQ3OS0xLjk4NywyLjM0NmMtMC4yMzksMC4zNzctMC40MjksMC43NzctMC41NjUsMS4xOTljLTAuMTYsMC45NTktMC4yMTcsMS45NTEtMC4xNzEsMi45NzkKCQkJQzI2LjU4OSwzMi4yMTgsMjMuNTc4LDMyLjIxOCwyMy41NzgsMzIuMjE4eiBNMjMuNTc4LDM4LjIydi0zLjQ4NGgzLjA3NnYzLjQ4NEgyMy41Nzh6Ii8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMEQ0N0ExIj4KICAgIDxwYXRoIGQ9Ik0xMS4xIDYuOVY1LjhINi45YzAtLjUgMC0xLjMuMi0xLjYuNC0uNy44LTEuMSAxLjctMS40IDEuNy0uMyAyLjUtLjMgMy45LS4xIDEgLjEgMS45LjkgMS45IDEuOXY0LjJjMCAuNS0uOSAxLjYtMiAxLjZIOC44Yy0xLjUgMC0yLjQgMS40LTIuNCAyLjh2Mi4ySDQuN0MzLjUgMTUuMSAzIDE0IDMgMTMuMVY5Yy0uMS0xIC42LTIgMS44LTIgMS41LS4xIDYuMy0uMSA2LjMtLjF6Ii8+CiAgICA8cGF0aCBkPSJNMTAuOSAxNS4xdjEuMWg0LjJjMCAuNSAwIDEuMy0uMiAxLjYtLjQuNy0uOCAxLjEtMS43IDEuNC0xLjcuMy0yLjUuMy0zLjkuMS0xLS4xLTEuOS0uOS0xLjktMS45di00LjJjMC0uNS45LTEuNiAyLTEuNmgzLjhjMS41IDAgMi40LTEuNCAyLjQtMi44VjYuNmgxLjdDMTguNSA2LjkgMTkgOCAxOSA4LjlWMTNjMCAxLS43IDIuMS0xLjkgMi4xaC02LjJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMikiIGZpbGw9IiMzMzMzMzMiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uLWFjY2VudDIganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGQ9Ik01LjA1NjY0IDguNzYxNzJDNS4wNTY2NCA4LjU5NzY2IDUuMDMxMjUgOC40NTMxMiA0Ljk4MDQ3IDguMzI4MTJDNC45MzM1OSA4LjE5OTIyIDQuODU1NDcgOC4wODIwMyA0Ljc0NjA5IDcuOTc2NTZDNC42NDA2MiA3Ljg3MTA5IDQuNSA3Ljc3NTM5IDQuMzI0MjIgNy42ODk0NUM0LjE1MjM0IDcuNTk5NjEgMy45NDMzNiA3LjUxMTcyIDMuNjk3MjcgNy40MjU3OEMzLjMwMjczIDcuMjg1MTYgMi45NDMzNiA3LjEzNjcyIDIuNjE5MTQgNi45ODA0N0MyLjI5NDkyIDYuODI0MjIgMi4wMTc1OCA2LjY0MjU4IDEuNzg3MTEgNi40MzU1NUMxLjU2MDU1IDYuMjI4NTIgMS4zODQ3NyA1Ljk4ODI4IDEuMjU5NzcgNS43MTQ4NEMxLjEzNDc3IDUuNDM3NSAxLjA3MjI3IDUuMTA5MzggMS4wNzIyNyA0LjczMDQ3QzEuMDcyMjcgNC4zOTg0NCAxLjEyODkxIDQuMDk1NyAxLjI0MjE5IDMuODIyMjdDMS4zNTU0NyAzLjU0NDkyIDEuNTE1NjIgMy4zMDQ2OSAxLjcyMjY2IDMuMTAxNTZDMS45Mjk2OSAyLjg5ODQ0IDIuMTc5NjkgMi43MzQzNyAyLjQ3MjY2IDIuNjA5MzhDMi43NjU2MiAyLjQ4NDM4IDMuMDkxOCAyLjQwNDMgMy40NTExNyAyLjM2OTE0VjEuMTA5MzhINC4zODg2N1YyLjM4MDg2QzQuNzQwMjMgMi40Mjc3MyA1LjA1NjY0IDIuNTIzNDQgNS4zMzc4OSAyLjY2Nzk3QzUuNjE5MTQgMi44MTI1IDUuODU3NDIgMy4wMDE5NSA2LjA1MjczIDMuMjM2MzNDNi4yNTE5NSAzLjQ2NjggNi40MDQzIDMuNzQwMjMgNi41MDk3NyA0LjA1NjY0QzYuNjE5MTQgNC4zNjkxNCA2LjY3MzgzIDQuNzIwNyA2LjY3MzgzIDUuMTExMzNINS4wNDQ5MkM1LjA0NDkyIDQuNjM4NjcgNC45Mzc1IDQuMjgxMjUgNC43MjI2NiA0LjAzOTA2QzQuNTA3ODEgMy43OTI5NyA0LjIxNjggMy42Njk5MiAzLjg0OTYxIDMuNjY5OTJDMy42NTAzOSAzLjY2OTkyIDMuNDc2NTYgMy42OTcyNyAzLjMyODEyIDMuNzUxOTVDMy4xODM1OSAzLjgwMjczIDMuMDY0NDUgMy44NzY5NSAyLjk3MDcgMy45NzQ2MUMyLjg3Njk1IDQuMDY4MzYgMi44MDY2NCA0LjE3OTY5IDIuNzU5NzcgNC4zMDg1OUMyLjcxNjggNC40Mzc1IDIuNjk1MzEgNC41NzgxMiAyLjY5NTMxIDQuNzMwNDdDMi42OTUzMSA0Ljg4MjgxIDIuNzE2OCA1LjAxOTUzIDIuNzU5NzcgNS4xNDA2MkMyLjgwNjY0IDUuMjU3ODEgMi44ODI4MSA1LjM2NzE5IDIuOTg4MjggNS40Njg3NUMzLjA5NzY2IDUuNTcwMzEgMy4yNDAyMyA1LjY2Nzk3IDMuNDE2MDIgNS43NjE3MkMzLjU5MTggNS44NTE1NiAzLjgxMDU1IDUuOTQzMzYgNC4wNzIyNyA2LjAzNzExQzQuNDY2OCA2LjE4NTU1IDQuODI0MjIgNi4zMzk4NCA1LjE0NDUzIDYuNUM1LjQ2NDg0IDYuNjU2MjUgNS43MzgyOCA2LjgzOTg0IDUuOTY0ODQgNy4wNTA3OEM2LjE5NTMxIDcuMjU3ODEgNi4zNzEwOSA3LjUgNi40OTIxOSA3Ljc3NzM0QzYuNjE3MTkgOC4wNTA3OCA2LjY3OTY5IDguMzc1IDYuNjc5NjkgOC43NUM2LjY3OTY5IDkuMDkzNzUgNi42MjMwNSA5LjQwNDMgNi41MDk3NyA5LjY4MTY0QzYuMzk2NDggOS45NTUwOCA2LjIzNDM4IDEwLjE5MTQgNi4wMjM0NCAxMC4zOTA2QzUuODEyNSAxMC41ODk4IDUuNTU4NTkgMTAuNzUgNS4yNjE3MiAxMC44NzExQzQuOTY0ODQgMTAuOTg4MyA0LjYzMjgxIDExLjA2NDUgNC4yNjU2MiAxMS4wOTk2VjEyLjI0OEgzLjMzMzk4VjExLjA5OTZDMy4wMDE5NSAxMS4wNjg0IDIuNjc5NjkgMTAuOTk2MSAyLjM2NzE5IDEwLjg4MjhDMi4wNTQ2OSAxMC43NjU2IDEuNzc3MzQgMTAuNTk3NyAxLjUzNTE2IDEwLjM3ODlDMS4yOTY4OCAxMC4xNjAyIDEuMTA1NDcgOS44ODQ3NyAwLjk2MDkzOCA5LjU1MjczQzAuODE2NDA2IDkuMjE2OCAwLjc0NDE0MSA4LjgxNDQ1IDAuNzQ0MTQxIDguMzQ1N0gyLjM3ODkxQzIuMzc4OTEgOC42MjY5NSAyLjQxOTkyIDguODYzMjggMi41MDE5NSA5LjA1NDY5QzIuNTgzOTggOS4yNDIxOSAyLjY4OTQ1IDkuMzkyNTggMi44MTgzNiA5LjUwNTg2QzIuOTUxMTcgOS42MTUyMyAzLjEwMTU2IDkuNjkzMzYgMy4yNjk1MyA5Ljc0MDIzQzMuNDM3NSA5Ljc4NzExIDMuNjA5MzggOS44MTA1NSAzLjc4NTE2IDkuODEwNTVDNC4yMDMxMiA5LjgxMDU1IDQuNTE5NTMgOS43MTI4OSA0LjczNDM4IDkuNTE3NThDNC45NDkyMiA5LjMyMjI3IDUuMDU2NjQgOS4wNzAzMSA1LjA1NjY0IDguNzYxNzJaTTEzLjQxOCAxMi4yNzE1SDguMDc0MjJWMTFIMTMuNDE4VjEyLjI3MTVaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzLjk1MjY0IDYpIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTUgMTVIM3YyaDEydi0yem0wLThIM3YyaDEyVjd6TTMgMTNoMTh2LTJIM3Yyem0wIDhoMTh2LTJIM3Yyek0zIDN2MmgxOFYzSDN6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4=);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}
.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}
.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}
.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}
.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}
.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}
.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}
.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}
.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}
.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}
.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}
.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}
.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}
.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}
.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}
.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}
.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}
.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}
.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}
.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}
.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}
.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}
.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}
.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}
.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}
.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}
.jp-FileIcon {
  background-image: var(--jp-icon-file);
}
.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}
.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}
.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}
.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}
.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}
.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}
.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}
.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
}
.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}
.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}
.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}
.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}
.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}
.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}
.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}
.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}
.jp-ListIcon {
  background-image: var(--jp-icon-list);
}
.jp-ListingsInfoIcon {
  background-image: var(--jp-icon-listings-info);
}
.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}
.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}
.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}
.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}
.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}
.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}
.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}
.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}
.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
}
.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}
.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}
.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}
.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
}
.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}
.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}
.jp-RunIcon {
  background-image: var(--jp-icon-run);
}
.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}
.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}
.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}
.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}
.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}
.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}
.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}
.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}
.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}
.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}
.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}
.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}
.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}
.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}
.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}
.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}
.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}
/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}
/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}
/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}
.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}
.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}
.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}
.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}
.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}
.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}
.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}
.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}
/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}
.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}
.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}
.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}
.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}
.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}
.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}
/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

/* CSS for icons in selected items in the settings editor */
#setting-editor .jp-PluginList .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
#setting-editor
  .jp-PluginList
  .jp-mod-selected
  .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected tabs in the sidebar tab manager */
#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable[fill] {
  fill: #fff;
}

#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable[fill] {
  fill: var(--jp-brand-color1);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable-inverse[fill] {
  fill: #fff;
}

/**
 * TODO: come up with non css-hack solution for showing the busy icon on top
 *  of the close icon
 * CSS for complex behavior of close icon of tabs in the sidebar tab manager
 */
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-dirty.jp-mod-active
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: #fff;
}

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) svg {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-border-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0px;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-warn-color0);
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

/* Override Blueprint's _reset.scss styles */
html {
  box-sizing: unset;
}

*,
*::before,
*::after {
  box-sizing: unset;
}

body {
  color: unset;
  font-family: var(--jp-ui-font-family);
}

p {
  margin-top: unset;
  margin-bottom: unset;
}

small {
  font-size: unset;
}

strong {
  font-weight: unset;
}

/* Override Blueprint's _typography.scss styles */
a {
  text-decoration: unset;
  color: unset;
}
a:hover {
  text-decoration: unset;
  color: unset;
}

/* Override Blueprint's _accessibility.scss styles */
:focus {
  outline: unset;
  outline-offset: unset;
  -moz-outline-radius: unset;
}

/* Styles for ui-components */
.jp-Button {
  border-radius: var(--jp-border-radius);
  padding: 0px 12px;
  font-size: var(--jp-ui-font-size1);
}

/* Use our own theme for hover styles */
button.jp-Button.bp3-button.bp3-minimal:hover {
  background-color: var(--jp-layout-color2);
}
.jp-Button.minimal {
  color: unset !important;
}

.jp-Button.jp-ToolbarButtonComponent {
  text-transform: none;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color3);
}

.jp-BPIcon {
  display: inline-block;
  vertical-align: middle;
  margin: auto;
}

/* Stop blueprint futzing with our icon fills */
.bp3-icon.jp-BPIcon > svg:not([fill]) {
  fill: var(--jp-inverse-layout-color3);
}

.jp-InputGroupAction {
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

/* Use our own theme for hover and option styles */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}
select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-top: 1px solid var(--jp-border-color2);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-Collapse-header {
  padding: 1px 12px;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size2);
}

.jp-Collapse-header:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Collapse-contents {
  padding: 0px 12px 0px 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0px;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0px 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px 5px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0px;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty:after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0px 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0px;
  left: 0px;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px;
  padding-bottom: 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
  resize: both;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0px;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0px 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

.jp-HoverBox.jp-mod-outofview {
  display: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;

  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;

  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #aa00ff;

  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;

  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;

  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;

  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;

  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;

  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;

  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;

  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;

  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;

  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ffff00;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;

  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;

  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;

  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;

  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;

  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eeeeee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;

  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent:before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent:after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0px 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FileDialog-Checkbox {
  margin-top: 35px;
  display: flex;
  flex-direction: row;
  align-items: end;
  width: 100%;
}

.jp-FileDialog-Checkbox > label {
  flex: 1 1 auto;
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  height: 28px;
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  background-color: var(--jp-layout-color1);
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0px 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  height: 32px;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 1;
  overflow-x: auto;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px;
  margin: 0px;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px 6px;
  margin: 0px;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent span {
  padding: 0px;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ body.p-mod-override-cursor *, /* </DEPRECATED> */
body.lm-mod-override-cursor * {
  cursor: inherit !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/* BASICS */

.CodeMirror {
  /* Set height, width, borders, and global font properties here */
  font-family: monospace;
  height: 300px;
  color: black;
  direction: ltr;
}

/* PADDING */

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  background-color: white; /* The little square between H and V scrollbars */
}

/* GUTTER */

.CodeMirror-gutters {
  border-right: 1px solid #ddd;
  background-color: #f7f7f7;
  white-space: nowrap;
}
.CodeMirror-linenumbers {}
.CodeMirror-linenumber {
  padding: 0 3px 0 5px;
  min-width: 20px;
  text-align: right;
  color: #999;
  white-space: nowrap;
}

.CodeMirror-guttermarker { color: black; }
.CodeMirror-guttermarker-subtle { color: #999; }

/* CURSOR */

.CodeMirror-cursor {
  border-left: 1px solid black;
  border-right: none;
  width: 0;
}
/* Shown when moving in bi-directional text */
.CodeMirror div.CodeMirror-secondarycursor {
  border-left: 1px solid silver;
}
.cm-fat-cursor .CodeMirror-cursor {
  width: auto;
  border: 0 !important;
  background: #7e7;
}
.cm-fat-cursor div.CodeMirror-cursors {
  z-index: 1;
}
.cm-fat-cursor-mark {
  background-color: rgba(20, 255, 20, 0.5);
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
}
.cm-animate-fat-cursor {
  width: auto;
  border: 0;
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
  background-color: #7e7;
}
@-moz-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@-webkit-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}

/* Can style cursor different in overwrite (non-insert) mode */
.CodeMirror-overwrite .CodeMirror-cursor {}

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers {
  position: absolute;
  left: 0; right: 0; top: -50px; bottom: 0;
  overflow: hidden;
}
.CodeMirror-ruler {
  border-left: 1px solid #ccc;
  top: 0; bottom: 0;
  position: absolute;
}

/* DEFAULT THEME */

.cm-s-default .cm-header {color: blue;}
.cm-s-default .cm-quote {color: #090;}
.cm-negative {color: #d44;}
.cm-positive {color: #292;}
.cm-header, .cm-strong {font-weight: bold;}
.cm-em {font-style: italic;}
.cm-link {text-decoration: underline;}
.cm-strikethrough {text-decoration: line-through;}

.cm-s-default .cm-keyword {color: #708;}
.cm-s-default .cm-atom {color: #219;}
.cm-s-default .cm-number {color: #164;}
.cm-s-default .cm-def {color: #00f;}
.cm-s-default .cm-variable,
.cm-s-default .cm-punctuation,
.cm-s-default .cm-property,
.cm-s-default .cm-operator {}
.cm-s-default .cm-variable-2 {color: #05a;}
.cm-s-default .cm-variable-3, .cm-s-default .cm-type {color: #085;}
.cm-s-default .cm-comment {color: #a50;}
.cm-s-default .cm-string {color: #a11;}
.cm-s-default .cm-string-2 {color: #f50;}
.cm-s-default .cm-meta {color: #555;}
.cm-s-default .cm-qualifier {color: #555;}
.cm-s-default .cm-builtin {color: #30a;}
.cm-s-default .cm-bracket {color: #997;}
.cm-s-default .cm-tag {color: #170;}
.cm-s-default .cm-attribute {color: #00c;}
.cm-s-default .cm-hr {color: #999;}
.cm-s-default .cm-link {color: #00c;}

.cm-s-default .cm-error {color: #f00;}
.cm-invalidchar {color: #f00;}

.CodeMirror-composing { border-bottom: 2px solid; }

/* Default styles for common addons */

div.CodeMirror span.CodeMirror-matchingbracket {color: #0b0;}
div.CodeMirror span.CodeMirror-nonmatchingbracket {color: #a22;}
.CodeMirror-matchingtag { background: rgba(255, 150, 0, .3); }
.CodeMirror-activeline-background {background: #e8f2ff;}

/* STOP */

/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: white;
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 50px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -50px; margin-right: -50px;
  padding-bottom: 50px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}
.CodeMirror-sizer {
  position: relative;
  border-right: 50px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
  outline: none;
}
.CodeMirror-vscrollbar {
  right: 0; top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}
.CodeMirror-hscrollbar {
  bottom: 0; left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}
.CodeMirror-scrollbar-filler {
  right: 0; bottom: 0;
}
.CodeMirror-gutter-filler {
  left: 0; bottom: 0;
}

.CodeMirror-gutters {
  position: absolute; left: 0; top: 0;
  min-height: 100%;
  z-index: 3;
}
.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -50px;
}
.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}
.CodeMirror-gutter-background {
  position: absolute;
  top: 0; bottom: 0;
  z-index: 4;
}
.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}
.CodeMirror-gutter-wrapper ::selection { background-color: transparent }
.CodeMirror-gutter-wrapper ::-moz-selection { background-color: transparent }

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  -moz-border-radius: 0; -webkit-border-radius: 0; border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}
.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-widget {}

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}
.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}
div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected { background: #d9d9d9; }
.CodeMirror-focused .CodeMirror-selected { background: #d7d4f0; }
.CodeMirror-crosshair { cursor: crosshair; }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: #d7d4f0; }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: #d7d4f0; }

.cm-searching {
  background-color: #ffa;
  background-color: rgba(255, 255, 0, .4);
}

/* Used to force a border model for a node */
.cm-force-border { padding-right: .1px; }

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack:after { content: ''; }

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext { background: none; }

.CodeMirror-dialog {
  position: absolute;
  left: 0; right: 0;
  background: inherit;
  z-index: 15;
  padding: .1em .8em;
  overflow: hidden;
  color: inherit;
}

.CodeMirror-dialog-top {
  border-bottom: 1px solid #eee;
  top: 0;
}

.CodeMirror-dialog-bottom {
  border-top: 1px solid #eee;
  bottom: 0;
}

.CodeMirror-dialog input {
  border: none;
  outline: none;
  background: transparent;
  width: 20em;
  color: inherit;
  font-family: monospace;
}

.CodeMirror-dialog button {
  font-size: 70%;
}

.CodeMirror-foldmarker {
  color: blue;
  text-shadow: #b9f 1px 1px 2px, #b9f -1px -1px 2px, #b9f 1px -1px 2px, #b9f -1px 1px 2px;
  font-family: arial;
  line-height: .3;
  cursor: pointer;
}
.CodeMirror-foldgutter {
  width: .7em;
}
.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
}
.CodeMirror-foldgutter-open:after {
  content: "\25BE";
}
.CodeMirror-foldgutter-folded:after {
  content: "\25B8";
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.CodeMirror {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;
  /* Changed to auto to autogrow */
}

.CodeMirror pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* This causes https://github.com/jupyter/jupyterlab/issues/522 */
/* May not cause it not because we changed it! */
.CodeMirror-lines {
  padding: var(--jp-code-padding) 0;
}

.CodeMirror-linenumber {
  padding: 0 8px;
}

.jp-CodeMirrorEditor {
  cursor: text;
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.CodeMirror.jp-mod-readOnly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--jp-border-color2);
  background-color: var(--jp-layout-color0);
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.CodeMirror-selectedtext.cm-searching {
  background-color: var(--jp-search-selected-match-background-color) !important;
  color: var(--jp-search-selected-match-color) !important;
}

.cm-searching {
  background-color: var(
    --jp-search-unselected-match-background-color
  ) !important;
  color: var(--jp-search-unselected-match-color) !important;
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--jp-editor-selected-focused-background);
}

.CodeMirror-selected {
  background-color: var(--jp-editor-selected-background);
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/**
 * Here is our jupyter theme for CodeMirror syntax highlighting
 * This is used in our marked.js syntax highlighting and CodeMirror itself
 * The string "jupyter" is set in ../codemirror/widget.DEFAULT_CODEMIRROR_THEME
 * This came from the classic notebook, which came form highlight.js/GitHub
 */

/**
 * CodeMirror themes are handling the background/color in this way. This works
 * fine for CodeMirror editors outside the notebook, but the notebook styles
 * these things differently.
 */
.CodeMirror.cm-s-jupyter {
  background: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* In the notebook, we want this styling to be handled by its container */
.jp-CodeConsole .CodeMirror.cm-s-jupyter,
.jp-Notebook .CodeMirror.cm-s-jupyter {
  background: transparent;
}

.cm-s-jupyter .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}
.cm-s-jupyter span.cm-keyword {
  color: var(--jp-mirror-editor-keyword-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-atom {
  color: var(--jp-mirror-editor-atom-color);
}
.cm-s-jupyter span.cm-number {
  color: var(--jp-mirror-editor-number-color);
}
.cm-s-jupyter span.cm-def {
  color: var(--jp-mirror-editor-def-color);
}
.cm-s-jupyter span.cm-variable {
  color: var(--jp-mirror-editor-variable-color);
}
.cm-s-jupyter span.cm-variable-2 {
  color: var(--jp-mirror-editor-variable-2-color);
}
.cm-s-jupyter span.cm-variable-3 {
  color: var(--jp-mirror-editor-variable-3-color);
}
.cm-s-jupyter span.cm-punctuation {
  color: var(--jp-mirror-editor-punctuation-color);
}
.cm-s-jupyter span.cm-property {
  color: var(--jp-mirror-editor-property-color);
}
.cm-s-jupyter span.cm-operator {
  color: var(--jp-mirror-editor-operator-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-comment {
  color: var(--jp-mirror-editor-comment-color);
  font-style: italic;
}
.cm-s-jupyter span.cm-string {
  color: var(--jp-mirror-editor-string-color);
}
.cm-s-jupyter span.cm-string-2 {
  color: var(--jp-mirror-editor-string-2-color);
}
.cm-s-jupyter span.cm-meta {
  color: var(--jp-mirror-editor-meta-color);
}
.cm-s-jupyter span.cm-qualifier {
  color: var(--jp-mirror-editor-qualifier-color);
}
.cm-s-jupyter span.cm-builtin {
  color: var(--jp-mirror-editor-builtin-color);
}
.cm-s-jupyter span.cm-bracket {
  color: var(--jp-mirror-editor-bracket-color);
}
.cm-s-jupyter span.cm-tag {
  color: var(--jp-mirror-editor-tag-color);
}
.cm-s-jupyter span.cm-attribute {
  color: var(--jp-mirror-editor-attribute-color);
}
.cm-s-jupyter span.cm-header {
  color: var(--jp-mirror-editor-header-color);
}
.cm-s-jupyter span.cm-quote {
  color: var(--jp-mirror-editor-quote-color);
}
.cm-s-jupyter span.cm-link {
  color: var(--jp-mirror-editor-link-color);
}
.cm-s-jupyter span.cm-error {
  color: var(--jp-mirror-editor-error-color);
}
.cm-s-jupyter span.cm-hr {
  color: #999;
}

.cm-s-jupyter span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}

.cm-s-jupyter .CodeMirror-activeline-background,
.cm-s-jupyter .CodeMirror-gutter {
  background-color: var(--jp-layout-color2);
}

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .remote-caret {
  position: relative;
  border-left: 2px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .remote-caret > div {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -2px;
  font-size: 0.95em;
  background-color: rgb(250, 129, 0);
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 3;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .remote-caret.hide-name > div {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .remote-caret:hover > div {
  opacity: 1;
  transition-delay: 0s;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0px;
  padding: 0px;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}
.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}
.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}
.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}
.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}
.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}
.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}
.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}
.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}
.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}
.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}
.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}
.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}
.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}
.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}
.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}
.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0em;
}

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: 12px;
  table-layout: fixed;
  margin-left: auto;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon table {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0px;
}

.jp-RenderedHTMLCommon p {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}
/* ...or leave it untouched if they don't */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-dark-background {
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-light-background {
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}
.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}
.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}
.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}
.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}
.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}
.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}
.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}
.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: 0.8em;
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser {
  display: flex;
  flex-direction: column;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  border-bottom: none;
  height: auto;
  margin: var(--jp-toolbar-header-margin);
  box-shadow: none;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0px 2px;
  padding: 0px 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0px;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar.jp-Toolbar {
  padding: 0px;
  margin: 8px 12px 0px 12px;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  justify-content: flex-start;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0px;
  padding-right: 2px;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-ToolbarButtonComponent {
  width: 40px;
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent {
  width: 72px;
  background: var(--jp-brand-color1);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent:focus-visible {
  background-color: var(--jp-brand-color0);
}

.jp-FileBrowser-toolbar.jp-Toolbar
  .jp-Toolbar-item:first-child
  .jp-ToolbarButtonComponent
  .jp-icon3 {
  fill: white;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileBrowser-filterBox {
  padding: 0px;
  flex: 0 0 auto;
  margin: 8px 12px 0px 12px;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing:focus-visible {
  border: 1px solid var(--jp-brand-color1);
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px 12px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon:before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon:before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0px;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-DirListing-deadSpace {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
}

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: flex;
  flex-direction: row;
}

body[data-format='mobile'] .jp-OutputArea-child {
  flex-direction: column;
}

.jp-OutputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

body[data-format='mobile'] .jp-OutputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

.jp-OutputArea-output {
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea-child .jp-OutputArea-output {
  flex-grow: 1;
  flex-shrink: 1;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  margin-left: var(--jp-notebook-padding);
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0px;
  padding: 0px;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0px;
  flex: 1 1 auto;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-OutputArea-stdin {
  line-height: var(--jp-code-line-height);
  padding-top: var(--jp-code-padding);
  display: flex;
}

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;
  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0px;
  bottom: 0px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0px;
  width: 100%;
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: flex;
  flex-direction: row;
  overflow: hidden;
}

body[data-format='mobile'] .jp-InputArea {
  flex-direction: column;
}

.jp-InputArea-editor {
  flex: 1 1 auto;
  overflow: hidden;
}

.jp-InputArea-editor {
  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0px;
  background: var(--jp-cell-editor-background);
}

body[data-format='mobile'] .jp-InputArea-editor {
  margin-left: var(--jp-notebook-padding);
}

.jp-InputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

body[data-format='mobile'] .jp-InputPrompt {
  flex: 0 0 auto;
  text-align: left;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: flex;
  flex-direction: row;
  flex: 1 1 auto;
}

.jp-Placeholder-prompt {
  box-sizing: border-box;
}

.jp-Placeholder-content {
  flex: 1 1 auto;
  border: none;
  background: transparent;
  height: 20px;
  box-sizing: border-box;
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0px;
  margin: 0px;
  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 200px;
  box-shadow: inset 0 0 6px 2px rgba(0, 0, 0, 0.3);
  margin-left: var(--jp-private-cell-scrolling-output-offset);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  flex: 0 0
    calc(
      var(--jp-cell-prompt-width) -
        var(--jp-private-cell-scrolling-output-offset)
    );
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  flex: 1 1 auto;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

.jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
}

.jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-collapseHeadingButton {
  display: none;
}

.jp-MarkdownCell:hover .jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  position: absolute;
  right: 0;
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: 2px;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
}

.jp-Notebook-render * {
  contain: none !important;
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
  float: left;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt:before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0px;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-NotebookTools-tool {
  padding: 0px 12px 0 12px;
}

.jp-ActiveCellTool {
  padding: 12px;
  background-color: var(--jp-layout-color1);
  border-top: none !important;
}

.jp-ActiveCellTool .jp-InputArea-prompt {
  flex: 0 0 auto;
  padding-left: 0px;
}

.jp-ActiveCellTool .jp-InputArea-editor {
  flex: 1 1 auto;
  background: var(--jp-cell-editor-background);
  border-color: var(--jp-cell-editor-border-color);
}

.jp-ActiveCellTool .jp-InputArea-editor .CodeMirror {
  background: transparent;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0px 12px 0px;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body div {
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

</style>

    <style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
    0px 1px 3px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
    0px 1px 5px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
    0px 1px 10px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
    0px 1px 18px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
    0px 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
    0px 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
    0px 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
    0px 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
    0px 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;

  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;

  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);

  --jp-content-link-color: var(--md-blue-700);

  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);

  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);

  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);

  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);

  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;

  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;

  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);

  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0px;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;
  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0px 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-border-color1);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: #05a;
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #aa22ff;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #aa22ff;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);
}
</style>

<style type="text/css">
/* Force rendering true colors when outputing to pdf */
* {
  -webkit-print-color-adjust: exact;
}

/* Misc */
a.anchor-link {
  display: none;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.CodeMirror.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.CodeMirror-line */
  padding: var(--jp-code-padding) 4px;
  margin: 0;

  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;

}

.jp-OutputArea-output pre {
  line-height: inherit;
  font-family: inherit;
}

.jp-RenderedText pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
}

/* Using table instead of flexbox so that we can use break-inside property */
/* CSS rules under this comment should not be required anymore after we move to the JupyterLab 4.0 CSS */


.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  min-width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-OutputArea-child {
  display: table;
  width: 100%;
}

.jp-OutputPrompt {
  display: table-cell;
  vertical-align: top;
  min-width: var(--jp-cell-prompt-width);
}

body[data-format='mobile'] .jp-OutputPrompt {
  display: table-row;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
  display: table-row;
}

.jp-OutputArea-output.jp-OutputArea-executeResult {
  width: 100%;
}

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }

  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}
</style>

<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: {
                    automatic: true
                    }
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
    <!-- End of mathjax configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">

<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p><a href="https://www.nvidia.com/dli"> <img src="images/combined_logo.png" alt="Header" style="width: 400px;"/> </a></p>

</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h2 id="Assessment:-Disaster-Risk-Monitoring-Using-Satellite-Imagery">Assessment: Disaster Risk Monitoring Using Satellite Imagery<a class="anchor-link" href="#Assessment:-Disaster-Risk-Monitoring-Using-Satellite-Imagery">&#182;</a></h2><p>In this notebook, you will utilize what you've learned in this course to complete an assessment. The assessment has been divided into a couple of steps to guide your development. You will be graded based on the performance of your model evaluation. Note that this coding portion does not give partial credit - it shows up as either 0 or 60 points.</p>
<table border="1" class="dataframe" align='left'>  <thead>    <tr style="text-align: right;">      <th>Step</th>      <th></th>      <th>Points</th>    </tr>  </thead>  <tbody>    <tr>      <td>0. The Problem</td>      <td></td>      <td></td>    </tr>    <tr>      <td>1. Set Up Triton Inference Server</td>      <td></td>      <td></td>    </tr>    <tr>      <td>2. Send Inference Request to Server</td>      <td></td>      <td></td>    </tr>    <tr>      <td>3. Model Performance Evaluation</td>      <td></td>      <td>60</td>    </tr>    <tr>      <td>(BONUS) Performance Analysis</td>      <td></td>      <td></td>    </tr></tbody></table>

</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Step-0:-The-Problem">Step 0: The Problem<a class="anchor-link" href="#Step-0:-The-Problem">&#182;</a></h3><p>In this course, we used the TAO Toolkit to simplify the development of a segmentation model for flood detection. We were able to easily deploy the segmentation model using the Triton Inference Server. Once deployed, the model needs to be maintained and model performance needs to be monitored over time. In the case where <a href="https://en.wikipedia.org/wiki/Drift_(data_science)">drift</a> occurs due to changes in the environment, the model starts to have a decay in its predictive power and needs to be re-trained. Below is a depiction of the process.</p>
<p><img src='images/monitoring.png' width=720></p>
<p>For the assessment we are asking you to generate evaluation metrics for a sample segmentation model, which has been converted to a TensorRT engine (<code>/dli/task/tao_project/unet/export/sample_resnet18.engine</code>), on the <a href="https://github.com/cloudtostreet/Sen1Floods11">Cloud to Street dataset</a>. The ability to analyze model performance is critical to a machine learning solution. Your task is to produce inference on the input images and calculate precision, recall, and IoU (intersection over union).</p>
<p><strong>Instructions</strong>: <br> 
0.1 Execute the below cell to unzip and load data <br>
0.2 Execute the cell below to set environment variables</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 0.1</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># unzip data file</span>
<span class="o">!</span>unzip data/flood_data.zip -d flood_data
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>Archive:  data/flood_data.zip
  inflating: flood_data/Sen1Floods11_Metadata.geojson  
   creating: flood_data/catalog/
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_953791/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_953791/Ghana_953791.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_210595/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_210595/Pakistan_210595.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_198411/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_198411/USA_198411.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_740461/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_740461/Pakistan_740461.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_401863/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_401863/Pakistan_401863.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_956740/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_956740/Sri-Lanka_956740.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_430764/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_430764/USA_430764.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7856615/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7856615/Spain_7856615.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_11745/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_11745/Ghana_11745.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_406026/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_406026/Ghana_406026.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_804466/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_804466/India_804466.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1029191/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1029191/Paraguay_1029191.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_177319/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_177319/India_177319.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_178753/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_178753/Sri-Lanka_178753.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_120804/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_120804/Sri-Lanka_120804.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_147015/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_147015/Ghana_147015.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_153941/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_153941/Paraguay_153941.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_249079/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_249079/Sri-Lanka_249079.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_265762/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_265762/India_265762.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_579082/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_579082/Sri-Lanka_579082.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1033830/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1033830/Ghana_1033830.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_264787/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_264787/Ghana_264787.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_314919/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_314919/Bolivia_314919.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7370579/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7370579/Spain_7370579.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_833266/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_833266/India_833266.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_989230/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_989230/Paraguay_989230.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1078550/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1078550/Ghana_1078550.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_528249/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_528249/Pakistan_528249.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1089161/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_1089161/Ghana_1089161.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_217598/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_217598/USA_217598.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_707886/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_707886/India_707886.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_866994/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_866994/Ghana_866994.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_921838/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_921838/Paraguay_921838.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_908474/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_908474/USA_908474.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_7496/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_7496/Ghana_7496.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_251323/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_251323/USA_251323.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_83483/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_83483/Ghana_83483.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_31559/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_31559/Sri-Lanka_31559.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_135434/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_135434/India_135434.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_67102/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_67102/USA_67102.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_764946/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_764946/India_764946.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_128663/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_128663/Ghana_128663.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_649376/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_649376/Somalia_649376.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_234935/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_234935/Ghana_234935.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_652955/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_652955/USA_652955.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_60373/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_60373/Bolivia_60373.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_308249/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_308249/Ghana_308249.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_604222/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_604222/USA_604222.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_194723/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_194723/Ghana_194723.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_36015/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_36015/Paraguay_36015.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_132143/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_132143/Pakistan_132143.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_233609/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_233609/Sri-Lanka_233609.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_495107/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_495107/Ghana_495107.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_56450/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_56450/India_56450.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_624341/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_624341/India_624341.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_324254/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_324254/India_324254.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7604243/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7604243/Spain_7604243.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_337094/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_337094/Spain_337094.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_952958/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_952958/Nigeria_952958.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1056717/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1056717/Paraguay_1056717.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_260929/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_260929/USA_260929.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6860600/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6860600/Spain_6860600.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_956930/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_956930/India_956930.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_600295/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_600295/Nigeria_600295.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_605682/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_605682/Paraguay_605682.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1019808/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1019808/Paraguay_1019808.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_78061/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_78061/Nigeria_78061.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_124834/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_124834/Ghana_124834.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_482517/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_482517/Paraguay_482517.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_80102/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_80102/Paraguay_80102.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_293769/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_293769/Mekong_293769.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_25540/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_25540/India_25540.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_333434/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_333434/Mekong_333434.json  
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/collection.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5650136/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5650136/Spain_5650136.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_943439/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_943439/India_943439.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_741178/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_741178/USA_741178.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_294583/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_294583/Bolivia_294583.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_366607/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_366607/USA_366607.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_79637/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_79637/India_79637.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_118868/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_118868/India_118868.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_790830/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_790830/Paraguay_790830.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_527077/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_527077/USA_527077.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_143329/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_143329/Nigeria_143329.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_132922/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_132922/Sri-Lanka_132922.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_167233/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_167233/Ghana_167233.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_172476/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_172476/Paraguay_172476.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_649970/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_649970/Sri-Lanka_649970.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_788696/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_788696/USA_788696.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_63307/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_63307/Sri-Lanka_63307.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_778194/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_778194/USA_778194.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_387945/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_387945/USA_387945.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_170264/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_170264/USA_170264.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_280900/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_280900/Paraguay_280900.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_822142/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_822142/Paraguay_822142.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_1038087/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_1038087/Sri-Lanka_1038087.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_236628/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_236628/Sri-Lanka_236628.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_382276/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_382276/Mekong_382276.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5923267/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5923267/Spain_5923267.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_399883/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_399883/India_399883.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_73419/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_73419/India_73419.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_693819/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_693819/USA_693819.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_225131/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_225131/Nigeria_225131.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_989553/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_989553/Somalia_989553.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_758178/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_758178/USA_758178.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1439641/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1439641/Mekong_1439641.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_191503/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_191503/Paraguay_191503.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_66026/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_66026/USA_66026.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_103757/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_103757/Bolivia_103757.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_49890/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_49890/Ghana_49890.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_76868/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_76868/Paraguay_76868.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_252217/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_252217/Paraguay_252217.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_59460/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_59460/India_59460.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_34417/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_34417/Paraguay_34417.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_205466/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_205466/Somalia_205466.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_246510/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_246510/Pakistan_246510.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7558720/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7558720/Spain_7558720.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_523539/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_523539/Sri-Lanka_523539.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_224165/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_224165/USA_224165.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_144050/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_144050/Ghana_144050.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1068117/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1068117/India_1068117.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_694942/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_694942/Pakistan_694942.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_3285448/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_3285448/Spain_3285448.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_97059/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_97059/Ghana_97059.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_44475/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_44475/India_44475.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_612594/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_612594/Sri-Lanka_612594.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_450918/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_450918/Sri-Lanka_450918.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_275372/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_275372/USA_275372.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_377277/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_377277/Sri-Lanka_377277.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_651904/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_651904/Paraguay_651904.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_149830/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_149830/Paraguay_149830.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_432776/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_432776/Bolivia_432776.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_205585/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_205585/Paraguay_205585.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_225187/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_225187/Paraguay_225187.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_605492/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_605492/USA_605492.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_391908/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_391908/India_391908.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_1087508/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_1087508/Somalia_1087508.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_11869/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_11869/Paraguay_11869.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_900498/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_900498/India_900498.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_970508/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_970508/Somalia_970508.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_336228/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_336228/Pakistan_336228.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_273873/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_273873/India_273873.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_22088/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_22088/Nigeria_22088.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_65724/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_65724/Pakistan_65724.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_148318/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_148318/Paraguay_148318.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_59731/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_59731/Paraguay_59731.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_895194/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_895194/Ghana_895194.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_847275/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_847275/Sri-Lanka_847275.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_826217/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_826217/USA_826217.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1111068/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1111068/Mekong_1111068.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_439488/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_439488/Nigeria_439488.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_592446/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_592446/India_592446.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_224845/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_224845/Paraguay_224845.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_11422/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_11422/USA_11422.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2938657/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2938657/Spain_2938657.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_806273/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_806273/USA_806273.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8199661/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8199661/Spain_8199661.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1068362/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1068362/USA_1068362.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_179238/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_179238/India_179238.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_812045/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_812045/Nigeria_812045.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_760290/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_760290/Pakistan_760290.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_45911/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_45911/Ghana_45911.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_887131/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_887131/Ghana_887131.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_350244/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_350244/USA_350244.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_319168/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_319168/Ghana_319168.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_1049830/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_1049830/Sri-Lanka_1049830.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1018327/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1018327/India_1018327.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_92824/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_92824/Sri-Lanka_92824.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_922192/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_922192/Sri-Lanka_922192.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_922373/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_922373/Mekong_922373.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_470303/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_470303/Paraguay_470303.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_795075/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_795075/Paraguay_795075.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_244057/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_244057/India_244057.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_97516/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_97516/Ghana_97516.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1010394/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1010394/USA_1010394.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_886726/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_886726/Somalia_886726.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1039203/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1039203/USA_1039203.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_529525/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_529525/Nigeria_529525.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_126224/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_126224/Paraguay_126224.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_179917/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_179917/USA_179917.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_284928/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_284928/Paraguay_284928.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_747992/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_747992/India_747992.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_187318/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_187318/Ghana_187318.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_909806/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_909806/Pakistan_909806.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_181503/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_181503/USA_181503.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_1068756/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_1068756/Somalia_1068756.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8154154/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8154154/Spain_8154154.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_81933/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_81933/Nigeria_81933.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_14484/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_14484/Sri-Lanka_14484.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_26376/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_26376/Ghana_26376.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_657443/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_657443/Paraguay_657443.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7387658/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7387658/Spain_7387658.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_769408/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_769408/India_769408.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_246718/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_246718/Pakistan_246718.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_295782/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_295782/Somalia_295782.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_366265/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_366265/Pakistan_366265.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_362274/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_362274/Ghana_362274.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_211406/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_211406/USA_211406.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_648632/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_648632/Paraguay_648632.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_93023/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_93023/Somalia_93023.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_747970/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_747970/India_747970.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_101973/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_101973/Sri-Lanka_101973.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_685158/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_685158/Somalia_685158.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_596495/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_596495/Mekong_596495.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_179624/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_179624/Paraguay_179624.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1191208/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1191208/Mekong_1191208.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_712873/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_712873/Pakistan_712873.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_354981/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_354981/USA_354981.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_230192/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_230192/Somalia_230192.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_716716/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_716716/Spain_716716.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_322855/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_322855/Somalia_322855.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_141271/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_141271/Ghana_141271.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_141910/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_141910/Ghana_141910.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_161233/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_161233/Ghana_161233.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_933610/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_933610/USA_933610.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_132163/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_132163/Ghana_132163.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_305760/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_305760/Paraguay_305760.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2472849/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2472849/Spain_2472849.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_591317/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_591317/India_591317.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_741073/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_741073/USA_741073.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_313799/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_313799/Ghana_313799.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_136196/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_136196/India_136196.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_277/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_277/Ghana_277.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_486103/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_486103/USA_486103.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_52610/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_52610/Mekong_52610.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_438959/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_438959/USA_438959.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1072277/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1072277/India_1072277.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_979278/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_979278/India_979278.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_70625/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_70625/Pakistan_70625.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_55568/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_55568/Sri-Lanka_55568.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_997480/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_997480/Paraguay_997480.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_215904/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_215904/Paraguay_215904.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_519181/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_519181/USA_519181.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_770353/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_770353/USA_770353.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_31096/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_31096/Nigeria_31096.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_35915/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_35915/Pakistan_35915.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_638521/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_638521/USA_638521.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_80221/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_80221/India_80221.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_664261/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_664261/USA_664261.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_1167260/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_1167260/Spain_1167260.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_916628/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_916628/Sri-Lanka_916628.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_166709/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_166709/India_166709.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_91379/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_91379/India_91379.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1248200/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1248200/Mekong_1248200.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1149855/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1149855/Mekong_1149855.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_53713/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_53713/Ghana_53713.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1082482/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1082482/USA_1082482.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_44682/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_44682/Paraguay_44682.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_474783/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_474783/Mekong_474783.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_321316/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_321316/Sri-Lanka_321316.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_896458/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_896458/Paraguay_896458.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5678382/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5678382/Spain_5678382.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_287642/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_287642/India_287642.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_269835/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_269835/Mekong_269835.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_114964/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_114964/USA_114964.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_168875/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_168875/Ghana_168875.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8372658/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8372658/Spain_8372658.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_849649/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_849649/Sri-Lanka_849649.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6199994/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6199994/Spain_6199994.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_7931/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_7931/Somalia_7931.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_348639/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_348639/USA_348639.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2594119/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2594119/Spain_2594119.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1049586/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_1049586/USA_1049586.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_62897/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_62897/Paraguay_62897.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_846007/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_846007/Mekong_846007.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_383430/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_383430/India_383430.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_24858/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_24858/Ghana_24858.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_54421/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_54421/Paraguay_54421.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_667363/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_667363/Pakistan_667363.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_664410/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_664410/India_664410.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_271769/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_271769/Paraguay_271769.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_242570/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_242570/Bolivia_242570.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_32375/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_32375/Somalia_32375.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_403081/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_403081/Paraguay_403081.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_45934/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_45934/Mekong_45934.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1018317/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1018317/India_1018317.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_992457/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_992457/Somalia_992457.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_308150/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_308150/USA_308150.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_698338/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_698338/India_698338.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_180633/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_180633/India_180633.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_721886/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_721886/Paraguay_721886.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_195014/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_195014/Somalia_195014.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_167787/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_167787/Somalia_167787.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_707067/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_707067/Nigeria_707067.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1050276/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1050276/India_1050276.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_225017/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_225017/USA_225017.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_48673/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_48673/Paraguay_48673.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_773682/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_773682/India_773682.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_94102/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_94102/Somalia_94102.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_167553/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_167553/Pakistan_167553.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7786924/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_7786924/Spain_7786924.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_115033/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_115033/USA_115033.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_9684/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_9684/Pakistan_9684.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_61925/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_61925/Ghana_61925.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_98310/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_98310/Mekong_98310.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_699062/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_699062/Somalia_699062.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_591549/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_591549/India_591549.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_981708/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_981708/India_981708.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_231124/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_231124/USA_231124.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_285297/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_285297/India_285297.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_163406/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_163406/Sri-Lanka_163406.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_670826/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_670826/USA_670826.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_977338/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_977338/Mekong_977338.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_347609/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_347609/USA_347609.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_597288/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_597288/Ghana_597288.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_94095/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_94095/Pakistan_94095.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_1095404/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_1095404/Nigeria_1095404.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_70352/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_70352/India_70352.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_868895/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_868895/Paraguay_868895.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_548910/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_548910/Pakistan_548910.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_135713/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_135713/Sri-Lanka_135713.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_952728/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_952728/India_952728.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_7894/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_7894/Paraguay_7894.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_842775/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_842775/India_842775.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_595451/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_595451/USA_595451.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_232060/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_232060/USA_232060.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_254910/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_254910/Mekong_254910.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_551926/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_551926/Sri-Lanka_551926.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_713926/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_713926/Sri-Lanka_713926.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_156478/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_156478/Ghana_156478.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_207862/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_207862/India_207862.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_36146/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_36146/Paraguay_36146.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1076204/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1076204/Paraguay_1076204.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_12849/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_12849/Somalia_12849.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_312675/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_312675/Bolivia_312675.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_360519/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_360519/Bolivia_360519.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_691027/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_691027/India_691027.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1396181/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1396181/Mekong_1396181.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_373039/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_373039/India_373039.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1282475/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1282475/Mekong_1282475.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_474121/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_474121/Pakistan_474121.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_581976/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_581976/Paraguay_581976.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_103272/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_103272/Ghana_103272.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_4282030/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_4282030/Spain_4282030.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_86502/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_86502/USA_86502.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_424793/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_424793/Mekong_424793.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_247288/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_247288/Ghana_247288.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_655230/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_655230/USA_655230.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_845821/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_845821/Sri-Lanka_845821.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_119477/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_119477/Mekong_119477.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_626316/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_626316/Somalia_626316.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_221789/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_221789/Mekong_221789.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_61368/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_61368/Somalia_61368.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_774689/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_774689/India_774689.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_233925/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_233925/Bolivia_233925.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_149787/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_149787/Paraguay_149787.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_772630/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_772630/India_772630.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_181263/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_181263/USA_181263.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_831672/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_831672/USA_831672.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_195474/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_195474/Bolivia_195474.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_1036366/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_1036366/Pakistan_1036366.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_748447/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_748447/Sri-Lanka_748447.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_511199/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_511199/Paraguay_511199.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_256539/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_256539/Somalia_256539.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_905409/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_905409/USA_905409.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_379434/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_379434/Bolivia_379434.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_5079/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_5079/Ghana_5079.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_213094/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_213094/Mekong_213094.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_828067/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_828067/India_828067.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_375183/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_375183/USA_375183.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2523247/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_2523247/Spain_2523247.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_84195/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_84195/USA_84195.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_134751/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_134751/Ghana_134751.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_774566/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_774566/Mekong_774566.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1017769/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_1017769/India_1017769.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1395593/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1395593/Mekong_1395593.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_212687/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_212687/Paraguay_212687.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_955053/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_955053/USA_955053.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_400518/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_400518/Sri-Lanka_400518.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_58086/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_58086/USA_58086.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_653336/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_653336/Sri-Lanka_653336.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_232281/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_232281/Paraguay_232281.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_85652/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_85652/Sri-Lanka_85652.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_792268/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_792268/Paraguay_792268.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_892933/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_892933/Paraguay_892933.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_566697/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_566697/India_566697.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_533192/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_533192/India_533192.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_135389/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_135389/Ghana_135389.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_869358/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_869358/India_869358.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_154838/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_154838/Ghana_154838.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8104659/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8104659/Spain_8104659.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_598959/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_598959/Nigeria_598959.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_761032/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_761032/USA_761032.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_1199913/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_1199913/Spain_1199913.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1443339/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1443339/Mekong_1443339.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_129334/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_129334/Bolivia_129334.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1029042/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_1029042/Paraguay_1029042.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_83200/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_83200/Ghana_83200.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_683296/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_683296/Paraguay_683296.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_12870/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_12870/Paraguay_12870.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_164336/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_164336/India_164336.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_534068/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_534068/Sri-Lanka_534068.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_534470/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_534470/India_534470.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_1027214/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_1027214/Pakistan_1027214.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_290290/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_290290/Bolivia_290290.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_117737/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_117737/Sri-Lanka_117737.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_19225/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_19225/USA_19225.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_66511/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_66511/USA_66511.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_166342/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_166342/Somalia_166342.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_4915752/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_4915752/Spain_4915752.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_142312/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_142312/Ghana_142312.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_76104/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_76104/Bolivia_76104.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_417184/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_417184/Nigeria_417184.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_43105/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_43105/Pakistan_43105.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_60129/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_60129/Somalia_60129.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_24341/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_24341/Paraguay_24341.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_371421/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Somalia_371421/Somalia_371421.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_500266/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_500266/India_500266.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_247656/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_247656/Paraguay_247656.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_504150/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_504150/USA_504150.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8565131/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_8565131/Spain_8565131.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_152185/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_152185/Sri-Lanka_152185.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_820924/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_820924/Nigeria_820924.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_103447/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_103447/India_103447.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_994009/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_994009/USA_994009.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6095801/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6095801/Spain_6095801.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_913449/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_913449/Paraguay_913449.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_791364/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_791364/Paraguay_791364.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_339807/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_339807/Paraguay_339807.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_35845/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_35845/Nigeria_35845.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_198534/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_198534/Paraguay_198534.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_8090/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_8090/Ghana_8090.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_146222/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_146222/Ghana_146222.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_570384/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_570384/India_570384.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_236030/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_236030/Sri-Lanka_236030.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_868803/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_868803/Ghana_868803.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_359826/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Ghana_359826/Ghana_359826.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_849790/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_849790/Pakistan_849790.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_664885/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_664885/Pakistan_664885.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_23014/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Bolivia_23014/Bolivia_23014.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_40936/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_40936/Paraguay_40936.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_631692/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_631692/India_631692.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_646878/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_646878/USA_646878.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_211386/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Pakistan_211386/Pakistan_211386.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_934240/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_934240/Paraguay_934240.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6537196/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_6537196/Spain_6537196.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_984831/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Nigeria_984831/Nigeria_984831.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_883641/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_883641/Sri-Lanka_883641.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1413877/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_1413877/Mekong_1413877.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_246154/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Paraguay_246154/Paraguay_246154.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/India_652725/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/India_652725/India_652725.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_16233/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_16233/Mekong_16233.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_52223/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_52223/Sri-Lanka_52223.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_986268/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/USA_986268/USA_986268.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_49764/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Sri-Lanka_49764/Sri-Lanka_49764.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_342411/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Mekong_342411/Mekong_342411.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5816638/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_source/Spain_5816638/Spain_5816638.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_321316_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_321316_label/Sri-Lanka_321316_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_896458_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_896458_label/Paraguay_896458_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1082482_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1082482_label/USA_1082482_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_44682_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_44682_label/Paraguay_44682_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_474783_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_474783_label/Mekong_474783_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_166709_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_166709_label/India_166709_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_91379_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_91379_label/India_91379_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1149855_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1149855_label/Mekong_1149855_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1248200_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1248200_label/Mekong_1248200_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_53713_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_53713_label/Ghana_53713_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8372658_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8372658_label/Spain_8372658_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5678382_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5678382_label/Spain_5678382_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_287642_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_287642_label/India_287642_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_269835_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_269835_label/Mekong_269835_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_114964_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_114964_label/USA_114964_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_168875_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_168875_label/Ghana_168875_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_916628_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_916628_label/Sri-Lanka_916628_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_1167260_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_1167260_label/Spain_1167260_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_80221_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_80221_label/India_80221_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_664261_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_664261_label/USA_664261_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_519181_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_519181_label/USA_519181_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_770353_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_770353_label/USA_770353_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_31096_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_31096_label/Nigeria_31096_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_35915_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_35915_label/Pakistan_35915_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_638521_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_638521_label/USA_638521_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_403081_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_403081_label/Paraguay_403081_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_32375_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_32375_label/Somalia_32375_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_242570_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_242570_label/Bolivia_242570_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_707067_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_707067_label/Nigeria_707067_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1050276_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1050276_label/India_1050276_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_225017_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_225017_label/USA_225017_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_721886_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_721886_label/Paraguay_721886_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_195014_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_195014_label/Somalia_195014_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_167787_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_167787_label/Somalia_167787_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_698338_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_698338_label/India_698338_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_180633_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_180633_label/India_180633_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_992457_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_992457_label/Somalia_992457_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_45934_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_45934_label/Mekong_45934_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1018317_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1018317_label/India_1018317_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_308150_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_308150_label/USA_308150_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_667363_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_667363_label/Pakistan_667363_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_54421_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_54421_label/Paraguay_54421_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_271769_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_271769_label/Paraguay_271769_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_664410_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_664410_label/India_664410_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_24858_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_24858_label/Ghana_24858_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_383430_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_383430_label/India_383430_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_849649_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_849649_label/Sri-Lanka_849649_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6199994_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6199994_label/Spain_6199994_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_7931_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_7931_label/Somalia_7931_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_348639_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_348639_label/USA_348639_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_846007_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_846007_label/Mekong_846007_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_62897_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_62897_label/Paraguay_62897_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2594119_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2594119_label/Spain_2594119_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1049586_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1049586_label/USA_1049586_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_597288_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_597288_label/Ghana_597288_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_7894_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_7894_label/Paraguay_7894_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_595451_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_595451_label/USA_595451_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_842775_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_842775_label/India_842775_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_232060_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_232060_label/USA_232060_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_254910_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_254910_label/Mekong_254910_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_952728_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_952728_label/India_952728_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_548910_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_548910_label/Pakistan_548910_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_135713_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_135713_label/Sri-Lanka_135713_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_868895_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_868895_label/Paraguay_868895_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_70352_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_70352_label/India_70352_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_94095_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_94095_label/Pakistan_94095_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_1095404_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_1095404_label/Nigeria_1095404_label.json  
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/collection.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_347609_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_347609_label/USA_347609_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_163406_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_163406_label/Sri-Lanka_163406_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_285297_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_285297_label/India_285297_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_231124_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_231124_label/USA_231124_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_670826_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_670826_label/USA_670826_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_977338_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_977338_label/Mekong_977338_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_981708_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_981708_label/India_981708_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_591549_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_591549_label/India_591549_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_98310_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_98310_label/Mekong_98310_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_699062_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_699062_label/Somalia_699062_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_94102_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_94102_label/Somalia_94102_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_167553_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_167553_label/Pakistan_167553_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7786924_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7786924_label/Spain_7786924_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_115033_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_115033_label/USA_115033_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_48673_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_48673_label/Paraguay_48673_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_773682_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_773682_label/India_773682_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_9684_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_9684_label/Pakistan_9684_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_61925_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_61925_label/Ghana_61925_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_119477_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_119477_label/Mekong_119477_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_845821_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_845821_label/Sri-Lanka_845821_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_655230_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_655230_label/USA_655230_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_61368_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_61368_label/Somalia_61368_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_221789_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_221789_label/Mekong_221789_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_626316_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_626316_label/Somalia_626316_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_247288_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_247288_label/Ghana_247288_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_424793_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_424793_label/Mekong_424793_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_149787_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_149787_label/Paraguay_149787_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_772630_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_772630_label/India_772630_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_181263_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_181263_label/USA_181263_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_774689_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_774689_label/India_774689_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_233925_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_233925_label/Bolivia_233925_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_581976_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_581976_label/Paraguay_581976_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_103272_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_103272_label/Ghana_103272_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_474121_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_474121_label/Pakistan_474121_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_86502_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_86502_label/USA_86502_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_4282030_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_4282030_label/Spain_4282030_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1396181_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1396181_label/Mekong_1396181_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_373039_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_373039_label/India_373039_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1282475_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1282475_label/Mekong_1282475_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_691027_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_691027_label/India_691027_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_360519_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_360519_label/Bolivia_360519_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_207862_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_207862_label/India_207862_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_36146_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_36146_label/Paraguay_36146_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_156478_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_156478_label/Ghana_156478_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_713926_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_713926_label/Sri-Lanka_713926_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_551926_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_551926_label/Sri-Lanka_551926_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_312675_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_312675_label/Bolivia_312675_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1076204_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1076204_label/Paraguay_1076204_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_12849_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_12849_label/Somalia_12849_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1395593_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1395593_label/Mekong_1395593_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_212687_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_212687_label/Paraguay_212687_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_955053_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_955053_label/USA_955053_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_400518_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_400518_label/Sri-Lanka_400518_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_58086_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_58086_label/USA_58086_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_375183_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_375183_label/USA_375183_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2523247_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2523247_label/Spain_2523247_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_379434_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_379434_label/Bolivia_379434_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_905409_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_905409_label/USA_905409_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_213094_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_213094_label/Mekong_213094_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_828067_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_828067_label/India_828067_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_5079_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_5079_label/Ghana_5079_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_84195_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_84195_label/USA_84195_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_774566_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_774566_label/Mekong_774566_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1017769_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1017769_label/India_1017769_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_134751_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_134751_label/Ghana_134751_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_748447_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_748447_label/Sri-Lanka_748447_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_1036366_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_1036366_label/Pakistan_1036366_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_256539_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_256539_label/Somalia_256539_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_511199_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_511199_label/Paraguay_511199_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_195474_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_195474_label/Bolivia_195474_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_831672_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_831672_label/USA_831672_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_129334_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_129334_label/Bolivia_129334_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_1199913_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_1199913_label/Spain_1199913_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1443339_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1443339_label/Mekong_1443339_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_83200_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_83200_label/Ghana_83200_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1029042_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1029042_label/Paraguay_1029042_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_12870_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_12870_label/Paraguay_12870_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_683296_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_683296_label/Paraguay_683296_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_164336_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_164336_label/India_164336_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_534068_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_534068_label/Sri-Lanka_534068_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_534470_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_534470_label/India_534470_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_1027214_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_1027214_label/Pakistan_1027214_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_117737_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_117737_label/Sri-Lanka_117737_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_290290_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_290290_label/Bolivia_290290_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_19225_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_19225_label/USA_19225_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_66511_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_66511_label/USA_66511_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_166342_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_166342_label/Somalia_166342_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_4915752_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_4915752_label/Spain_4915752_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_142312_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_142312_label/Ghana_142312_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_869358_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_869358_label/India_869358_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_154838_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_154838_label/Ghana_154838_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8104659_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8104659_label/Spain_8104659_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_598959_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_598959_label/Nigeria_598959_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_761032_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_761032_label/USA_761032_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_566697_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_566697_label/India_566697_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_533192_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_533192_label/India_533192_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_135389_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_135389_label/Ghana_135389_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_232281_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_232281_label/Paraguay_232281_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_85652_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_85652_label/Sri-Lanka_85652_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_792268_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_792268_label/Paraguay_792268_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_892933_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_892933_label/Paraguay_892933_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_653336_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_653336_label/Sri-Lanka_653336_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8565131_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8565131_label/Spain_8565131_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_504150_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_504150_label/USA_504150_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_247656_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_247656_label/Paraguay_247656_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_103447_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_103447_label/India_103447_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_152185_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_152185_label/Sri-Lanka_152185_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_820924_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_820924_label/Nigeria_820924_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6095801_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6095801_label/Spain_6095801_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_994009_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_994009_label/USA_994009_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_198534_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_198534_label/Paraguay_198534_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_35845_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_35845_label/Nigeria_35845_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_913449_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_913449_label/Paraguay_913449_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_339807_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_339807_label/Paraguay_339807_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_791364_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_791364_label/Paraguay_791364_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_60129_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_60129_label/Somalia_60129_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_24341_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_24341_label/Paraguay_24341_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_500266_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_500266_label/India_500266_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_371421_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_371421_label/Somalia_371421_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_43105_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_43105_label/Pakistan_43105_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_76104_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_76104_label/Bolivia_76104_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_417184_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_417184_label/Nigeria_417184_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_23014_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_23014_label/Bolivia_23014_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_40936_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_40936_label/Paraguay_40936_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_664885_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_664885_label/Pakistan_664885_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_849790_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_849790_label/Pakistan_849790_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_934240_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_934240_label/Paraguay_934240_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6537196_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6537196_label/Spain_6537196_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_984831_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_984831_label/Nigeria_984831_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_883641_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_883641_label/Sri-Lanka_883641_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_211386_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_211386_label/Pakistan_211386_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_646878_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_646878_label/USA_646878_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_631692_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_631692_label/India_631692_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_652725_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_652725_label/India_652725_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_16233_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_16233_label/Mekong_16233_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_246154_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_246154_label/Paraguay_246154_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1413877_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1413877_label/Mekong_1413877_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5816638_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5816638_label/Spain_5816638_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_342411_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_342411_label/Mekong_342411_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_52223_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_52223_label/Sri-Lanka_52223_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_49764_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_49764_label/Sri-Lanka_49764_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_986268_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_986268_label/USA_986268_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_146222_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_146222_label/Ghana_146222_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_359826_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_359826_label/Ghana_359826_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_236030_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_236030_label/Sri-Lanka_236030_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_868803_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_868803_label/Ghana_868803_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_570384_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_570384_label/India_570384_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_8090_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_8090_label/Ghana_8090_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_179238_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_179238_label/India_179238_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_812045_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_812045_label/Nigeria_812045_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_760290_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_760290_label/Pakistan_760290_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_45911_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_45911_label/Ghana_45911_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1068362_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1068362_label/USA_1068362_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8199661_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8199661_label/Spain_8199661_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_806273_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_806273_label/USA_806273_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2938657_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2938657_label/Spain_2938657_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_11422_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_11422_label/USA_11422_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_224845_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_224845_label/Paraguay_224845_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_592446_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_592446_label/India_592446_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_65724_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_65724_label/Pakistan_65724_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1111068_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1111068_label/Mekong_1111068_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_439488_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_439488_label/Nigeria_439488_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_895194_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_895194_label/Ghana_895194_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_847275_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_847275_label/Sri-Lanka_847275_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_826217_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_826217_label/USA_826217_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_148318_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_148318_label/Paraguay_148318_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_59731_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_59731_label/Paraguay_59731_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_651904_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_651904_label/Paraguay_651904_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_377277_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_377277_label/Sri-Lanka_377277_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_275372_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_275372_label/USA_275372_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_205585_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_205585_label/Paraguay_205585_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_225187_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_225187_label/Paraguay_225187_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_432776_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_432776_label/Bolivia_432776_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_1087508_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_1087508_label/Somalia_1087508_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_605492_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_605492_label/USA_605492_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_391908_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_391908_label/India_391908_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_149830_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_149830_label/Paraguay_149830_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_273873_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_273873_label/India_273873_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_336228_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_336228_label/Pakistan_336228_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_11869_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_11869_label/Paraguay_11869_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_900498_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_900498_label/India_900498_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_970508_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_970508_label/Somalia_970508_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_22088_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_22088_label/Nigeria_22088_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_747992_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_747992_label/India_747992_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_909806_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_909806_label/Pakistan_909806_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_181503_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_181503_label/USA_181503_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_187318_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_187318_label/Ghana_187318_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_284928_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_284928_label/Paraguay_284928_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_886726_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_886726_label/Somalia_886726_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1039203_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1039203_label/USA_1039203_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_529525_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_529525_label/Nigeria_529525_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_97516_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_97516_label/Ghana_97516_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1010394_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_1010394_label/USA_1010394_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_179917_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_179917_label/USA_179917_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_126224_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_126224_label/Paraguay_126224_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_350244_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_350244_label/USA_350244_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_887131_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_887131_label/Ghana_887131_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_319168_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_319168_label/Ghana_319168_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1018327_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1018327_label/India_1018327_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_1049830_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_1049830_label/Sri-Lanka_1049830_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_92824_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_92824_label/Sri-Lanka_92824_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_922373_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_922373_label/Mekong_922373_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_922192_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_922192_label/Sri-Lanka_922192_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_244057_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_244057_label/India_244057_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_795075_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_795075_label/Paraguay_795075_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_470303_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_470303_label/Paraguay_470303_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_716716_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_716716_label/Spain_716716_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_230192_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_230192_label/Somalia_230192_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_354981_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_354981_label/USA_354981_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_596495_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_596495_label/Mekong_596495_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_685158_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_685158_label/Somalia_685158_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_712873_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_712873_label/Pakistan_712873_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_179624_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_179624_label/Paraguay_179624_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1191208_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1191208_label/Mekong_1191208_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_747970_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_747970_label/India_747970_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_93023_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_93023_label/Somalia_93023_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_101973_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_101973_label/Sri-Lanka_101973_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_1068756_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_1068756_label/Somalia_1068756_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8154154_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_8154154_label/Spain_8154154_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_14484_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_14484_label/Sri-Lanka_14484_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_81933_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_81933_label/Nigeria_81933_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7387658_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7387658_label/Spain_7387658_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_657443_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_657443_label/Paraguay_657443_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_26376_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_26376_label/Ghana_26376_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_295782_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_295782_label/Somalia_295782_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_246718_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_246718_label/Pakistan_246718_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_769408_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_769408_label/India_769408_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_366265_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_366265_label/Pakistan_366265_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_211406_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_211406_label/USA_211406_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_648632_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_648632_label/Paraguay_648632_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_362274_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_362274_label/Ghana_362274_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_215904_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_215904_label/Paraguay_215904_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_997480_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_997480_label/Paraguay_997480_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_979278_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_979278_label/India_979278_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_70625_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_70625_label/Pakistan_70625_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_55568_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_55568_label/Sri-Lanka_55568_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_313799_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_313799_label/Ghana_313799_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_136196_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_136196_label/India_136196_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_277_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_277_label/Ghana_277_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_486103_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_486103_label/USA_486103_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_52610_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_52610_label/Mekong_52610_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_438959_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_438959_label/USA_438959_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1072277_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1072277_label/India_1072277_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_141271_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_141271_label/Ghana_141271_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_322855_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_322855_label/Somalia_322855_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_141910_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_141910_label/Ghana_141910_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_161233_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_161233_label/Ghana_161233_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_933610_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_933610_label/USA_933610_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_132163_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_132163_label/Ghana_132163_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_305760_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_305760_label/Paraguay_305760_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_591317_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_591317_label/India_591317_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_741073_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_741073_label/USA_741073_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2472849_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_2472849_label/Spain_2472849_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_527077_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_527077_label/USA_527077_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_790830_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_790830_label/Paraguay_790830_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_118868_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_118868_label/India_118868_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_366607_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_366607_label/USA_366607_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_79637_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_79637_label/India_79637_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_788696_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_788696_label/USA_788696_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_63307_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_63307_label/Sri-Lanka_63307_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_649970_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_649970_label/Sri-Lanka_649970_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_132922_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_132922_label/Sri-Lanka_132922_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_143329_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_143329_label/Nigeria_143329_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_167233_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_167233_label/Ghana_167233_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_172476_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_172476_label/Paraguay_172476_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_294583_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_294583_label/Bolivia_294583_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_741178_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_741178_label/USA_741178_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_943439_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_943439_label/India_943439_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_25540_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_25540_label/India_25540_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_333434_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_333434_label/Mekong_333434_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5650136_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5650136_label/Spain_5650136_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_600295_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_600295_label/Nigeria_600295_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_956930_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_956930_label/India_956930_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6860600_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_6860600_label/Spain_6860600_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_260929_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_260929_label/USA_260929_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7604243_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7604243_label/Spain_7604243_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_337094_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_337094_label/Spain_337094_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_952958_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_952958_label/Nigeria_952958_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1056717_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1056717_label/Paraguay_1056717_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_293769_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_293769_label/Mekong_293769_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_482517_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_482517_label/Paraguay_482517_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_80102_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_80102_label/Paraguay_80102_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_605682_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_605682_label/Paraguay_605682_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1019808_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1019808_label/Paraguay_1019808_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_78061_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_78061_label/Nigeria_78061_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_124834_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_124834_label/Ghana_124834_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_694942_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_694942_label/Pakistan_694942_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_97059_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_97059_label/Ghana_97059_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_3285448_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_3285448_label/Spain_3285448_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1068117_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_1068117_label/India_1068117_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_144050_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_144050_label/Ghana_144050_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_523539_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_523539_label/Sri-Lanka_523539_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7558720_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7558720_label/Spain_7558720_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_224165_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_224165_label/USA_224165_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_450918_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_450918_label/Sri-Lanka_450918_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_612594_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_612594_label/Sri-Lanka_612594_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_44475_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_44475_label/India_44475_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_246510_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_246510_label/Pakistan_246510_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_34417_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_34417_label/Paraguay_34417_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_205466_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_205466_label/Somalia_205466_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_103757_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_103757_label/Bolivia_103757_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_49890_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_49890_label/Ghana_49890_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_76868_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_76868_label/Paraguay_76868_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_252217_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_252217_label/Paraguay_252217_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_59460_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_59460_label/India_59460_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_280900_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_280900_label/Paraguay_280900_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_822142_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_822142_label/Paraguay_822142_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_778194_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_778194_label/USA_778194_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_170264_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_170264_label/USA_170264_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_387945_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_387945_label/USA_387945_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_66026_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_66026_label/USA_66026_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_758178_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_758178_label/USA_758178_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1439641_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_1439641_label/Mekong_1439641_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_191503_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_191503_label/Paraguay_191503_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_989553_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_989553_label/Somalia_989553_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_225131_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Nigeria_225131_label/Nigeria_225131_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_382276_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Mekong_382276_label/Mekong_382276_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_236628_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_236628_label/Sri-Lanka_236628_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_1038087_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_1038087_label/Sri-Lanka_1038087_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_693819_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_693819_label/USA_693819_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_73419_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_73419_label/India_73419_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5923267_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_5923267_label/Spain_5923267_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_399883_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_399883_label/India_399883_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_194723_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_194723_label/Ghana_194723_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_132143_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_132143_label/Pakistan_132143_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_36015_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_36015_label/Paraguay_36015_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_233609_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_233609_label/Sri-Lanka_233609_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_495107_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_495107_label/Ghana_495107_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_56450_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_56450_label/India_56450_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_624341_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_624341_label/India_624341_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_324254_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_324254_label/India_324254_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_649376_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Somalia_649376_label/Somalia_649376_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_128663_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_128663_label/Ghana_128663_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_234935_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_234935_label/Ghana_234935_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_652955_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_652955_label/USA_652955_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_60373_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_60373_label/Bolivia_60373_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_604222_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_604222_label/USA_604222_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_308249_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_308249_label/Ghana_308249_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_764946_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_764946_label/India_764946_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_67102_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_67102_label/USA_67102_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_217598_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_217598_label/USA_217598_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_707886_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_707886_label/India_707886_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_866994_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_866994_label/Ghana_866994_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_921838_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_921838_label/Paraguay_921838_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1078550_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1078550_label/Ghana_1078550_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1089161_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1089161_label/Ghana_1089161_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_528249_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_528249_label/Pakistan_528249_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_989230_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_989230_label/Paraguay_989230_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_251323_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_251323_label/USA_251323_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_83483_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_83483_label/Ghana_83483_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_31559_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_31559_label/Sri-Lanka_31559_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_135434_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_135434_label/India_135434_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_7496_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_7496_label/Ghana_7496_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_908474_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_908474_label/USA_908474_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_401863_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_401863_label/Pakistan_401863_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_740461_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_740461_label/Pakistan_740461_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_198411_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_198411_label/USA_198411_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_210595_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Pakistan_210595_label/Pakistan_210595_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_953791_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_953791_label/Ghana_953791_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_804466_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_804466_label/India_804466_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_406026_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_406026_label/Ghana_406026_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_11745_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_11745_label/Ghana_11745_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7856615_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7856615_label/Spain_7856615_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_956740_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_956740_label/Sri-Lanka_956740_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_430764_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/USA_430764_label/USA_430764_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_579082_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_579082_label/Sri-Lanka_579082_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1033830_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_1033830_label/Ghana_1033830_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_265762_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_265762_label/India_265762_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_249079_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_249079_label/Sri-Lanka_249079_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_153941_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_153941_label/Paraguay_153941_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_120804_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_120804_label/Sri-Lanka_120804_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_178753_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Sri-Lanka_178753_label/Sri-Lanka_178753_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_147015_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_147015_label/Ghana_147015_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1029191_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Paraguay_1029191_label/Paraguay_1029191_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_177319_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_177319_label/India_177319_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7370579_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Spain_7370579_label/Spain_7370579_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/India_833266_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/India_833266_label/India_833266_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_314919_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Bolivia_314919_label/Bolivia_314919_label.json  
   creating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_264787_label/
  inflating: flood_data/catalog/sen1floods11_hand_labeled_label/Ghana_264787_label/Ghana_264787_label.json  
  inflating: flood_data/catalog/catalog.json  
   creating: flood_data/images/
   creating: flood_data/images/all_images/
  inflating: flood_data/images/all_images/Bolivia_312675.png  
  inflating: flood_data/images/all_images/Paraguay_1076204.png  
  inflating: flood_data/images/all_images/Somalia_12849.png  
  inflating: flood_data/images/all_images/Sri-Lanka_713926.png  
  inflating: flood_data/images/all_images/Sri-Lanka_551926.png  
  inflating: flood_data/images/all_images/Ghana_156478.png  
  inflating: flood_data/images/all_images/Paraguay_36146.png  
  inflating: flood_data/images/all_images/India_207862.png  
  inflating: flood_data/images/all_images/USA_86502.png  
  inflating: flood_data/images/all_images/Spain_4282030.png  
  inflating: flood_data/images/all_images/Pakistan_474121.png  
  inflating: flood_data/images/all_images/Ghana_103272.png  
  inflating: flood_data/images/all_images/Paraguay_581976.png  
  inflating: flood_data/images/all_images/Bolivia_360519.png  
  inflating: flood_data/images/all_images/India_691027.png  
  inflating: flood_data/images/all_images/Mekong_1282475.png  
  inflating: flood_data/images/all_images/Mekong_1396181.png  
  inflating: flood_data/images/all_images/India_373039.png  
  inflating: flood_data/images/all_images/Somalia_626316.png  
  inflating: flood_data/images/all_images/Mekong_221789.png  
  inflating: flood_data/images/all_images/Somalia_61368.png  
  inflating: flood_data/images/all_images/USA_655230.png  
  inflating: flood_data/images/all_images/Mekong_119477.png  
  inflating: flood_data/images/all_images/Sri-Lanka_845821.png  
  inflating: flood_data/images/all_images/Mekong_424793.png  
  inflating: flood_data/images/all_images/Ghana_247288.png  
  inflating: flood_data/images/all_images/USA_181263.png  
  inflating: flood_data/images/all_images/India_772630.png  
  inflating: flood_data/images/all_images/Paraguay_149787.png  
  inflating: flood_data/images/all_images/Bolivia_233925.png  
  inflating: flood_data/images/all_images/India_774689.png  
  inflating: flood_data/images/all_images/Ghana_597288.png  
  inflating: flood_data/images/all_images/Mekong_254910.png  
  inflating: flood_data/images/all_images/USA_232060.png  
  inflating: flood_data/images/all_images/Paraguay_7894.png  
  inflating: flood_data/images/all_images/USA_595451.png  
  inflating: flood_data/images/all_images/India_842775.png  
  inflating: flood_data/images/all_images/Pakistan_94095.png  
  inflating: flood_data/images/all_images/Nigeria_1095404.png  
  inflating: flood_data/images/all_images/India_70352.png  
  inflating: flood_data/images/all_images/Paraguay_868895.png  
  inflating: flood_data/images/all_images/Sri-Lanka_135713.png  
  inflating: flood_data/images/all_images/Pakistan_548910.png  
  inflating: flood_data/images/all_images/India_952728.png  
  inflating: flood_data/images/all_images/USA_347609.png  
  inflating: flood_data/images/all_images/Somalia_699062.png  
  inflating: flood_data/images/all_images/Mekong_98310.png  
  inflating: flood_data/images/all_images/India_591549.png  
  inflating: flood_data/images/all_images/India_981708.png  
  inflating: flood_data/images/all_images/India_285297.png  
  inflating: flood_data/images/all_images/USA_231124.png  
  inflating: flood_data/images/all_images/Sri-Lanka_163406.png  
  inflating: flood_data/images/all_images/USA_670826.png  
  inflating: flood_data/images/all_images/Mekong_977338.png  
  inflating: flood_data/images/all_images/Paraguay_48673.png  
  inflating: flood_data/images/all_images/India_773682.png  
  inflating: flood_data/images/all_images/Somalia_94102.png  
  inflating: flood_data/images/all_images/Pakistan_167553.png  
  inflating: flood_data/images/all_images/Spain_7786924.png  
  inflating: flood_data/images/all_images/USA_115033.png  
  inflating: flood_data/images/all_images/Pakistan_9684.png  
  inflating: flood_data/images/all_images/Ghana_61925.png  
  inflating: flood_data/images/all_images/Paraguay_896458.png  
  inflating: flood_data/images/all_images/Sri-Lanka_321316.png  
  inflating: flood_data/images/all_images/Paraguay_44682.png  
  inflating: flood_data/images/all_images/Mekong_474783.png  
  inflating: flood_data/images/all_images/USA_1082482.png  
  inflating: flood_data/images/all_images/India_91379.png  
  inflating: flood_data/images/all_images/Mekong_1248200.png  
  inflating: flood_data/images/all_images/Mekong_1149855.png  
  inflating: flood_data/images/all_images/India_166709.png  
  inflating: flood_data/images/all_images/Ghana_53713.png  
  inflating: flood_data/images/all_images/Spain_8372658.png  
  inflating: flood_data/images/all_images/India_287642.png  
  inflating: flood_data/images/all_images/Mekong_269835.png  
  inflating: flood_data/images/all_images/Spain_5678382.png  
  inflating: flood_data/images/all_images/Ghana_168875.png  
  inflating: flood_data/images/all_images/USA_114964.png  
  inflating: flood_data/images/all_images/Sri-Lanka_916628.png  
  inflating: flood_data/images/all_images/Spain_1167260.png  
  inflating: flood_data/images/all_images/India_80221.png  
  inflating: flood_data/images/all_images/USA_664261.png  
  inflating: flood_data/images/all_images/USA_519181.png  
  inflating: flood_data/images/all_images/Nigeria_31096.png  
  inflating: flood_data/images/all_images/Pakistan_35915.png  
  inflating: flood_data/images/all_images/USA_770353.png  
  inflating: flood_data/images/all_images/USA_638521.png  
  inflating: flood_data/images/all_images/Paraguay_403081.png  
  inflating: flood_data/images/all_images/Somalia_32375.png  
  inflating: flood_data/images/all_images/Bolivia_242570.png  
  inflating: flood_data/images/all_images/India_1050276.png  
  inflating: flood_data/images/all_images/Nigeria_707067.png  
  inflating: flood_data/images/all_images/USA_225017.png  
  inflating: flood_data/images/all_images/Somalia_195014.png  
  inflating: flood_data/images/all_images/Somalia_167787.png  
  inflating: flood_data/images/all_images/Paraguay_721886.png  
  inflating: flood_data/images/all_images/India_180633.png  
  inflating: flood_data/images/all_images/India_698338.png  
  inflating: flood_data/images/all_images/Somalia_992457.png  
  inflating: flood_data/images/all_images/India_1018317.png  
  inflating: flood_data/images/all_images/Mekong_45934.png  
  inflating: flood_data/images/all_images/USA_308150.png  
  inflating: flood_data/images/all_images/Pakistan_667363.png  
  inflating: flood_data/images/all_images/Paraguay_54421.png  
  inflating: flood_data/images/all_images/Paraguay_271769.png  
  inflating: flood_data/images/all_images/India_664410.png  
  inflating: flood_data/images/all_images/Ghana_24858.png  
  inflating: flood_data/images/all_images/India_383430.png  
  inflating: flood_data/images/all_images/Sri-Lanka_849649.png  
  inflating: flood_data/images/all_images/Spain_6199994.png  
  inflating: flood_data/images/all_images/Somalia_7931.png  
  inflating: flood_data/images/all_images/USA_348639.png  
  inflating: flood_data/images/all_images/Mekong_846007.png  
  inflating: flood_data/images/all_images/Paraguay_62897.png  
  inflating: flood_data/images/all_images/Spain_2594119.png  
  inflating: flood_data/images/all_images/USA_1049586.png  
  inflating: flood_data/images/all_images/Ghana_8090.png  
  inflating: flood_data/images/all_images/Ghana_868803.png  
  inflating: flood_data/images/all_images/Sri-Lanka_236030.png  
  inflating: flood_data/images/all_images/India_570384.png  
  inflating: flood_data/images/all_images/Ghana_359826.png  
  inflating: flood_data/images/all_images/Ghana_146222.png  
  inflating: flood_data/images/all_images/Pakistan_211386.png  
  inflating: flood_data/images/all_images/USA_646878.png  
  inflating: flood_data/images/all_images/India_631692.png  
  inflating: flood_data/images/all_images/Sri-Lanka_883641.png  
  inflating: flood_data/images/all_images/Nigeria_984831.png  
  inflating: flood_data/images/all_images/Spain_6537196.png  
  inflating: flood_data/images/all_images/Paraguay_934240.png  
  inflating: flood_data/images/all_images/Paraguay_40936.png  
  inflating: flood_data/images/all_images/Bolivia_23014.png  
  inflating: flood_data/images/all_images/Pakistan_849790.png  
  inflating: flood_data/images/all_images/Pakistan_664885.png  
  inflating: flood_data/images/all_images/Sri-Lanka_52223.png  
  inflating: flood_data/images/all_images/Sri-Lanka_49764.png  
  inflating: flood_data/images/all_images/USA_986268.png  
  inflating: flood_data/images/all_images/Mekong_342411.png  
  inflating: flood_data/images/all_images/Spain_5816638.png  
  inflating: flood_data/images/all_images/Mekong_16233.png  
  inflating: flood_data/images/all_images/India_652725.png  
  inflating: flood_data/images/all_images/Paraguay_246154.png  
  inflating: flood_data/images/all_images/Mekong_1413877.png  
  inflating: flood_data/images/all_images/Nigeria_820924.png  
  inflating: flood_data/images/all_images/Sri-Lanka_152185.png  
  inflating: flood_data/images/all_images/India_103447.png  
  inflating: flood_data/images/all_images/Spain_8565131.png  
  inflating: flood_data/images/all_images/USA_504150.png  
  inflating: flood_data/images/all_images/Paraguay_247656.png  
  inflating: flood_data/images/all_images/Paraguay_791364.png  
  inflating: flood_data/images/all_images/Paraguay_339807.png  
  inflating: flood_data/images/all_images/Paraguay_913449.png  
  inflating: flood_data/images/all_images/Paraguay_198534.png  
  inflating: flood_data/images/all_images/Nigeria_35845.png  
  inflating: flood_data/images/all_images/Spain_6095801.png  
  inflating: flood_data/images/all_images/USA_994009.png  
  inflating: flood_data/images/all_images/Somalia_371421.png  
  inflating: flood_data/images/all_images/India_500266.png  
  inflating: flood_data/images/all_images/Somalia_60129.png  
  inflating: flood_data/images/all_images/Paraguay_24341.png  
  inflating: flood_data/images/all_images/Nigeria_417184.png  
  inflating: flood_data/images/all_images/Bolivia_76104.png  
  inflating: flood_data/images/all_images/Pakistan_43105.png  
  inflating: flood_data/images/all_images/Paraguay_212687.png  
  inflating: flood_data/images/all_images/Mekong_1395593.png  
  inflating: flood_data/images/all_images/USA_58086.png  
  inflating: flood_data/images/all_images/Sri-Lanka_400518.png  
  inflating: flood_data/images/all_images/USA_955053.png  
  inflating: flood_data/images/all_images/Ghana_134751.png  
  inflating: flood_data/images/all_images/India_1017769.png  
  inflating: flood_data/images/all_images/Mekong_774566.png  
  inflating: flood_data/images/all_images/USA_84195.png  
  inflating: flood_data/images/all_images/USA_375183.png  
  inflating: flood_data/images/all_images/Spain_2523247.png  
  inflating: flood_data/images/all_images/Mekong_213094.png  
  inflating: flood_data/images/all_images/India_828067.png  
  inflating: flood_data/images/all_images/Ghana_5079.png  
  inflating: flood_data/images/all_images/USA_905409.png  
  inflating: flood_data/images/all_images/Bolivia_379434.png  
  inflating: flood_data/images/all_images/USA_831672.png  
  inflating: flood_data/images/all_images/Bolivia_195474.png  
  inflating: flood_data/images/all_images/Paraguay_511199.png  
  inflating: flood_data/images/all_images/Somalia_256539.png  
  inflating: flood_data/images/all_images/Sri-Lanka_748447.png  
  inflating: flood_data/images/all_images/Pakistan_1036366.png  
  inflating: flood_data/images/all_images/Paraguay_12870.png  
  inflating: flood_data/images/all_images/Paraguay_683296.png  
  inflating: flood_data/images/all_images/India_164336.png  
  inflating: flood_data/images/all_images/Ghana_83200.png  
  inflating: flood_data/images/all_images/Paraguay_1029042.png  
  inflating: flood_data/images/all_images/Bolivia_129334.png  
  inflating: flood_data/images/all_images/Spain_1199913.png  
  inflating: flood_data/images/all_images/Mekong_1443339.png  
  inflating: flood_data/images/all_images/USA_19225.png  
  inflating: flood_data/images/all_images/Somalia_166342.png  
  inflating: flood_data/images/all_images/USA_66511.png  
  inflating: flood_data/images/all_images/Spain_4915752.png  
  inflating: flood_data/images/all_images/Ghana_142312.png  
  inflating: flood_data/images/all_images/Bolivia_290290.png  
  inflating: flood_data/images/all_images/Sri-Lanka_117737.png  
  inflating: flood_data/images/all_images/Pakistan_1027214.png  
  inflating: flood_data/images/all_images/India_534470.png  
  inflating: flood_data/images/all_images/Sri-Lanka_534068.png  
  inflating: flood_data/images/all_images/Ghana_154838.png  
  inflating: flood_data/images/all_images/Spain_8104659.png  
  inflating: flood_data/images/all_images/USA_761032.png  
  inflating: flood_data/images/all_images/Nigeria_598959.png  
  inflating: flood_data/images/all_images/India_869358.png  
  inflating: flood_data/images/all_images/Sri-Lanka_85652.png  
  inflating: flood_data/images/all_images/Paraguay_232281.png  
  inflating: flood_data/images/all_images/Paraguay_892933.png  
  inflating: flood_data/images/all_images/Paraguay_792268.png  
  inflating: flood_data/images/all_images/Sri-Lanka_653336.png  
  inflating: flood_data/images/all_images/India_533192.png  
  inflating: flood_data/images/all_images/India_566697.png  
  inflating: flood_data/images/all_images/Ghana_135389.png  
  inflating: flood_data/images/all_images/Ghana_141910.png  
  inflating: flood_data/images/all_images/Somalia_322855.png  
  inflating: flood_data/images/all_images/Ghana_141271.png  
  inflating: flood_data/images/all_images/Ghana_132163.png  
  inflating: flood_data/images/all_images/USA_933610.png  
  inflating: flood_data/images/all_images/Ghana_161233.png  
  inflating: flood_data/images/all_images/India_591317.png  
  inflating: flood_data/images/all_images/USA_741073.png  
  inflating: flood_data/images/all_images/Spain_2472849.png  
  inflating: flood_data/images/all_images/Paraguay_305760.png  
  inflating: flood_data/images/all_images/Ghana_313799.png  
  inflating: flood_data/images/all_images/India_136196.png  
  inflating: flood_data/images/all_images/India_1072277.png  
  inflating: flood_data/images/all_images/USA_438959.png  
  inflating: flood_data/images/all_images/USA_486103.png  
  inflating: flood_data/images/all_images/Ghana_277.png  
  inflating: flood_data/images/all_images/Mekong_52610.png  
  inflating: flood_data/images/all_images/Sri-Lanka_55568.png  
  inflating: flood_data/images/all_images/India_979278.png  
  inflating: flood_data/images/all_images/Pakistan_70625.png  
  inflating: flood_data/images/all_images/Paraguay_215904.png  
  inflating: flood_data/images/all_images/Paraguay_997480.png  
  inflating: flood_data/images/all_images/Sri-Lanka_101973.png  
  inflating: flood_data/images/all_images/India_747970.png  
  inflating: flood_data/images/all_images/Somalia_93023.png  
  inflating: flood_data/images/all_images/Mekong_1191208.png  
  inflating: flood_data/images/all_images/Paraguay_179624.png  
  inflating: flood_data/images/all_images/Pakistan_712873.png  
  inflating: flood_data/images/all_images/Somalia_685158.png  
  inflating: flood_data/images/all_images/Mekong_596495.png  
  inflating: flood_data/images/all_images/Somalia_230192.png  
  inflating: flood_data/images/all_images/Spain_716716.png  
  inflating: flood_data/images/all_images/USA_354981.png  
  inflating: flood_data/images/all_images/Pakistan_366265.png  
  inflating: flood_data/images/all_images/Pakistan_246718.png  
  inflating: flood_data/images/all_images/Somalia_295782.png  
  inflating: flood_data/images/all_images/India_769408.png  
  inflating: flood_data/images/all_images/Ghana_362274.png  
  inflating: flood_data/images/all_images/Paraguay_648632.png  
  inflating: flood_data/images/all_images/USA_211406.png  
  inflating: flood_data/images/all_images/Spain_7387658.png  
  inflating: flood_data/images/all_images/Paraguay_657443.png  
  inflating: flood_data/images/all_images/Ghana_26376.png  
  inflating: flood_data/images/all_images/Spain_8154154.png  
  inflating: flood_data/images/all_images/Somalia_1068756.png  
  inflating: flood_data/images/all_images/Nigeria_81933.png  
  inflating: flood_data/images/all_images/Sri-Lanka_14484.png  
  inflating: flood_data/images/all_images/Pakistan_65724.png  
  inflating: flood_data/images/all_images/Nigeria_439488.png  
  inflating: flood_data/images/all_images/Mekong_1111068.png  
  inflating: flood_data/images/all_images/USA_826217.png  
  inflating: flood_data/images/all_images/Sri-Lanka_847275.png  
  inflating: flood_data/images/all_images/Ghana_895194.png  
  inflating: flood_data/images/all_images/Paraguay_148318.png  
  inflating: flood_data/images/all_images/Paraguay_59731.png  
  inflating: flood_data/images/all_images/Spain_8199661.png  
  inflating: flood_data/images/all_images/USA_1068362.png  
  inflating: flood_data/images/all_images/Spain_2938657.png  
  inflating: flood_data/images/all_images/USA_806273.png  
  inflating: flood_data/images/all_images/USA_11422.png  
  inflating: flood_data/images/all_images/Paraguay_224845.png  
  inflating: flood_data/images/all_images/India_592446.png  
  inflating: flood_data/images/all_images/Ghana_45911.png  
  inflating: flood_data/images/all_images/Pakistan_760290.png  
  inflating: flood_data/images/all_images/Nigeria_812045.png  
  inflating: flood_data/images/all_images/India_179238.png  
  inflating: flood_data/images/all_images/India_273873.png  
  inflating: flood_data/images/all_images/Pakistan_336228.png  
  inflating: flood_data/images/all_images/India_900498.png  
  inflating: flood_data/images/all_images/Paraguay_11869.png  
  inflating: flood_data/images/all_images/Somalia_970508.png  
  inflating: flood_data/images/all_images/Nigeria_22088.png  
  inflating: flood_data/images/all_images/Bolivia_432776.png  
  inflating: flood_data/images/all_images/Paraguay_225187.png  
  inflating: flood_data/images/all_images/Paraguay_205585.png  
  inflating: flood_data/images/all_images/Somalia_1087508.png  
  inflating: flood_data/images/all_images/India_391908.png  
  inflating: flood_data/images/all_images/USA_605492.png  
  inflating: flood_data/images/all_images/Paraguay_149830.png  
  inflating: flood_data/images/all_images/USA_275372.png  
  inflating: flood_data/images/all_images/Sri-Lanka_377277.png  
  inflating: flood_data/images/all_images/Paraguay_651904.png  
  inflating: flood_data/images/all_images/USA_1039203.png  
  inflating: flood_data/images/all_images/Nigeria_529525.png  
  inflating: flood_data/images/all_images/Somalia_886726.png  
  inflating: flood_data/images/all_images/USA_1010394.png  
  inflating: flood_data/images/all_images/Ghana_97516.png  
  inflating: flood_data/images/all_images/USA_179917.png  
  inflating: flood_data/images/all_images/Paraguay_126224.png  
  inflating: flood_data/images/all_images/Paraguay_284928.png  
  inflating: flood_data/images/all_images/Ghana_187318.png  
  inflating: flood_data/images/all_images/USA_181503.png  
  inflating: flood_data/images/all_images/Pakistan_909806.png  
  inflating: flood_data/images/all_images/India_747992.png  
  inflating: flood_data/images/all_images/Mekong_922373.png  
  inflating: flood_data/images/all_images/Sri-Lanka_922192.png  
  inflating: flood_data/images/all_images/Paraguay_795075.png  
  inflating: flood_data/images/all_images/India_244057.png  
  inflating: flood_data/images/all_images/Paraguay_470303.png  
  inflating: flood_data/images/all_images/Sri-Lanka_92824.png  
  inflating: flood_data/images/all_images/Sri-Lanka_1049830.png  
  inflating: flood_data/images/all_images/India_1018327.png  
  inflating: flood_data/images/all_images/Ghana_319168.png  
  inflating: flood_data/images/all_images/Ghana_887131.png  
  inflating: flood_data/images/all_images/USA_350244.png  
  inflating: flood_data/images/all_images/India_177319.png  
  inflating: flood_data/images/all_images/Paraguay_1029191.png  
  inflating: flood_data/images/all_images/Sri-Lanka_249079.png  
  inflating: flood_data/images/all_images/India_265762.png  
  inflating: flood_data/images/all_images/Paraguay_153941.png  
  inflating: flood_data/images/all_images/Sri-Lanka_120804.png  
  inflating: flood_data/images/all_images/Sri-Lanka_178753.png  
  inflating: flood_data/images/all_images/Ghana_147015.png  
  inflating: flood_data/images/all_images/Sri-Lanka_579082.png  
  inflating: flood_data/images/all_images/Ghana_1033830.png  
  inflating: flood_data/images/all_images/Bolivia_314919.png  
  inflating: flood_data/images/all_images/Ghana_264787.png  
  inflating: flood_data/images/all_images/Spain_7370579.png  
  inflating: flood_data/images/all_images/India_833266.png  
  inflating: flood_data/images/all_images/USA_430764.png  
  inflating: flood_data/images/all_images/Sri-Lanka_956740.png  
  inflating: flood_data/images/all_images/Spain_7856615.png  
  inflating: flood_data/images/all_images/Ghana_406026.png  
  inflating: flood_data/images/all_images/India_804466.png  
  inflating: flood_data/images/all_images/Ghana_11745.png  
  inflating: flood_data/images/all_images/Pakistan_401863.png  
  inflating: flood_data/images/all_images/USA_198411.png  
  inflating: flood_data/images/all_images/Pakistan_740461.png  
  inflating: flood_data/images/all_images/Pakistan_210595.png  
  inflating: flood_data/images/all_images/Ghana_953791.png  
  inflating: flood_data/images/all_images/USA_67102.png  
  inflating: flood_data/images/all_images/India_764946.png  
  inflating: flood_data/images/all_images/Ghana_234935.png  
  inflating: flood_data/images/all_images/Somalia_649376.png  
  inflating: flood_data/images/all_images/Ghana_128663.png  
  inflating: flood_data/images/all_images/Bolivia_60373.png  
  inflating: flood_data/images/all_images/Ghana_308249.png  
  inflating: flood_data/images/all_images/USA_604222.png  
  inflating: flood_data/images/all_images/USA_652955.png  
  inflating: flood_data/images/all_images/Paraguay_36015.png  
  inflating: flood_data/images/all_images/Pakistan_132143.png  
  inflating: flood_data/images/all_images/Ghana_194723.png  
  inflating: flood_data/images/all_images/Ghana_495107.png  
  inflating: flood_data/images/all_images/Sri-Lanka_233609.png  
  inflating: flood_data/images/all_images/India_324254.png  
  inflating: flood_data/images/all_images/India_624341.png  
  inflating: flood_data/images/all_images/India_56450.png  
  inflating: flood_data/images/all_images/Ghana_7496.png  
  inflating: flood_data/images/all_images/USA_908474.png  
  inflating: flood_data/images/all_images/Sri-Lanka_31559.png  
  inflating: flood_data/images/all_images/Ghana_83483.png  
  inflating: flood_data/images/all_images/USA_251323.png  
  inflating: flood_data/images/all_images/India_135434.png  
  inflating: flood_data/images/all_images/India_707886.png  
  inflating: flood_data/images/all_images/USA_217598.png  
  inflating: flood_data/images/all_images/Paraguay_921838.png  
  inflating: flood_data/images/all_images/Ghana_866994.png  
  inflating: flood_data/images/all_images/Ghana_1089161.png  
  inflating: flood_data/images/all_images/Pakistan_528249.png  
  inflating: flood_data/images/all_images/Ghana_1078550.png  
  inflating: flood_data/images/all_images/Paraguay_989230.png  
  inflating: flood_data/images/all_images/India_25540.png  
  inflating: flood_data/images/all_images/Mekong_333434.png  
  inflating: flood_data/images/all_images/Spain_5650136.png  
  inflating: flood_data/images/all_images/India_943439.png  
  inflating: flood_data/images/all_images/USA_741178.png  
  inflating: flood_data/images/all_images/Bolivia_294583.png  
  inflating: flood_data/images/all_images/USA_366607.png  
  inflating: flood_data/images/all_images/India_79637.png  
  inflating: flood_data/images/all_images/India_118868.png  
  inflating: flood_data/images/all_images/Paraguay_790830.png  
  inflating: flood_data/images/all_images/USA_527077.png  
  inflating: flood_data/images/all_images/Nigeria_143329.png  
  inflating: flood_data/images/all_images/Sri-Lanka_132922.png  
  inflating: flood_data/images/all_images/Paraguay_172476.png  
  inflating: flood_data/images/all_images/Ghana_167233.png  
  inflating: flood_data/images/all_images/Sri-Lanka_649970.png  
  inflating: flood_data/images/all_images/Sri-Lanka_63307.png  
  inflating: flood_data/images/all_images/USA_788696.png  
  inflating: flood_data/images/all_images/Paraguay_1019808.png  
  inflating: flood_data/images/all_images/Paraguay_605682.png  
  inflating: flood_data/images/all_images/Nigeria_78061.png  
  inflating: flood_data/images/all_images/Ghana_124834.png  
  inflating: flood_data/images/all_images/Paraguay_80102.png  
  inflating: flood_data/images/all_images/Paraguay_482517.png  
  inflating: flood_data/images/all_images/Mekong_293769.png  
  inflating: flood_data/images/all_images/USA_260929.png  
  inflating: flood_data/images/all_images/Spain_6860600.png  
  inflating: flood_data/images/all_images/India_956930.png  
  inflating: flood_data/images/all_images/Nigeria_600295.png  
  inflating: flood_data/images/all_images/Paraguay_1056717.png  
  inflating: flood_data/images/all_images/Nigeria_952958.png  
  inflating: flood_data/images/all_images/Spain_337094.png  
  inflating: flood_data/images/all_images/Spain_7604243.png  
  inflating: flood_data/images/all_images/Ghana_49890.png  
  inflating: flood_data/images/all_images/Bolivia_103757.png  
  inflating: flood_data/images/all_images/Paraguay_252217.png  
  inflating: flood_data/images/all_images/Paraguay_76868.png  
  inflating: flood_data/images/all_images/India_59460.png  
  inflating: flood_data/images/all_images/Paraguay_34417.png  
  inflating: flood_data/images/all_images/Somalia_205466.png  
  inflating: flood_data/images/all_images/Pakistan_246510.png  
  inflating: flood_data/images/all_images/Spain_7558720.png  
  inflating: flood_data/images/all_images/Sri-Lanka_523539.png  
  inflating: flood_data/images/all_images/USA_224165.png  
  inflating: flood_data/images/all_images/Ghana_144050.png  
  inflating: flood_data/images/all_images/India_1068117.png  
  inflating: flood_data/images/all_images/Pakistan_694942.png  
  inflating: flood_data/images/all_images/Spain_3285448.png  
  inflating: flood_data/images/all_images/Ghana_97059.png  
  inflating: flood_data/images/all_images/India_44475.png  
  inflating: flood_data/images/all_images/Sri-Lanka_612594.png  
  inflating: flood_data/images/all_images/Sri-Lanka_450918.png  
  inflating: flood_data/images/all_images/Sri-Lanka_1038087.png  
  inflating: flood_data/images/all_images/Sri-Lanka_236628.png  
  inflating: flood_data/images/all_images/Mekong_382276.png  
  inflating: flood_data/images/all_images/India_399883.png  
  inflating: flood_data/images/all_images/Spain_5923267.png  
  inflating: flood_data/images/all_images/India_73419.png  
  inflating: flood_data/images/all_images/USA_693819.png  
  inflating: flood_data/images/all_images/Nigeria_225131.png  
  inflating: flood_data/images/all_images/Somalia_989553.png  
  inflating: flood_data/images/all_images/Mekong_1439641.png  
  inflating: flood_data/images/all_images/USA_758178.png  
  inflating: flood_data/images/all_images/Paraguay_191503.png  
  inflating: flood_data/images/all_images/USA_66026.png  
  inflating: flood_data/images/all_images/Paraguay_280900.png  
  inflating: flood_data/images/all_images/Paraguay_822142.png  
  inflating: flood_data/images/all_images/USA_387945.png  
  inflating: flood_data/images/all_images/USA_170264.png  
  inflating: flood_data/images/all_images/USA_778194.png  
   creating: flood_data/masks/
   creating: flood_data/masks/all_masks/
  inflating: flood_data/masks/all_masks/Bolivia_312675.png  
  inflating: flood_data/masks/all_masks/Paraguay_1076204.png  
  inflating: flood_data/masks/all_masks/Somalia_12849.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_713926.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_551926.png  
  inflating: flood_data/masks/all_masks/Ghana_156478.png  
  inflating: flood_data/masks/all_masks/Paraguay_36146.png  
 extracting: flood_data/masks/all_masks/India_207862.png  
 extracting: flood_data/masks/all_masks/USA_86502.png  
 extracting: flood_data/masks/all_masks/Spain_4282030.png  
  inflating: flood_data/masks/all_masks/Pakistan_474121.png  
  inflating: flood_data/masks/all_masks/Ghana_103272.png  
 extracting: flood_data/masks/all_masks/Paraguay_581976.png  
  inflating: flood_data/masks/all_masks/Bolivia_360519.png  
  inflating: flood_data/masks/all_masks/India_691027.png  
  inflating: flood_data/masks/all_masks/Mekong_1282475.png  
 extracting: flood_data/masks/all_masks/Mekong_1396181.png  
  inflating: flood_data/masks/all_masks/India_373039.png  
  inflating: flood_data/masks/all_masks/Somalia_626316.png  
  inflating: flood_data/masks/all_masks/Mekong_221789.png  
  inflating: flood_data/masks/all_masks/Somalia_61368.png  
  inflating: flood_data/masks/all_masks/USA_655230.png  
  inflating: flood_data/masks/all_masks/Mekong_119477.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_845821.png  
  inflating: flood_data/masks/all_masks/Mekong_424793.png  
  inflating: flood_data/masks/all_masks/Ghana_247288.png  
  inflating: flood_data/masks/all_masks/USA_181263.png  
  inflating: flood_data/masks/all_masks/India_772630.png  
  inflating: flood_data/masks/all_masks/Paraguay_149787.png  
  inflating: flood_data/masks/all_masks/Bolivia_233925.png  
 extracting: flood_data/masks/all_masks/India_774689.png  
  inflating: flood_data/masks/all_masks/Ghana_597288.png  
  inflating: flood_data/masks/all_masks/Mekong_254910.png  
  inflating: flood_data/masks/all_masks/USA_232060.png  
  inflating: flood_data/masks/all_masks/Paraguay_7894.png  
  inflating: flood_data/masks/all_masks/USA_595451.png  
  inflating: flood_data/masks/all_masks/India_842775.png  
  inflating: flood_data/masks/all_masks/Pakistan_94095.png  
  inflating: flood_data/masks/all_masks/Nigeria_1095404.png  
  inflating: flood_data/masks/all_masks/India_70352.png  
  inflating: flood_data/masks/all_masks/Paraguay_868895.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_135713.png  
  inflating: flood_data/masks/all_masks/Pakistan_548910.png  
  inflating: flood_data/masks/all_masks/India_952728.png  
  inflating: flood_data/masks/all_masks/USA_347609.png  
  inflating: flood_data/masks/all_masks/Somalia_699062.png  
  inflating: flood_data/masks/all_masks/Mekong_98310.png  
 extracting: flood_data/masks/all_masks/India_591549.png  
  inflating: flood_data/masks/all_masks/India_981708.png  
 extracting: flood_data/masks/all_masks/India_285297.png  
  inflating: flood_data/masks/all_masks/USA_231124.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_163406.png  
  inflating: flood_data/masks/all_masks/USA_670826.png  
  inflating: flood_data/masks/all_masks/Mekong_977338.png  
  inflating: flood_data/masks/all_masks/Paraguay_48673.png  
 extracting: flood_data/masks/all_masks/India_773682.png  
  inflating: flood_data/masks/all_masks/Somalia_94102.png  
  inflating: flood_data/masks/all_masks/Pakistan_167553.png  
  inflating: flood_data/masks/all_masks/Spain_7786924.png  
  inflating: flood_data/masks/all_masks/USA_115033.png  
  inflating: flood_data/masks/all_masks/Pakistan_9684.png  
  inflating: flood_data/masks/all_masks/Ghana_61925.png  
  inflating: flood_data/masks/all_masks/Paraguay_896458.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_321316.png  
  inflating: flood_data/masks/all_masks/Paraguay_44682.png  
  inflating: flood_data/masks/all_masks/Mekong_474783.png  
  inflating: flood_data/masks/all_masks/USA_1082482.png  
 extracting: flood_data/masks/all_masks/India_91379.png  
 extracting: flood_data/masks/all_masks/Mekong_1248200.png  
  inflating: flood_data/masks/all_masks/Mekong_1149855.png  
  inflating: flood_data/masks/all_masks/India_166709.png  
  inflating: flood_data/masks/all_masks/Ghana_53713.png  
  inflating: flood_data/masks/all_masks/Spain_8372658.png  
  inflating: flood_data/masks/all_masks/India_287642.png  
  inflating: flood_data/masks/all_masks/Mekong_269835.png  
  inflating: flood_data/masks/all_masks/Spain_5678382.png  
  inflating: flood_data/masks/all_masks/Ghana_168875.png  
  inflating: flood_data/masks/all_masks/USA_114964.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_916628.png  
  inflating: flood_data/masks/all_masks/Spain_1167260.png  
  inflating: flood_data/masks/all_masks/India_80221.png  
  inflating: flood_data/masks/all_masks/USA_664261.png  
  inflating: flood_data/masks/all_masks/USA_519181.png  
  inflating: flood_data/masks/all_masks/Nigeria_31096.png  
  inflating: flood_data/masks/all_masks/Pakistan_35915.png  
 extracting: flood_data/masks/all_masks/USA_770353.png  
  inflating: flood_data/masks/all_masks/USA_638521.png  
  inflating: flood_data/masks/all_masks/Paraguay_403081.png  
  inflating: flood_data/masks/all_masks/Somalia_32375.png  
  inflating: flood_data/masks/all_masks/Bolivia_242570.png  
 extracting: flood_data/masks/all_masks/India_1050276.png  
  inflating: flood_data/masks/all_masks/Nigeria_707067.png  
  inflating: flood_data/masks/all_masks/USA_225017.png  
  inflating: flood_data/masks/all_masks/Somalia_195014.png  
  inflating: flood_data/masks/all_masks/Somalia_167787.png  
  inflating: flood_data/masks/all_masks/Paraguay_721886.png  
  inflating: flood_data/masks/all_masks/India_180633.png  
  inflating: flood_data/masks/all_masks/India_698338.png  
  inflating: flood_data/masks/all_masks/Somalia_992457.png  
  inflating: flood_data/masks/all_masks/India_1018317.png  
  inflating: flood_data/masks/all_masks/Mekong_45934.png  
  inflating: flood_data/masks/all_masks/USA_308150.png  
  inflating: flood_data/masks/all_masks/Pakistan_667363.png  
  inflating: flood_data/masks/all_masks/Paraguay_54421.png  
  inflating: flood_data/masks/all_masks/Paraguay_271769.png  
 extracting: flood_data/masks/all_masks/India_664410.png  
  inflating: flood_data/masks/all_masks/Ghana_24858.png  
 extracting: flood_data/masks/all_masks/India_383430.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_849649.png  
  inflating: flood_data/masks/all_masks/Spain_6199994.png  
  inflating: flood_data/masks/all_masks/Somalia_7931.png  
  inflating: flood_data/masks/all_masks/USA_348639.png  
  inflating: flood_data/masks/all_masks/Mekong_846007.png  
  inflating: flood_data/masks/all_masks/Paraguay_62897.png  
  inflating: flood_data/masks/all_masks/Spain_2594119.png  
  inflating: flood_data/masks/all_masks/USA_1049586.png  
  inflating: flood_data/masks/all_masks/Ghana_8090.png  
 extracting: flood_data/masks/all_masks/Ghana_868803.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_236030.png  
 extracting: flood_data/masks/all_masks/India_570384.png  
  inflating: flood_data/masks/all_masks/Ghana_359826.png  
  inflating: flood_data/masks/all_masks/Ghana_146222.png  
  inflating: flood_data/masks/all_masks/Pakistan_211386.png  
  inflating: flood_data/masks/all_masks/USA_646878.png  
  inflating: flood_data/masks/all_masks/India_631692.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_883641.png  
 extracting: flood_data/masks/all_masks/Nigeria_984831.png  
  inflating: flood_data/masks/all_masks/Spain_6537196.png  
  inflating: flood_data/masks/all_masks/Paraguay_934240.png  
  inflating: flood_data/masks/all_masks/Paraguay_40936.png  
  inflating: flood_data/masks/all_masks/Bolivia_23014.png  
 extracting: flood_data/masks/all_masks/Pakistan_849790.png  
  inflating: flood_data/masks/all_masks/Pakistan_664885.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_52223.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_49764.png  
  inflating: flood_data/masks/all_masks/USA_986268.png  
  inflating: flood_data/masks/all_masks/Mekong_342411.png  
  inflating: flood_data/masks/all_masks/Spain_5816638.png  
  inflating: flood_data/masks/all_masks/Mekong_16233.png  
 extracting: flood_data/masks/all_masks/India_652725.png  
  inflating: flood_data/masks/all_masks/Paraguay_246154.png  
  inflating: flood_data/masks/all_masks/Mekong_1413877.png  
  inflating: flood_data/masks/all_masks/Nigeria_820924.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_152185.png  
  inflating: flood_data/masks/all_masks/India_103447.png  
  inflating: flood_data/masks/all_masks/Spain_8565131.png  
  inflating: flood_data/masks/all_masks/USA_504150.png  
  inflating: flood_data/masks/all_masks/Paraguay_247656.png  
  inflating: flood_data/masks/all_masks/Paraguay_791364.png  
 extracting: flood_data/masks/all_masks/Paraguay_339807.png  
  inflating: flood_data/masks/all_masks/Paraguay_913449.png  
  inflating: flood_data/masks/all_masks/Paraguay_198534.png  
  inflating: flood_data/masks/all_masks/Nigeria_35845.png  
  inflating: flood_data/masks/all_masks/Spain_6095801.png  
  inflating: flood_data/masks/all_masks/USA_994009.png  
  inflating: flood_data/masks/all_masks/Somalia_371421.png  
 extracting: flood_data/masks/all_masks/India_500266.png  
  inflating: flood_data/masks/all_masks/Somalia_60129.png  
  inflating: flood_data/masks/all_masks/Paraguay_24341.png  
  inflating: flood_data/masks/all_masks/Nigeria_417184.png  
  inflating: flood_data/masks/all_masks/Bolivia_76104.png  
  inflating: flood_data/masks/all_masks/Pakistan_43105.png  
  inflating: flood_data/masks/all_masks/Paraguay_212687.png  
  inflating: flood_data/masks/all_masks/Mekong_1395593.png  
  inflating: flood_data/masks/all_masks/USA_58086.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_400518.png  
 extracting: flood_data/masks/all_masks/USA_955053.png  
  inflating: flood_data/masks/all_masks/Ghana_134751.png  
 extracting: flood_data/masks/all_masks/India_1017769.png  
 extracting: flood_data/masks/all_masks/Mekong_774566.png  
  inflating: flood_data/masks/all_masks/USA_84195.png  
  inflating: flood_data/masks/all_masks/USA_375183.png  
  inflating: flood_data/masks/all_masks/Spain_2523247.png  
  inflating: flood_data/masks/all_masks/Mekong_213094.png  
  inflating: flood_data/masks/all_masks/India_828067.png  
  inflating: flood_data/masks/all_masks/Ghana_5079.png  
  inflating: flood_data/masks/all_masks/USA_905409.png  
 extracting: flood_data/masks/all_masks/Bolivia_379434.png  
  inflating: flood_data/masks/all_masks/USA_831672.png  
  inflating: flood_data/masks/all_masks/Bolivia_195474.png  
  inflating: flood_data/masks/all_masks/Paraguay_511199.png  
  inflating: flood_data/masks/all_masks/Somalia_256539.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_748447.png  
  inflating: flood_data/masks/all_masks/Pakistan_1036366.png  
  inflating: flood_data/masks/all_masks/Paraguay_12870.png  
  inflating: flood_data/masks/all_masks/Paraguay_683296.png  
  inflating: flood_data/masks/all_masks/India_164336.png  
  inflating: flood_data/masks/all_masks/Ghana_83200.png  
  inflating: flood_data/masks/all_masks/Paraguay_1029042.png  
 extracting: flood_data/masks/all_masks/Bolivia_129334.png  
  inflating: flood_data/masks/all_masks/Spain_1199913.png  
  inflating: flood_data/masks/all_masks/Mekong_1443339.png  
  inflating: flood_data/masks/all_masks/USA_19225.png  
  inflating: flood_data/masks/all_masks/Somalia_166342.png  
  inflating: flood_data/masks/all_masks/USA_66511.png  
  inflating: flood_data/masks/all_masks/Spain_4915752.png  
  inflating: flood_data/masks/all_masks/Ghana_142312.png  
  inflating: flood_data/masks/all_masks/Bolivia_290290.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_117737.png  
  inflating: flood_data/masks/all_masks/Pakistan_1027214.png  
  inflating: flood_data/masks/all_masks/India_534470.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_534068.png  
  inflating: flood_data/masks/all_masks/Ghana_154838.png  
  inflating: flood_data/masks/all_masks/Spain_8104659.png  
  inflating: flood_data/masks/all_masks/USA_761032.png  
  inflating: flood_data/masks/all_masks/Nigeria_598959.png  
  inflating: flood_data/masks/all_masks/India_869358.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_85652.png  
  inflating: flood_data/masks/all_masks/Paraguay_232281.png  
  inflating: flood_data/masks/all_masks/Paraguay_892933.png  
  inflating: flood_data/masks/all_masks/Paraguay_792268.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_653336.png  
  inflating: flood_data/masks/all_masks/India_533192.png  
 extracting: flood_data/masks/all_masks/India_566697.png  
  inflating: flood_data/masks/all_masks/Ghana_135389.png  
  inflating: flood_data/masks/all_masks/Ghana_141910.png  
  inflating: flood_data/masks/all_masks/Somalia_322855.png  
  inflating: flood_data/masks/all_masks/Ghana_141271.png  
  inflating: flood_data/masks/all_masks/Ghana_132163.png  
  inflating: flood_data/masks/all_masks/USA_933610.png  
  inflating: flood_data/masks/all_masks/Ghana_161233.png  
  inflating: flood_data/masks/all_masks/India_591317.png  
  inflating: flood_data/masks/all_masks/USA_741073.png  
  inflating: flood_data/masks/all_masks/Spain_2472849.png  
 extracting: flood_data/masks/all_masks/Paraguay_305760.png  
  inflating: flood_data/masks/all_masks/Ghana_313799.png  
  inflating: flood_data/masks/all_masks/India_136196.png  
 extracting: flood_data/masks/all_masks/India_1072277.png  
  inflating: flood_data/masks/all_masks/USA_438959.png  
  inflating: flood_data/masks/all_masks/USA_486103.png  
  inflating: flood_data/masks/all_masks/Ghana_277.png  
 extracting: flood_data/masks/all_masks/Mekong_52610.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_55568.png  
  inflating: flood_data/masks/all_masks/India_979278.png  
  inflating: flood_data/masks/all_masks/Pakistan_70625.png  
  inflating: flood_data/masks/all_masks/Paraguay_215904.png  
  inflating: flood_data/masks/all_masks/Paraguay_997480.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_101973.png  
  inflating: flood_data/masks/all_masks/India_747970.png  
  inflating: flood_data/masks/all_masks/Somalia_93023.png  
  inflating: flood_data/masks/all_masks/Mekong_1191208.png  
  inflating: flood_data/masks/all_masks/Paraguay_179624.png  
  inflating: flood_data/masks/all_masks/Pakistan_712873.png  
  inflating: flood_data/masks/all_masks/Somalia_685158.png  
 extracting: flood_data/masks/all_masks/Mekong_596495.png  
  inflating: flood_data/masks/all_masks/Somalia_230192.png  
  inflating: flood_data/masks/all_masks/Spain_716716.png  
  inflating: flood_data/masks/all_masks/USA_354981.png  
  inflating: flood_data/masks/all_masks/Pakistan_366265.png  
  inflating: flood_data/masks/all_masks/Pakistan_246718.png  
  inflating: flood_data/masks/all_masks/Somalia_295782.png  
  inflating: flood_data/masks/all_masks/India_769408.png  
  inflating: flood_data/masks/all_masks/Ghana_362274.png  
  inflating: flood_data/masks/all_masks/Paraguay_648632.png  
  inflating: flood_data/masks/all_masks/USA_211406.png  
 extracting: flood_data/masks/all_masks/Spain_7387658.png  
  inflating: flood_data/masks/all_masks/Paraguay_657443.png  
  inflating: flood_data/masks/all_masks/Ghana_26376.png  
  inflating: flood_data/masks/all_masks/Spain_8154154.png  
  inflating: flood_data/masks/all_masks/Somalia_1068756.png  
 extracting: flood_data/masks/all_masks/Nigeria_81933.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_14484.png  
  inflating: flood_data/masks/all_masks/Pakistan_65724.png  
  inflating: flood_data/masks/all_masks/Nigeria_439488.png  
 extracting: flood_data/masks/all_masks/Mekong_1111068.png  
  inflating: flood_data/masks/all_masks/USA_826217.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_847275.png  
  inflating: flood_data/masks/all_masks/Ghana_895194.png  
  inflating: flood_data/masks/all_masks/Paraguay_148318.png  
  inflating: flood_data/masks/all_masks/Paraguay_59731.png  
  inflating: flood_data/masks/all_masks/Spain_8199661.png  
  inflating: flood_data/masks/all_masks/USA_1068362.png  
  inflating: flood_data/masks/all_masks/Spain_2938657.png  
  inflating: flood_data/masks/all_masks/USA_806273.png  
  inflating: flood_data/masks/all_masks/USA_11422.png  
  inflating: flood_data/masks/all_masks/Paraguay_224845.png  
  inflating: flood_data/masks/all_masks/India_592446.png  
  inflating: flood_data/masks/all_masks/Ghana_45911.png  
  inflating: flood_data/masks/all_masks/Pakistan_760290.png  
  inflating: flood_data/masks/all_masks/Nigeria_812045.png  
 extracting: flood_data/masks/all_masks/India_179238.png  
  inflating: flood_data/masks/all_masks/India_273873.png  
  inflating: flood_data/masks/all_masks/Pakistan_336228.png  
 extracting: flood_data/masks/all_masks/India_900498.png  
  inflating: flood_data/masks/all_masks/Paraguay_11869.png  
 extracting: flood_data/masks/all_masks/Somalia_970508.png  
  inflating: flood_data/masks/all_masks/Nigeria_22088.png  
  inflating: flood_data/masks/all_masks/Bolivia_432776.png  
  inflating: flood_data/masks/all_masks/Paraguay_225187.png  
  inflating: flood_data/masks/all_masks/Paraguay_205585.png  
  inflating: flood_data/masks/all_masks/Somalia_1087508.png  
  inflating: flood_data/masks/all_masks/India_391908.png  
  inflating: flood_data/masks/all_masks/USA_605492.png  
  inflating: flood_data/masks/all_masks/Paraguay_149830.png  
  inflating: flood_data/masks/all_masks/USA_275372.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_377277.png  
  inflating: flood_data/masks/all_masks/Paraguay_651904.png  
  inflating: flood_data/masks/all_masks/USA_1039203.png  
  inflating: flood_data/masks/all_masks/Nigeria_529525.png  
 extracting: flood_data/masks/all_masks/Somalia_886726.png  
  inflating: flood_data/masks/all_masks/USA_1010394.png  
  inflating: flood_data/masks/all_masks/Ghana_97516.png  
  inflating: flood_data/masks/all_masks/USA_179917.png  
 extracting: flood_data/masks/all_masks/Paraguay_126224.png  
  inflating: flood_data/masks/all_masks/Paraguay_284928.png  
  inflating: flood_data/masks/all_masks/Ghana_187318.png  
  inflating: flood_data/masks/all_masks/USA_181503.png  
  inflating: flood_data/masks/all_masks/Pakistan_909806.png  
 extracting: flood_data/masks/all_masks/India_747992.png  
 extracting: flood_data/masks/all_masks/Mekong_922373.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_922192.png  
  inflating: flood_data/masks/all_masks/Paraguay_795075.png  
  inflating: flood_data/masks/all_masks/India_244057.png  
  inflating: flood_data/masks/all_masks/Paraguay_470303.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_92824.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_1049830.png  
 extracting: flood_data/masks/all_masks/India_1018327.png  
  inflating: flood_data/masks/all_masks/Ghana_319168.png  
  inflating: flood_data/masks/all_masks/Ghana_887131.png  
  inflating: flood_data/masks/all_masks/USA_350244.png  
  inflating: flood_data/masks/all_masks/India_177319.png  
  inflating: flood_data/masks/all_masks/Paraguay_1029191.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_249079.png  
  inflating: flood_data/masks/all_masks/India_265762.png  
  inflating: flood_data/masks/all_masks/Paraguay_153941.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_120804.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_178753.png  
  inflating: flood_data/masks/all_masks/Ghana_147015.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_579082.png  
  inflating: flood_data/masks/all_masks/Ghana_1033830.png  
 extracting: flood_data/masks/all_masks/Bolivia_314919.png  
  inflating: flood_data/masks/all_masks/Ghana_264787.png  
 extracting: flood_data/masks/all_masks/Spain_7370579.png  
 extracting: flood_data/masks/all_masks/India_833266.png  
  inflating: flood_data/masks/all_masks/USA_430764.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_956740.png  
  inflating: flood_data/masks/all_masks/Spain_7856615.png  
  inflating: flood_data/masks/all_masks/Ghana_406026.png  
 extracting: flood_data/masks/all_masks/India_804466.png  
  inflating: flood_data/masks/all_masks/Ghana_11745.png  
  inflating: flood_data/masks/all_masks/Pakistan_401863.png  
  inflating: flood_data/masks/all_masks/USA_198411.png  
  inflating: flood_data/masks/all_masks/Pakistan_740461.png  
  inflating: flood_data/masks/all_masks/Pakistan_210595.png  
  inflating: flood_data/masks/all_masks/Ghana_953791.png  
  inflating: flood_data/masks/all_masks/USA_67102.png  
  inflating: flood_data/masks/all_masks/India_764946.png  
  inflating: flood_data/masks/all_masks/Ghana_234935.png  
  inflating: flood_data/masks/all_masks/Somalia_649376.png  
  inflating: flood_data/masks/all_masks/Ghana_128663.png  
  inflating: flood_data/masks/all_masks/Bolivia_60373.png  
  inflating: flood_data/masks/all_masks/Ghana_308249.png  
  inflating: flood_data/masks/all_masks/USA_604222.png  
  inflating: flood_data/masks/all_masks/USA_652955.png  
  inflating: flood_data/masks/all_masks/Paraguay_36015.png  
  inflating: flood_data/masks/all_masks/Pakistan_132143.png  
  inflating: flood_data/masks/all_masks/Ghana_194723.png  
  inflating: flood_data/masks/all_masks/Ghana_495107.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_233609.png  
  inflating: flood_data/masks/all_masks/India_324254.png  
  inflating: flood_data/masks/all_masks/India_624341.png  
  inflating: flood_data/masks/all_masks/India_56450.png  
  inflating: flood_data/masks/all_masks/Ghana_7496.png  
  inflating: flood_data/masks/all_masks/USA_908474.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_31559.png  
  inflating: flood_data/masks/all_masks/Ghana_83483.png  
  inflating: flood_data/masks/all_masks/USA_251323.png  
  inflating: flood_data/masks/all_masks/India_135434.png  
  inflating: flood_data/masks/all_masks/India_707886.png  
  inflating: flood_data/masks/all_masks/USA_217598.png  
  inflating: flood_data/masks/all_masks/Paraguay_921838.png  
  inflating: flood_data/masks/all_masks/Ghana_866994.png  
  inflating: flood_data/masks/all_masks/Ghana_1089161.png  
  inflating: flood_data/masks/all_masks/Pakistan_528249.png  
  inflating: flood_data/masks/all_masks/Ghana_1078550.png  
  inflating: flood_data/masks/all_masks/Paraguay_989230.png  
  inflating: flood_data/masks/all_masks/India_25540.png  
  inflating: flood_data/masks/all_masks/Mekong_333434.png  
  inflating: flood_data/masks/all_masks/Spain_5650136.png  
 extracting: flood_data/masks/all_masks/India_943439.png  
  inflating: flood_data/masks/all_masks/USA_741178.png  
  inflating: flood_data/masks/all_masks/Bolivia_294583.png  
  inflating: flood_data/masks/all_masks/USA_366607.png  
  inflating: flood_data/masks/all_masks/India_79637.png  
  inflating: flood_data/masks/all_masks/India_118868.png  
  inflating: flood_data/masks/all_masks/Paraguay_790830.png  
  inflating: flood_data/masks/all_masks/USA_527077.png  
  inflating: flood_data/masks/all_masks/Nigeria_143329.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_132922.png  
  inflating: flood_data/masks/all_masks/Paraguay_172476.png  
  inflating: flood_data/masks/all_masks/Ghana_167233.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_649970.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_63307.png  
  inflating: flood_data/masks/all_masks/USA_788696.png  
  inflating: flood_data/masks/all_masks/Paraguay_1019808.png  
 extracting: flood_data/masks/all_masks/Paraguay_605682.png  
  inflating: flood_data/masks/all_masks/Nigeria_78061.png  
  inflating: flood_data/masks/all_masks/Ghana_124834.png  
  inflating: flood_data/masks/all_masks/Paraguay_80102.png  
  inflating: flood_data/masks/all_masks/Paraguay_482517.png  
  inflating: flood_data/masks/all_masks/Mekong_293769.png  
  inflating: flood_data/masks/all_masks/USA_260929.png  
  inflating: flood_data/masks/all_masks/Spain_6860600.png  
 extracting: flood_data/masks/all_masks/India_956930.png  
  inflating: flood_data/masks/all_masks/Nigeria_600295.png  
  inflating: flood_data/masks/all_masks/Paraguay_1056717.png  
  inflating: flood_data/masks/all_masks/Nigeria_952958.png  
  inflating: flood_data/masks/all_masks/Spain_337094.png  
  inflating: flood_data/masks/all_masks/Spain_7604243.png  
  inflating: flood_data/masks/all_masks/Ghana_49890.png  
  inflating: flood_data/masks/all_masks/Bolivia_103757.png  
  inflating: flood_data/masks/all_masks/Paraguay_252217.png  
  inflating: flood_data/masks/all_masks/Paraguay_76868.png  
  inflating: flood_data/masks/all_masks/India_59460.png  
  inflating: flood_data/masks/all_masks/Paraguay_34417.png  
  inflating: flood_data/masks/all_masks/Somalia_205466.png  
  inflating: flood_data/masks/all_masks/Pakistan_246510.png  
  inflating: flood_data/masks/all_masks/Spain_7558720.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_523539.png  
  inflating: flood_data/masks/all_masks/USA_224165.png  
  inflating: flood_data/masks/all_masks/Ghana_144050.png  
 extracting: flood_data/masks/all_masks/India_1068117.png  
  inflating: flood_data/masks/all_masks/Pakistan_694942.png  
  inflating: flood_data/masks/all_masks/Spain_3285448.png  
  inflating: flood_data/masks/all_masks/Ghana_97059.png  
  inflating: flood_data/masks/all_masks/India_44475.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_612594.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_450918.png  
 extracting: flood_data/masks/all_masks/Sri-Lanka_1038087.png  
  inflating: flood_data/masks/all_masks/Sri-Lanka_236628.png  
  inflating: flood_data/masks/all_masks/Mekong_382276.png  
 extracting: flood_data/masks/all_masks/India_399883.png  
  inflating: flood_data/masks/all_masks/Spain_5923267.png  
  inflating: flood_data/masks/all_masks/India_73419.png  
  inflating: flood_data/masks/all_masks/USA_693819.png  
  inflating: flood_data/masks/all_masks/Nigeria_225131.png  
  inflating: flood_data/masks/all_masks/Somalia_989553.png  
  inflating: flood_data/masks/all_masks/Mekong_1439641.png  
  inflating: flood_data/masks/all_masks/USA_758178.png  
  inflating: flood_data/masks/all_masks/Paraguay_191503.png  
  inflating: flood_data/masks/all_masks/USA_66026.png  
  inflating: flood_data/masks/all_masks/Paraguay_280900.png  
 extracting: flood_data/masks/all_masks/Paraguay_822142.png  
  inflating: flood_data/masks/all_masks/USA_387945.png  
  inflating: flood_data/masks/all_masks/USA_170264.png  
  inflating: flood_data/masks/all_masks/USA_778194.png  
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 0.2</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># set environment variables</span>
<span class="kn">import</span> <span class="nn">os</span>

<span class="o">%</span><span class="k">set_env</span> LOCAL_PROJECT_DIR=/dli/task/tao_project
<span class="o">%</span><span class="k">set_env</span> LOCAL_DATA_DIR=/dli/task/flood_data

<span class="n">os</span><span class="o">.</span><span class="n">environ</span><span class="p">[</span><span class="s2">&quot;LOCAL_EXPERIMENT_DIR&quot;</span><span class="p">]</span><span class="o">=</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s2">&quot;LOCAL_PROJECT_DIR&quot;</span><span class="p">),</span> <span class="s2">&quot;unet&quot;</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>env: LOCAL_PROJECT_DIR=/dli/task/tao_project
env: LOCAL_DATA_DIR=/dli/task/flood_data
</pre>
</div>
</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Step-1:-Set-Up-Triton-Inference-Server">Step 1: Set Up Triton Inference Server<a class="anchor-link" href="#Step-1:-Set-Up-Triton-Inference-Server">&#182;</a></h3><p>Next, we will prepare Triton Inference Server. Triton Inference Server has been placed in polling mode. It will serve models within a model repository, which is mounted to the local <code>models</code> directory. Below is an example structure of the model repository that contains the segmentation model. For more details on how to work with model repositories and model directory structures in Triton Inference Server, please see the <a href="https://github.com/triton-inference-server/server/blob/r20.12/docs/model_repository.md">documentation</a>.</p>
<pre><code>root@server:/models$ tree
.
├── flood_segmentation_model
│   ├── 1
│   │   └── model.plan
│   └── config.pbtxt
</code></pre>
<p><strong>Instructions</strong>: <br>
2.1 Execute the below cell to set up a directory in the model repository and copy the TensorRT engine into the newly created directory. <br>
2.2 Execute the cell below to create the configuration file for the <code>flood_segmentation_model</code>. <br>
2.3 Execute the cell below to check the model repository folder structure. <br>
2.4 Execute the cell below to check the status of the <code>flood_segmentation_model</code> using the <code>curl</code> command.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 2.1</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># create directory for model</span>
<span class="o">!</span>mkdir -p models/flood_segmentation_model/1

<span class="c1"># copy sample_resnet18.engine from previous notebook to the model repository</span>
<span class="o">!</span>cp <span class="nv">$LOCAL_EXPERIMENT_DIR</span>/export/sample_resnet18.engine models/flood_segmentation_model/1/model.plan
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 2.2</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="n">configuration</span> <span class="o">=</span> <span class="s2">&quot;&quot;&quot;</span>
<span class="s2">name: &quot;flood_segmentation_model&quot;</span>
<span class="s2">platform: &quot;tensorrt_plan&quot;</span>
<span class="s2">max_batch_size: 1</span>
<span class="s2">input: [</span>
<span class="s2"> {</span>
<span class="s2">    name: &quot;input_1&quot;</span>
<span class="s2">    data_type: TYPE_FP32</span>
<span class="s2">    format: FORMAT_NCHW</span>
<span class="s2">    dims: [ 3, 512, 512 ]</span>
<span class="s2">  }</span>
<span class="s2">]</span>
<span class="s2">output: {</span>
<span class="s2">    name: &quot;softmax_1&quot;</span>
<span class="s2">    data_type: TYPE_FP32</span>
<span class="s2">    dims: [ 512, 512, 2 ]</span>
<span class="s2">  }</span>
<span class="s2">&quot;&quot;&quot;</span>

<span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="s1">&#39;models/flood_segmentation_model/config.pbtxt&#39;</span><span class="p">,</span> <span class="s1">&#39;w&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
    <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="n">configuration</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 2.3</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># show model repository folder structure</span>
<span class="o">!</span>tree -a models
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre><span class="ansi-blue-intense-fg ansi-bold">models</span>
└── <span class="ansi-blue-intense-fg ansi-bold">flood_segmentation_model</span>
    ├── <span class="ansi-blue-intense-fg ansi-bold">1</span>
    │   └── model.plan
    └── config.pbtxt

2 directories, 2 files
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 2.4</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="o">!</span>sleep <span class="m">45</span>

<span class="c1"># check model status</span>
<span class="o">!</span>curl -v triton:8000/v2/models/flood_segmentation_model
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>*   Trying 172.18.0.5:8000...
* TCP_NODELAY set
* Connected to triton (172.18.0.5) port 8000 (#0)
&gt; GET /v2/models/flood_segmentation_model HTTP/1.1
&gt; Host: triton:8000
&gt; User-Agent: curl/7.68.0
&gt; Accept: */*
&gt; 
* Mark bundle as not supporting multiuse
&lt; HTTP/1.1 200 OK
&lt; Content-Type: application/json
&lt; Content-Length: 224
&lt; 
* Connection #0 to host triton left intact
{&#34;name&#34;:&#34;flood_segmentation_model&#34;,&#34;versions&#34;:[&#34;1&#34;],&#34;platform&#34;:&#34;tensorrt_plan&#34;,&#34;inputs&#34;:[{&#34;name&#34;:&#34;input_1&#34;,&#34;datatype&#34;:&#34;FP32&#34;,&#34;shape&#34;:[-1,3,512,512]}],&#34;outputs&#34;:[{&#34;name&#34;:&#34;softmax_1&#34;,&#34;datatype&#34;:&#34;FP32&#34;,&#34;shape&#34;:[-1,512,512,2]}]}</pre>
</div>
</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Step-3:-Send-Inference-Request-to-Server">Step 3: Send Inference Request to Server<a class="anchor-link" href="#Step-3:-Send-Inference-Request-to-Server">&#182;</a></h3><p>The next step is to generate flood mask predictions. With our models deployed, it is now time to send inference requests to our models served on the Triton Inference Server. Triton Inference Server itself does not do anything with your input tensors, it simply feeds them to the model. Same for outputs. Ensuring that the pre-processing operations used for inference are defined identically as they were when the model was trained is key to achieving high accuracy. When we developed the segmentation model, some data pre-processing were done for training. Therefore, we need to perform the same normalization and mean subtraction to produce the final float planar data that the TensorRT engine is looking for. The pre-processing function is:</p>
<p><b>y = net scale factor * (x-mean)</b></p>
<p>where:</p>
<ul>
<li><strong>x</strong> is the input pixel value. It is an int8 with range [0,255].</li>
<li><strong>mean</strong> is <code>127.5</code> for all 3 RGB channels.</li>
<li><strong>net-scale-factor</strong> is <code>1/127.5</code>, or <code>0.00784313725490196</code>.</li>
<li><strong>y</strong> is the corresponding output pixel value. It is a float.</li>
</ul>
<p><strong>Instructions</strong>: <br>
3.1 Execute the below cell to load dependencies, set parameters, and instantiate a Triton Client to communicate with the Triton Inference Server at <code>triton:8000</code>. <br>
3.2 Modify the <code>&lt;FIXME&gt;</code>s only and execute the cell below to define the <code>preprocessing_image</code> function. <br>
3.3 Execute the cell below to instantiate a placeholder for our input data and output. <br>
3.4 Modify the <code>&lt;FIXME&gt;</code>s only to iteratively pre-process input images, send inference requests, and post-process the inference results for the entire dataset. We will save the mask images. <br>
3.5 Execute the cell below to preview a sample.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 3.1</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="kn">import</span> <span class="nn">tritonclient.http</span> <span class="k">as</span> <span class="nn">tritonhttpclient</span>
<span class="kn">import</span> <span class="nn">random</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">from</span> <span class="nn">PIL</span> <span class="kn">import</span> <span class="n">Image</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">warnings</span>
<span class="n">warnings</span><span class="o">.</span><span class="n">filterwarnings</span><span class="p">(</span><span class="s2">&quot;ignore&quot;</span><span class="p">)</span>

<span class="c1"># set parameters</span>
<span class="n">VERBOSE</span><span class="o">=</span><span class="kc">False</span>
<span class="n">input_name</span><span class="o">=</span><span class="s1">&#39;input_1&#39;</span>
<span class="n">input_shape</span><span class="o">=</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="mi">512</span><span class="p">,</span> <span class="mi">512</span><span class="p">)</span>
<span class="n">input_dtype</span><span class="o">=</span><span class="s1">&#39;FP32&#39;</span>
<span class="n">output_name</span><span class="o">=</span><span class="s1">&#39;softmax_1&#39;</span>
<span class="n">model_name</span><span class="o">=</span><span class="s1">&#39;flood_segmentation_model&#39;</span>
<span class="n">url</span><span class="o">=</span><span class="s1">&#39;triton:8000&#39;</span>
<span class="n">model_version</span><span class="o">=</span><span class="s1">&#39;1&#39;</span>

<span class="n">triton_client</span><span class="o">=</span><span class="n">tritonhttpclient</span><span class="o">.</span><span class="n">InferenceServerClient</span><span class="p">(</span><span class="n">url</span><span class="o">=</span><span class="n">url</span><span class="p">,</span> <span class="n">verbose</span><span class="o">=</span><span class="n">VERBOSE</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 3.2</span>
<span class="c1"># define pre-process function</span>
<span class="k">def</span> <span class="nf">preprocess_image</span><span class="p">(</span><span class="n">image</span><span class="p">):</span> 
    <span class="sd">&quot;&quot;&quot;</span>
<span class="sd">    This function returns the pre-processed image as a NumPy array. </span>
<span class="sd">    &quot;&quot;&quot;</span>
    <span class="c1"># load image as a 32-bit floating point array </span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">asarray</span><span class="p">(</span><span class="n">image</span><span class="p">)</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">image_ary</span><span class="o">.</span><span class="n">astype</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">float32</span><span class="p">)</span>
        
    <span class="c1"># pre-processing</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="p">(</span><span class="n">image_ary</span><span class="o">-</span><span class="mf">127.5</span><span class="p">)</span><span class="o">*</span><span class="mf">0.00784313725490196</span>
    
    <span class="c1"># the sample_resnet18 segmentation model requires the data to be in BGR format</span>
    <span class="n">BGR</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">empty_like</span><span class="p">(</span><span class="n">image_ary</span><span class="p">)</span>
    <span class="n">BGR</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">0</span><span class="p">]</span><span class="o">=</span><span class="n">image_ary</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">2</span><span class="p">]</span>
    <span class="n">BGR</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">1</span><span class="p">]</span><span class="o">=</span><span class="n">image_ary</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">1</span><span class="p">]</span>
    <span class="n">BGR</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">2</span><span class="p">]</span><span class="o">=</span><span class="n">image_ary</span><span class="p">[:,</span> <span class="p">:,</span> <span class="mi">0</span><span class="p">]</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">BGR</span>
    
    <span class="c1"># convert array from h, w, c to 1, c, h, w</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">transpose</span><span class="p">(</span><span class="n">image_ary</span><span class="p">,</span> <span class="p">[</span><span class="mi">2</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">])</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">expand_dims</span><span class="p">(</span><span class="n">image_ary</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">0</span><span class="p">)</span>
    <span class="k">return</span> <span class="n">image_ary</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[9]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 3.3</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># set inference input and output configurations</span>
<span class="n">inference_input</span><span class="o">=</span><span class="n">tritonhttpclient</span><span class="o">.</span><span class="n">InferInput</span><span class="p">(</span><span class="n">input_name</span><span class="p">,</span> <span class="n">input_shape</span><span class="p">,</span> <span class="n">input_dtype</span><span class="p">)</span>
<span class="n">output</span><span class="o">=</span><span class="n">tritonhttpclient</span><span class="o">.</span><span class="n">InferRequestedOutput</span><span class="p">(</span><span class="n">output_name</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[10]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 3.4</span>
<span class="c1"># remove previous inference results if exists</span>
<span class="o">!</span>rm -rf inference_results
<span class="o">!</span>mkdir inference_results

<span class="n">image_dir</span><span class="o">=</span><span class="n">os</span><span class="o">.</span><span class="n">listdir</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;LOCAL_DATA_DIR&#39;</span><span class="p">),</span> <span class="s1">&#39;images&#39;</span><span class="p">,</span> <span class="s1">&#39;all_images&#39;</span><span class="p">))</span>

<span class="c1"># iterate through all images</span>
<span class="k">for</span> <span class="n">idx</span><span class="p">,</span> <span class="n">image_path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">image_dir</span><span class="p">):</span> 
    <span class="n">image</span><span class="o">=</span><span class="n">Image</span><span class="o">.</span><span class="n">open</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;LOCAL_DATA_DIR&#39;</span><span class="p">),</span> <span class="s1">&#39;images&#39;</span><span class="p">,</span> <span class="s1">&#39;all_images&#39;</span><span class="p">,</span> <span class="n">image_path</span><span class="p">))</span>
    
    <span class="c1"># pre-process image</span>
    <span class="n">image_ary</span><span class="o">=</span><span class="n">preprocess_image</span><span class="p">(</span><span class="n">image</span><span class="p">)</span>
    
    <span class="c1"># send image_ary for inference</span>
    <span class="n">inference_input</span><span class="o">.</span><span class="n">set_data_from_numpy</span><span class="p">(</span><span class="n">image_ary</span><span class="p">)</span>
    <span class="n">response</span><span class="o">=</span><span class="n">triton_client</span><span class="o">.</span><span class="n">infer</span><span class="p">(</span><span class="n">model_name</span><span class="p">,</span> 
                                 <span class="n">model_version</span><span class="o">=</span><span class="n">model_version</span><span class="p">,</span> 
                                 <span class="n">inputs</span><span class="o">=</span><span class="p">[</span><span class="n">inference_input</span><span class="p">],</span> 
                                 <span class="n">outputs</span><span class="o">=</span><span class="p">[</span><span class="n">output</span><span class="p">])</span>
    <span class="n">logits</span><span class="o">=</span><span class="n">response</span><span class="o">.</span><span class="n">as_numpy</span><span class="p">(</span><span class="n">output_name</span><span class="p">)</span>
    
    <span class="c1"># post-processing and create mask image from inference output</span>
    <span class="n">mask</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">argmax</span><span class="p">(</span><span class="n">logits</span><span class="p">,</span> <span class="n">axis</span><span class="o">=</span><span class="mi">3</span><span class="p">)[</span><span class="mi">0</span><span class="p">]</span>
    
    <span class="c1"># save mask image</span>
    <span class="n">mask_img</span><span class="o">=</span><span class="n">Image</span><span class="o">.</span><span class="n">fromarray</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">uint8</span><span class="p">(</span><span class="n">mask</span><span class="p">))</span>
    <span class="n">mask_img</span><span class="o">.</span><span class="n">save</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">,</span> <span class="n">image_path</span><span class="p">))</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[11]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 3.5</span>
<span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="c1"># select random sample</span>
<span class="n">random_choice</span><span class="o">=</span><span class="n">random</span><span class="o">.</span><span class="n">choice</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">listdir</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">))</span>

<span class="c1"># plot input, triton inference, and ground truth</span>
<span class="n">fig</span><span class="p">,</span> <span class="n">ax</span><span class="o">=</span><span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">3</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">[</span><span class="mi">20</span><span class="p">,</span> <span class="mi">5</span><span class="p">],</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">sharey</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">imshow</span><span class="p">(</span><span class="n">plt</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;LOCAL_DATA_DIR&#39;</span><span class="p">),</span> <span class="s1">&#39;images&#39;</span><span class="p">,</span> <span class="s1">&#39;all_images&#39;</span><span class="p">,</span> <span class="n">random_choice</span><span class="p">)))</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">imshow</span><span class="p">(</span><span class="n">plt</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">,</span> <span class="n">random_choice</span><span class="p">)))</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">imshow</span><span class="p">(</span><span class="n">plt</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;LOCAL_DATA_DIR&#39;</span><span class="p">),</span> <span class="s1">&#39;masks&#39;</span><span class="p">,</span> <span class="s1">&#39;all_masks&#39;</span><span class="p">,</span> <span class="n">random_choice</span><span class="p">)))</span>

<span class="c1"># set title</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s1">&#39;Input Image&#39;</span><span class="p">)</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s1">&#39;Triton Inference&#39;</span><span class="p">)</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s1">&#39;Ground Truth&#39;</span><span class="p">)</span>

<span class="c1"># remove ticks</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_xticks</span><span class="p">([])</span>
<span class="n">ax</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_yticks</span><span class="p">([])</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Sample: </span><span class="si">{}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">random_choice</span><span class="p">))</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>Sample: Somalia_1087508.png
</pre>
</div>
</div>
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
"
class="
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Step-4:-Model-Performance-Evaluation">Step 4: Model Performance Evaluation<a class="anchor-link" href="#Step-4:-Model-Performance-Evaluation">&#182;</a></h3><p>The last step is to generate evaluation metrics on the inference performed. As we have learned, <strong>precision</strong>, <strong>recall</strong>, and <strong>IoU</strong> are useful metrics when evaluating a segmentation model. These metrics are derived from the confusion matrix, as shown below:</p>
<p><img src='images/precision_recall.png' width=720></p>
<p>The first measure is focused on identifying positive cases and is called recall. We define recall as the ability of the model to identify all true positive samples of the dataset. In mathematical terms, recall is the ratio of true positives over true positives plus false negatives. By other means, recall tells us, among all the test samples belonging to the output class, how many of them are identified correctly by the model. The next measure is called precision and is defined as the ability of the model to identify the relevant samples only. It is the ratio of true positives over true positives plus false positives. The last metric is called intersection over union and measures the overlap between the actual and predicted positive, as depicted below:</p>
<p><img src='images/metrics_visual.png' width=720></p>
<p><strong>Instructions</strong>: <br>
4.1 Replace the <code>&lt;FIXME&gt;</code>s with either <code>==</code> (equal) or <code>!=</code> (not equal) as appropriate, and execute the below cell to define the <code>calc_confusion_matrix</code> function. <br>
4.2 Execute the cell below to calculate precision, recall, and IoU (intersection over union) for class <code>1</code>, which indicates <code>flood</code>. <br>
4.3 Execute the cell below to mark your answer for grading.</p>
<p><strong>Notes</strong>: <br>
Only the IoU will be graded. To help you complete the assessment, we have provided the precision and recall.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[14]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 4.1</span>
<span class="c1"># define calc_confusion_matrix function</span>
<span class="k">def</span> <span class="nf">calc_confusion_matrix</span><span class="p">(</span><span class="n">inference</span><span class="p">,</span> <span class="n">ground_truth</span><span class="p">,</span> <span class="n">class_id</span><span class="p">):</span> 
    <span class="c1"># calculate true positive, false positive, false negative, and true positive</span>
    <span class="n">true_negative</span><span class="o">=</span><span class="p">((</span><span class="n">inference</span><span class="o">!=</span><span class="n">class_id</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">ground_truth</span><span class="o">!=</span><span class="n">class_id</span><span class="p">))</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
    <span class="n">false_positive</span><span class="o">=</span><span class="p">((</span><span class="n">inference</span><span class="o">==</span><span class="n">class_id</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">ground_truth</span><span class="o">!=</span><span class="n">class_id</span><span class="p">))</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
    <span class="n">false_negative</span><span class="o">=</span><span class="p">((</span><span class="n">inference</span><span class="o">!=</span><span class="n">class_id</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">ground_truth</span><span class="o">==</span><span class="n">class_id</span><span class="p">))</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
    <span class="n">true_positive</span><span class="o">=</span><span class="p">((</span><span class="n">inference</span><span class="o">==</span><span class="n">class_id</span><span class="p">)</span> <span class="o">&amp;</span> <span class="p">(</span><span class="n">ground_truth</span><span class="o">==</span><span class="n">class_id</span><span class="p">))</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
    <span class="k">return</span> <span class="n">true_negative</span><span class="p">,</span> <span class="n">false_positive</span><span class="p">,</span> <span class="n">false_negative</span><span class="p">,</span> <span class="n">true_positive</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[15]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 4.2</span>
<span class="c1"># DO NOT CHANAGE THIS CELL</span>
<span class="c1"># set target class and create lists to hold tn, fp, fn, and tp</span>
<span class="n">target_class</span><span class="o">=</span><span class="mi">1</span>
<span class="n">tns</span><span class="o">=</span><span class="p">[]</span>
<span class="n">fps</span><span class="o">=</span><span class="p">[]</span>
<span class="n">fns</span><span class="o">=</span><span class="p">[]</span>
<span class="n">tps</span><span class="o">=</span><span class="p">[]</span>

<span class="k">for</span> <span class="n">each_inference</span> <span class="ow">in</span> <span class="n">os</span><span class="o">.</span><span class="n">listdir</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">):</span> 
    <span class="k">if</span> <span class="n">each_inference</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;.&#39;</span><span class="p">)[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span><span class="o">==</span><span class="s1">&#39;png&#39;</span><span class="p">:</span> 
        <span class="n">inference</span><span class="o">=</span><span class="n">plt</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">,</span> <span class="n">each_inference</span><span class="p">))</span><span class="o">*</span><span class="mi">255</span>
        <span class="n">ground_truth</span><span class="o">=</span><span class="n">plt</span><span class="o">.</span><span class="n">imread</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">os</span><span class="o">.</span><span class="n">getenv</span><span class="p">(</span><span class="s1">&#39;LOCAL_DATA_DIR&#39;</span><span class="p">),</span> <span class="s1">&#39;masks&#39;</span><span class="p">,</span> <span class="s1">&#39;all_masks&#39;</span><span class="p">,</span> <span class="n">each_inference</span><span class="p">))</span>

        <span class="n">tn</span><span class="p">,</span> <span class="n">fp</span><span class="p">,</span> <span class="n">fn</span><span class="p">,</span> <span class="n">tp</span><span class="o">=</span><span class="n">calc_confusion_matrix</span><span class="p">(</span><span class="n">inference</span><span class="p">,</span> <span class="n">ground_truth</span><span class="p">,</span> <span class="n">target_class</span><span class="p">)</span>
        <span class="n">tps</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">tp</span><span class="p">)</span>
        <span class="n">fps</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">fp</span><span class="p">)</span>
        <span class="n">fns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">fn</span><span class="p">)</span>
        <span class="n">tns</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">tn</span><span class="p">)</span>
            
<span class="n">recall</span><span class="o">=</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">+</span><span class="nb">sum</span><span class="p">(</span><span class="n">fns</span><span class="p">))</span>
<span class="n">precision</span><span class="o">=</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">+</span><span class="nb">sum</span><span class="p">(</span><span class="n">fps</span><span class="p">))</span>
<span class="n">iou</span><span class="o">=</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">tps</span><span class="p">)</span><span class="o">+</span><span class="nb">sum</span><span class="p">(</span><span class="n">fps</span><span class="p">)</span><span class="o">+</span><span class="nb">sum</span><span class="p">(</span><span class="n">fns</span><span class="p">))</span>

<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Recall is </span><span class="si">{}</span><span class="s1"> when it should be 0.6649179565283793. &#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">recall</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;Precision is </span><span class="si">{}</span><span class="s1"> when it should be 0.7669037257648811. &#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">precision</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;IoU is </span><span class="si">{}</span><span class="s1">. &#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">iou</span><span class="p">))</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>Recall is 0.6649179565283793 when it should be 0.6649179565283793. 
Precision is 0.7669037257648811 when it should be 0.7669037257648811. 
IoU is 0.5531311258230802. 
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[16]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># 4.3</span>
<span class="c1"># DO NOT CHANGE BELOW</span>
<span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="s1">&#39;/dli/task/my_assessment/answer.txt&#39;</span><span class="p">,</span> <span class="s1">&#39;w&#39;</span><span class="p">)</span> <span class="k">as</span> <span class="n">f</span><span class="p">:</span> 
    <span class="n">f</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="nb">round</span><span class="p">(</span><span class="n">iou</span><span class="p">,</span> <span class="mi">2</span><span class="p">)))</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="Grade-Your-Code">Grade Your Code<a class="anchor-link" href="#Grade-Your-Code">&#182;</a></h3><p>If you have completed model evaluation successfully, save changes to the notebook and revisit the webpage where you launched this interactive environment. Click on the &quot;<strong>ASSESS TASK</strong>&quot; button as shown in the screenshot below. Doing so will give you credit for this part of the lab that counts towards earning a certificate of competency for the entire course.</p>
<p><img src='images/credit.png' width=720></p>

</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h3 id="BONUS.-Performance-Evaluation">BONUS. Performance Evaluation<a class="anchor-link" href="#BONUS.-Performance-Evaluation">&#182;</a></h3><p>Below we have included some sample procedures to calculate the performance metrics based on image groups - this is intended to demonstrate potential weaknesses of the model that could warrant further fine-tuning of the model. There are a number of techniques to improve model performance, including adding relevant training data.</p>
<p><strong>Instructions</strong>: <br>
B.1 Execute the below cell to create a DataFrame with the appropriate data. <br>
B.2 Execute the cell below to calculate IoU for each image group and visualize the results for comparison.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[17]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># DO NOT CHANGE THIS CELL</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>

<span class="c1"># create DataFrame</span>
<span class="n">df</span><span class="o">=</span><span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">({</span><span class="s1">&#39;image&#39;</span><span class="p">:</span> <span class="n">os</span><span class="o">.</span><span class="n">listdir</span><span class="p">(</span><span class="s1">&#39;inference_results&#39;</span><span class="p">),</span> 
                 <span class="s1">&#39;tp&#39;</span><span class="p">:</span> <span class="n">tps</span><span class="p">,</span> 
                 <span class="s1">&#39;fp&#39;</span><span class="p">:</span> <span class="n">fps</span><span class="p">,</span> 
                 <span class="s1">&#39;fn&#39;</span><span class="p">:</span> <span class="n">fns</span><span class="p">,</span> 
                 <span class="s1">&#39;tn&#39;</span><span class="p">:</span> <span class="n">tns</span><span class="p">})</span>

<span class="c1"># create image_group, union, and intersect columns</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;image_group&#39;</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;image&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">split</span><span class="p">(</span><span class="s1">&#39;_&#39;</span><span class="p">)</span><span class="o">.</span><span class="n">str</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;union&#39;</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;tp&#39;</span><span class="p">]</span><span class="o">+</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;fp&#39;</span><span class="p">]</span><span class="o">+</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;fn&#39;</span><span class="p">]</span>
<span class="n">df</span><span class="p">[</span><span class="s1">&#39;intersect&#39;</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">&#39;tp&#39;</span><span class="p">]</span>
<span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[17]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>image</th>
      <th>tp</th>
      <th>fp</th>
      <th>fn</th>
      <th>tn</th>
      <th>image_group</th>
      <th>union</th>
      <th>intersect</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>India_1018317.png</td>
      <td>148847</td>
      <td>31694</td>
      <td>1863</td>
      <td>79740</td>
      <td>India</td>
      <td>182404</td>
      <td>148847</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Sri-Lanka_579082.png</td>
      <td>5415</td>
      <td>3075</td>
      <td>9051</td>
      <td>244603</td>
      <td>Sri-Lanka</td>
      <td>17541</td>
      <td>5415</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Ghana_187318.png</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>262144</td>
      <td>Ghana</td>
      <td>0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Pakistan_760290.png</td>
      <td>0</td>
      <td>1575</td>
      <td>0</td>
      <td>260569</td>
      <td>Pakistan</td>
      <td>1575</td>
      <td>0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>USA_778194.png</td>
      <td>2013</td>
      <td>505</td>
      <td>1825</td>
      <td>257801</td>
      <td>USA</td>
      <td>4343</td>
      <td>2013</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[18]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># B.2</span>
<span class="c1"># group by image_group and calculate iou</span>
<span class="n">df_grouped</span><span class="o">=</span><span class="n">df</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">&#39;image_group&#39;</span><span class="p">)[[</span><span class="s1">&#39;intersect&#39;</span><span class="p">,</span> <span class="s1">&#39;union&#39;</span><span class="p">]]</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
<span class="n">df_grouped</span><span class="p">[</span><span class="s1">&#39;iou&#39;</span><span class="p">]</span><span class="o">=</span><span class="n">df_grouped</span><span class="p">[</span><span class="s1">&#39;intersect&#39;</span><span class="p">]</span><span class="o">/</span><span class="n">df_grouped</span><span class="p">[</span><span class="s1">&#39;union&#39;</span><span class="p">]</span>

<span class="c1"># visualize results</span>
<span class="n">df_grouped</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="s1">&#39;iou&#39;</span><span class="p">,</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)[</span><span class="s1">&#39;iou&#39;</span><span class="p">]</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">kind</span><span class="o">=</span><span class="s1">&#39;bar&#39;</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">10</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;IoU by Image Group&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Image Group&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;IoU&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>


<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA04AAAIJCAYAAACSim3hAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/NK7nSAAAACXBIWXMAAA9hAAAPYQGoP6dpAABhPElEQVR4nO3deVxV1f7/8TeggBM4IDiEomIOKWLilBqmGDmb3TKHQDQrUzPRW1omDiWWOevNJmcL07ym6dcJh65KOaU5m1NSCqImJiio7N8f/jxJHNxaygbP6/l47MeDs/be53zOzg68z1p7LSfDMAwBAAAAALLlbHUBAAAAAJDbEZwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAH+Lk5OT+vbta3UZAADkCIITAORBs2bNkpOTk7Zv337X5w4fPlxOTk46e/as3f01atRQ06ZN/2GF98aGDRvk5OSkRYsWWV3KfZeWlqYpU6aocePGKlasmFxdXVWmTBm1a9dOX375pa5fv251iQDg0PJZXQAAAI4uKSlJLVu21I4dOxQaGqqhQ4eqePHiSkhI0Nq1a9WlSxcdOXJE77zzjtWlAoDDIjgBAGCxF154QT/++KO+/vprdezYMdO+IUOGaPv27Tp06NBtn+PKlStydXWVszODSQDgfuDTFQAeIOvWrVOTJk1UqFAhFS1aVO3bt9eBAwfu62vOnz9fVapUkbu7u+rUqaPvvvvOtm/9+vVycnLSf//73yznffHFF3JyclJcXNxdvd7NoYaHDx9Wt27d5OnpqZIlS+qdd96RYRiKj49X+/bt5eHhoVKlSmncuHGZzk9PT9ewYcNUp04deXp6qlChQmrSpInWr1+f5bXOnTunF154QR4eHipatKjCw8O1e/duOTk5adasWZmOPXjwoP71r3+pePHicnd3V1BQkJYuXWr6fuLi4rRq1Sq99NJLWULTTUFBQeratavt8c0hjDExMRo6dKjKli2rggUL6uLFi5KkhQsXqk6dOipQoIC8vLzUrVs3/fbbb5mes2nTpnaHZHbv3l1+fn62xydOnJCTk5M+/PBDTZgwQeXLl1eBAgUUHBysvXv3mr4/AHhQEJwA4AGxdu1ahYaG6syZMxo+fLgiIyO1ZcsWNWrUSCdOnLgvr7lx40a9/vrr6tatm0aOHKlz587pqaeesv1B3bRpU/n6+mr+/PlZzp0/f74qVaqkhg0b/q3X7tSpkzIyMjRmzBjVr19f7777riZOnKgWLVqobNmyev/99+Xv769BgwZlCnMXL17UZ599pqZNm+r999/X8OHDlZSUpNDQUO3atct2XEZGhtq2basvv/xS4eHheu+993T69GmFh4dnqWXfvn1q0KCBDhw4oMGDB2vcuHEqVKiQOnToYDc03mrZsmWSpG7dut31NRg1apSWL1+uQYMGafTo0XJ1ddWsWbP03HPPycXFRdHR0erVq5cWL16sxo0b68KFC3f9GjfNmTNHkydPVp8+fTRkyBDt3btXzZo1U2Ji4t9+TgDIUwwAQJ4zc+ZMQ5Kxbds2W1tgYKDh7e1tnDt3zta2e/duw9nZ2QgLC7O1RUVFGZKMpKQku8/9yCOPGMHBwaY1SDIkGdu3b7e1/fLLL4a7u7vx9NNP29qGDBliuLm5GRcuXLC1nTlzxsiXL58RFRV129dYv369IclYuHBhlvpfeuklW9u1a9eMhx56yHBycjLGjBlja//999+NAgUKGOHh4ZmOTUtLy/Q6v//+u+Hj42P06NHD1vb1118bkoyJEyfa2q5fv240a9bMkGTMnDnT1t68eXOjZs2axpUrV2xtGRkZxmOPPWZUrlz5tu/x6aefNiRluj6GYRiXL182kpKSbNvvv/+e5bpUrFjRSE1NtbWnp6cb3t7eRo0aNYzLly/b2r/99ltDkjFs2DBbW3BwsN3/zuHh4Ub58uVtj48fP25IMgoUKGD8+uuvtvYffvjBkGQMGDDgtu8PAB4U9DgBwAPg9OnT2rVrl7p3767ixYvb2gMCAtSiRQutWLHivrxuw4YNVadOHdvjcuXKqX379lq1apVtFriwsDClpaVlmhlvwYIFunbt2t/qZbnpxRdftP3s4uKioKAgGYahnj172tqLFi2qKlWq6NixY5mOdXV1lXSjV+n8+fO6du2agoKCtHPnTttxK1euVP78+dWrVy9bm7Ozs/r06ZOpjvPnz2vdunV67rnn9Mcff+js2bM6e/aszp07p9DQUP38889Zhsnd6ubwusKFC2dqnz59ukqWLGnbGjdunOXc8PBwFShQwPZ4+/btOnPmjF599VW5u7vb2lu3bq2qVatq+fLl2dZhpkOHDipbtqztcb169VS/fv379m8LAHIbghMAPAB++eUXSVKVKlWy7KtWrZrOnj2rlJSUO34+JyenOzqucuXKWdoefvhhpaamKikpSZJUtWpV1a1bN9Nwvfnz56tBgwby9/e/45r+qly5cpkee3p6yt3dXV5eXlnaf//990xts2fPVkBAgNzd3VWiRAmVLFlSy5cvV3Jysu2YX375RaVLl1bBggUznfvXmo8cOSLDMPTOO+9kCjolS5ZUVFSUJOnMmTPZvo8iRYpIki5dupSp/ZlnntGaNWu0Zs0aBQQE2D23QoUKmR7f7t9B1apVbfv/juz+W9+vYaAAkNswqx4AOJibPRGXL1+2uz81NTVTb8W9EBYWpv79++vXX39VWlqavv/+e02dOvUfPaeLi8sdtUmSYRi2n+fNm6fu3burQ4cO+ve//y1vb2/b/UBHjx696zoyMjIkSYMGDVJoaKjdY24XEKtWrSpJ2rt3rxo1amRr9/X1la+vrySpWLFidtfdurW36W45OTllui43sV4UANhHcAKAB0D58uUlye6U1QcPHpSXl5cKFSqU5dibf5jflJqaqvj4eD355JN39Lo///xzlrbDhw+rYMGCKlmypK3t+eefV2RkpL788ktdvnxZ+fPnV6dOne7szd1jixYtUsWKFbV48eJMPWs3e4duKl++vNavX6/U1NRMvU5HjhzJdFzFihUlSfnz51dISMhd19OmTRuNGTNG8+fPzxSc/o5b/9s2a9Ys075Dhw7Z9ks3wtitQxhvyq5XKrv/1rfOwAcADzKG6gHAA6B06dIKDAzU7NmzM82ctnfvXq1evVqtWrWytTVv3lyurq766KOPbL0lN33yySe6du2aWrZseUevGxcXl+m+oPj4eH3zzTd68sknM/X+eHl5qWXLlpo3b57mz5+vp556KsuQupxys65be1t++OGHLNOih4aG6urVq/r0009tbRkZGZo2bVqm47y9vdW0aVN9/PHHOn36dJbXuzlkMTuNGjVSixYt9Mknn+ibb76xe4y9niF7goKC5O3trenTpystLc3W/n//9386cOCAWrdubWurVKmSDh48mKm+3bt3a/PmzXafe8mSJZnu1dq6dat++OGHO/63AgB5HT1OAPCAGDt2rFq2bKmGDRuqZ8+eunz5sqZMmSJPT08NHz7cdpy3t7eGDRumoUOH6vHHH1e7du1UsGBBbdmyRV9++aWefPJJtW3b9o5es0aNGgoNDdVrr70mNzc3/ec//5EkjRgxIsuxYWFh+te//iXpxjTaVmnTpo0WL16sp59+Wq1bt9bx48c1ffp0Va9ePdN9Rh06dFC9evU0cOBAHTlyRFWrVtXSpUt1/vx5SZnvA5s2bZoaN26smjVrqlevXqpYsaISExMVFxenX3/9Vbt3775tTfPmzdNTTz2lDh06qGXLlgoJCVGxYsWUkJCgtWvX6rvvvrujgJI/f369//77ioiIUHBwsDp37qzExERNmjRJfn5+GjBggO3YHj16aPz48QoNDVXPnj115swZTZ8+XY888ohtwopb+fv7q3Hjxurdu7fS0tI0ceJElShRQm+88YZpXQDwQLBySj8AwN9jbzpywzCMtWvXGo0aNTIKFChgeHh4GG3btjX2799v9znmzZtnNGjQwChUqJDh5uZmVK1a1RgxYkSmKbVvR5LRp08fY968eUblypUNNzc3o3bt2sb69evtHp+WlmYUK1bM8PT0zDRV9u3cbjryv06nHh4ebhQqVCjLcwQHBxuPPPKI7XFGRoYxevRoo3z58raav/322yzTcBuGYSQlJRldunQxihQpYnh6ehrdu3c3Nm/ebEgyYmJiMh179OhRIywszChVqpSRP39+o2zZskabNm2MRYsW3dF7vXz5sjFx4kSjYcOGhoeHh5EvXz6jVKlSRps2bYz58+cb165du+11udWCBQuM2rVrG25ubkbx4sWNrl27ZppK/KZ58+YZFStWNFxdXY3AwEBj1apV2U5HPnbsWGPcuHGGr6+v4ebmZjRp0sTYvXv3Hb03AHgQOBnGHfb/AwDwD1y7dk1lypRR27Zt9fnnn1tdzt+2ZMkSPf3009q0adM/vicpLzhx4oQqVKigsWPHatCgQVaXAwCW4R4nAECOWLJkiZKSkhQWFmZ1KXfsrzMPXr9+XVOmTJGHh4ceffRRi6oCAFiBe5wAAPfVDz/8oJ9++kmjRo1S7dq1FRwcbHVJd6xfv366fPmyGjZsqLS0NC1evFhbtmzR6NGj/9FU4ACAvIfgBAC4rz766CPNmzdPgYGBmjVrltXl3JVmzZpp3Lhx+vbbb3XlyhX5+/trypQp6tu3r9WlAQByGPc4AQAAAIAJ7nECAAAAABMON1QvIyNDp06dUpEiRTKtwQEAAADAsRiGoT/++ENlypSRs/Pt+5QcLjidOnVKvr6+VpcBAAAAIJeIj4/XQw89dNtjHC44FSlSRNKNi+Ph4WFxNQAAAACscvHiRfn6+toywu04XHC6OTzPw8OD4AQAAADgjm7hYXIIAAAAADBBcAIAAAAAEwQnAAAAADBheXCaNm2a/Pz85O7urvr162vr1q23PX7ixImqUqWKChQoIF9fXw0YMEBXrlzJoWoBAAAAOCJLg9OCBQsUGRmpqKgo7dy5U7Vq1VJoaKjOnDlj9/gvvvhCgwcPVlRUlA4cOKDPP/9cCxYs0FtvvZXDlQMAAABwJE6GYRhWvXj9+vVVt25dTZ06VdKNxWl9fX3Vr18/DR48OMvxffv21YEDBxQbG2trGzhwoH744Qdt2rTJ7mukpaUpLS3N9vjmlIPJycnMqgcAAAA4sIsXL8rT0/OOsoFlPU7p6enasWOHQkJC/izG2VkhISGKi4uze85jjz2mHTt22IbzHTt2TCtWrFCrVq2yfZ3o6Gh5enraNha/BQAAAHC3LFvH6ezZs7p+/bp8fHwytfv4+OjgwYN2z+nSpYvOnj2rxo0byzAMXbt2Ta+88spth+oNGTJEkZGRtsc3e5wAAAAA4E5ZPjnE3diwYYNGjx6t//znP9q5c6cWL16s5cuXa9SoUdme4+bmZlvslkVvAQAAAPwdlvU4eXl5ycXFRYmJiZnaExMTVapUKbvnvPPOO3rhhRf04osvSpJq1qyplJQUvfTSS3r77bfl7JynciAAAACAPMKypOHq6qo6depkmughIyNDsbGxatiwod1zUlNTs4QjFxcXSZKFc1wAAAAAeMBZ1uMkSZGRkQoPD1dQUJDq1auniRMnKiUlRREREZKksLAwlS1bVtHR0ZKktm3bavz48apdu7bq16+vI0eO6J133lHbtm1tAQoAAAAA7jVLg1OnTp2UlJSkYcOGKSEhQYGBgVq5cqVtwoiTJ09m6mEaOnSonJycNHToUP32228qWbKk2rZtq/fee8+qtwAAAADAAVi6jpMV7maudgAAAAAPrjyxjhMAAAAA5BUEJwAAAAAwYek9Tnmd3+DlVpdgc2JMa6tLAAAAAB5Y9DgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgIl8VheAB4/f4OVWl5DJiTGtrS4BAAAAeRw9TgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgIlcEp2nTpsnPz0/u7u6qX7++tm7dmu2xTZs2lZOTU5atdWtmTgMAAABwf1genBYsWKDIyEhFRUVp586dqlWrlkJDQ3XmzBm7xy9evFinT5+2bXv37pWLi4ueffbZHK4cAAAAgKOwPDiNHz9evXr1UkREhKpXr67p06erYMGCmjFjht3jixcvrlKlStm2NWvWqGDBgtkGp7S0NF28eDHTBgAAAAB3w9LglJ6erh07digkJMTW5uzsrJCQEMXFxd3Rc3z++ed6/vnnVahQIbv7o6Oj5enpadt8fX3vSe0AAAAAHIelwens2bO6fv26fHx8MrX7+PgoISHB9PytW7dq7969evHFF7M9ZsiQIUpOTrZt8fHx/7huAAAAAI4ln9UF/BOff/65atasqXr16mV7jJubm9zc3HKwKgAAAAAPGkt7nLy8vOTi4qLExMRM7YmJiSpVqtRtz01JSVFMTIx69ux5P0sEAAAAAGuDk6urq+rUqaPY2FhbW0ZGhmJjY9WwYcPbnrtw4UKlpaWpW7du97tMAAAAAA7O8qF6kZGRCg8PV1BQkOrVq6eJEycqJSVFERERkqSwsDCVLVtW0dHRmc77/PPP1aFDB5UoUcKKsgEAAAA4EMuDU6dOnZSUlKRhw4YpISFBgYGBWrlypW3CiJMnT8rZOXPH2KFDh7Rp0yatXr3aipIBAAAAOBjLg5Mk9e3bV3379rW7b8OGDVnaqlSpIsMw7nNVAAAAAHCD5QvgAgAAAEBuR3ACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwkc/qAgBH4jd4udUl2JwY09rqEgAAAPIMepwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMEJwAAAAAwATBCQAAAABMWB6cpk2bJj8/P7m7u6t+/fraunXrbY+/cOGC+vTpo9KlS8vNzU0PP/ywVqxYkUPVAgAAAHBE+ax88QULFigyMlLTp09X/fr1NXHiRIWGhurQoUPy9vbOcnx6erpatGghb29vLVq0SGXLltUvv/yiokWL5nzxAAAAAByGpcFp/Pjx6tWrlyIiIiRJ06dP1/LlyzVjxgwNHjw4y/EzZszQ+fPntWXLFuXPn1+S5Ofnd9vXSEtLU1pamu3xxYsX790bAAAAAOAQLAtO6enp2rFjh4YMGWJrc3Z2VkhIiOLi4uyes3TpUjVs2FB9+vTRN998o5IlS6pLly5688035eLiYvec6OhojRgx4r68BwD3ht/g5VaXYHNiTGurSwAAALmQZfc4nT17VtevX5ePj0+mdh8fHyUkJNg959ixY1q0aJGuX7+uFStW6J133tG4ceP07rvvZvs6Q4YMUXJysm2Lj4+/p+8DAAAAwIPP0qF6dysjI0Pe3t765JNP5OLiojp16ui3337T2LFjFRUVZfccNzc3ubm55XClAAAAAB4klgUnLy8vubi4KDExMVN7YmKiSpUqZfec0qVLK3/+/JmG5VWrVk0JCQlKT0+Xq6vrfa0ZAAAAgGOybKieq6ur6tSpo9jYWFtbRkaGYmNj1bBhQ7vnNGrUSEeOHFFGRoat7fDhwypdujShCQAAAMB9Y+k6TpGRkfr00081e/ZsHThwQL1791ZKSoptlr2wsLBMk0f07t1b58+fV//+/XX48GEtX75co0ePVp8+fax6CwAAAAAcgKX3OHXq1ElJSUkaNmyYEhISFBgYqJUrV9omjDh58qScnf/Mdr6+vlq1apUGDBiggIAAlS1bVv3799ebb75p1VsAAAAA4AAsnxyib9++6tu3r919GzZsyNLWsGFDff/99/e5KgAAAAD4k6VD9QAAAAAgLyA4AQAAAIAJy4fqAQCy5zd4udUl2JwY09rqEgAAsAw9TgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgIp/VBQAAcLf8Bi+3ugSbE2NaW10CACAH0OMEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACYITgAAAABgguAEAAAAACZyRXCaNm2a/Pz85O7urvr162vr1q3ZHjtr1iw5OTll2tzd3XOwWgAAAACOxvLgtGDBAkVGRioqKko7d+5UrVq1FBoaqjNnzmR7joeHh06fPm3bfvnllxysGAAAAICjsTw4jR8/Xr169VJERISqV6+u6dOnq2DBgpoxY0a25zg5OalUqVK2zcfHJ9tj09LSdPHixUwbAAAAANwNS4NTenq6duzYoZCQEFubs7OzQkJCFBcXl+15ly5dUvny5eXr66v27dtr37592R4bHR0tT09P2+br63tP3wMAAACAB5+lwens2bO6fv16lh4jHx8fJSQk2D2nSpUqmjFjhr755hvNmzdPGRkZeuyxx/Trr7/aPX7IkCFKTk62bfHx8ff8fQAAAAB4sOWzuoC71bBhQzVs2ND2+LHHHlO1atX08ccfa9SoUVmOd3Nzk5ubW06WCAAAAOABY2mPk5eXl1xcXJSYmJipPTExUaVKlbqj58ifP79q166tI0eO3I8SAQAAAMDa4OTq6qo6deooNjbW1paRkaHY2NhMvUq3c/36de3Zs0elS5e+X2UCAAAAcHCWD9WLjIxUeHi4goKCVK9ePU2cOFEpKSmKiIiQJIWFhals2bKKjo6WJI0cOVINGjSQv7+/Lly4oLFjx+qXX37Riy++aOXbAAAAAPAAszw4derUSUlJSRo2bJgSEhIUGBiolStX2iaMOHnypJyd/+wY+/3339WrVy8lJCSoWLFiqlOnjrZs2aLq1atb9RYAAAAAPOAsD06S1LdvX/Xt29fuvg0bNmR6PGHCBE2YMCEHqgIAAACAGyxfABcAAAAAcjuCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgAmCEwAAAACYIDgBAAAAgIlcsY4TAAC4N/wGL7e6BJsTY1pbXQIA3DP0OAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJggOAEAAACACYITAAAAAJjIdzcHT5482W67p6enHn74YTVs2PCeFAUAAAAAucldBacJEybYbb9w4YKSk5P12GOPaenSpSpevPg9KQ4AAAAAcoO7Gqp3/Phxu9vvv/+uI0eOKCMjQ0OHDr1ftQIAAACAJe7ZPU4VK1bUmDFjtHr16nv1lAAAAACQK9zTySHKlSunhISEe/mUAAAAAGC5exqc9uzZo/Lly9/LpwQAAAAAy93V5BAXL160256cnKwdO3Zo4MCBCg8PvyeFAQAAAEBucVfBqWjRonJycrK7z8nJSS+++KIGDx58TwoDAAAAgNziroLT+vXr7bZ7eHiocuXKKly48N8qYtq0aRo7dqwSEhJUq1YtTZkyRfXq1TM9LyYmRp07d1b79u21ZMmSv/XaAAAAAGDmroJTcHDwPS9gwYIFioyM1PTp01W/fn1NnDhRoaGhOnTokLy9vbM978SJExo0aJCaNGlyz2sCAAAAgFv97ckhLly4oHHjxunFF1/Uiy++qPHjxys5Ofmun2f8+PHq1auXIiIiVL16dU2fPl0FCxbUjBkzsj3n+vXr6tq1q0aMGKGKFSve9vnT0tJ08eLFTBsAAAAA3I276nG6afv27QoNDVWBAgVsQ+omTJig0aNHa/Xq1Xr00Ufv6HnS09O1Y8cODRkyxNbm7OyskJAQxcXFZXveyJEj5e3trZ49e+p///vfbV8jOjpaI0aMuKN6AADAg8lv8HKrS7A5Maa11SUA+Bv+Vo/TgAED1K5dO504cUKLFy/W4sWLdfz4cbVp00avv/76HT/P2bNndf36dfn4+GRq9/HxyXY9qE2bNunzzz/Xp59+ekevMWTIECUnJ9u2+Pj4O64PAAAAAKR/0OP06aefKl++P0/Ply+f3njjDQUFBd2z4v7qjz/+0AsvvKBPP/1UXl5ed3SOm5ub3Nzc7ltNAAAAAB58fys4eXh46OTJk6patWqm9vj4eBUpUuSOn8fLy0suLi5KTEzM1J6YmKhSpUplOf7o0aM6ceKE2rZta2vLyMiQdCO4HTp0SJUqVbqbtwIAAAAApv7WUL1OnTqpZ8+eWrBggeLj4xUfH6+YmBi9+OKL6ty58x0/j6urq+rUqaPY2FhbW0ZGhmJjY9WwYcMsx1etWlV79uzRrl27bFu7du30xBNPaNeuXfL19f07bwcAAAAAbutv9Th9+OGHcnJyUlhYmK5duybDMOTq6qrevXtrzJgxd/VckZGRCg8PV1BQkOrVq6eJEycqJSVFERERkqSwsDCVLVtW0dHRcnd3V40aNTKdX7RoUUnK0g4AAAAA98rfCk6urq6aNGmSoqOjdfToUUlSpUqVVLBgwbt+rk6dOikpKUnDhg1TQkKCAgMDtXLlStuEESdPnpSz89+eNR0AAAAA/rG7Ck4dO3a8o+MWL158V0X07dtXffv2tbtvw4YNtz131qxZd/VaAAAAAHC37io4eXp63q86AAAAACDXuqvgNHPmzPtVBwAAAADkWtw8BAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYCKf1QUAAADAOn6Dl1tdgs2JMa2tLgHIFj1OAAAAAGCC4AQAAAAAJghOAAAAAGCC4AQAAAAAJghOAAAAAGCC4AQAAAAAJghOAAAAAGCC4AQAAAAAJghOAAAAAGCC4AQAAAAAJghOAAAAAGAiVwSnadOmyc/PT+7u7qpfv762bt2a7bGLFy9WUFCQihYtqkKFCikwMFBz587NwWoBAAAAOBrLg9OCBQsUGRmpqKgo7dy5U7Vq1VJoaKjOnDlj9/jixYvr7bffVlxcnH766SdFREQoIiJCq1atyuHKAQAAADgKy4PT+PHj1atXL0VERKh69eqaPn26ChYsqBkzZtg9vmnTpnr66adVrVo1VapUSf3791dAQIA2bdpk9/i0tDRdvHgx0wYAAAAAd8PS4JSenq4dO3YoJCTE1ubs7KyQkBDFxcWZnm8YhmJjY3Xo0CE9/vjjdo+Jjo6Wp6enbfP19b1n9QMAAABwDJYGp7Nnz+r69evy8fHJ1O7j46OEhIRsz0tOTlbhwoXl6uqq1q1ba8qUKWrRooXdY4cMGaLk5GTbFh8ff0/fAwAAAIAHXz6rC/g7ihQpol27dunSpUuKjY1VZGSkKlasqKZNm2Y51s3NTW5ubjlfJAAAAIAHhqXBycvLSy4uLkpMTMzUnpiYqFKlSmV7nrOzs/z9/SVJgYGBOnDggKKjo+0GJwAAAAD4pywdqufq6qo6deooNjbW1paRkaHY2Fg1bNjwjp8nIyNDaWlp96NEAAAAALB+qF5kZKTCw8MVFBSkevXqaeLEiUpJSVFERIQkKSwsTGXLllV0dLSkG5M9BAUFqVKlSkpLS9OKFSs0d+5cffTRR1a+DQAAAAAPMMuDU6dOnZSUlKRhw4YpISFBgYGBWrlypW3CiJMnT8rZ+c+OsZSUFL366qv69ddfVaBAAVWtWlXz5s1Tp06drHoLAAAAAB5wlgcnSerbt6/69u1rd9+GDRsyPX733Xf17rvv5kBVAAAAAHCD5QvgAgAAAEBuR3ACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABMEJwAAAAAwQXACAAAAABP5rC4AAAAAyG38Bi+3ugSbE2NaW10CRI8TAAAAAJgiOAEAAACACYbqAQAAALgjuWkIo5SzwxjpcQIAAAAAEwQnAAAAADBBcAIAAAAAEwQnAAAAADBBcAIAAAAAEwQnAAAAADBBcAIAAAAAEwQnAAAAADBBcAIAAAAAEwQnAAAAADBBcAIAAAAAEwQnAAAAADCRK4LTtGnT5OfnJ3d3d9WvX19bt27N9thPP/1UTZo0UbFixVSsWDGFhITc9ngAAAAA+KcsD04LFixQZGSkoqKitHPnTtWqVUuhoaE6c+aM3eM3bNigzp07a/369YqLi5Ovr6+efPJJ/fbbbzlcOQAAAABHYXlwGj9+vHr16qWIiAhVr15d06dPV8GCBTVjxgy7x8+fP1+vvvqqAgMDVbVqVX322WfKyMhQbGys3ePT0tJ08eLFTBsAAAAA3A1Lg1N6erp27NihkJAQW5uzs7NCQkIUFxd3R8+Rmpqqq1evqnjx4nb3R0dHy9PT07b5+vrek9oBAAAAOA5Lg9PZs2d1/fp1+fj4ZGr38fFRQkLCHT3Hm2++qTJlymQKX7caMmSIkpOTbVt8fPw/rhsAAACAY8lndQH/xJgxYxQTE6MNGzbI3d3d7jFubm5yc3PL4coAAAAAPEgsDU5eXl5ycXFRYmJipvbExESVKlXqtud++OGHGjNmjNauXauAgID7WSYAAAAAB2fpUD1XV1fVqVMn08QONyd6aNiwYbbnffDBBxo1apRWrlypoKCgnCgVAAAAgAOzfKheZGSkwsPDFRQUpHr16mnixIlKSUlRRESEJCksLExly5ZVdHS0JOn999/XsGHD9MUXX8jPz892L1ThwoVVuHBhy94HAAAAgAeX5cGpU6dOSkpK0rBhw5SQkKDAwECtXLnSNmHEyZMn5ez8Z8fYRx99pPT0dP3rX//K9DxRUVEaPnx4TpYOAAAAwEFYHpwkqW/fvurbt6/dfRs2bMj0+MSJE/e/IAAAAAC4heUL4AIAAABAbkdwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATBCcAAAAAMEFwAgAAAAATlgenadOmyc/PT+7u7qpfv762bt2a7bH79u3TM888Iz8/Pzk5OWnixIk5VygAAAAAh2VpcFqwYIEiIyMVFRWlnTt3qlatWgoNDdWZM2fsHp+amqqKFStqzJgxKlWqVA5XCwAAAMBRWRqcxo8fr169eikiIkLVq1fX9OnTVbBgQc2YMcPu8XXr1tXYsWP1/PPPy83N7Y5eIy0tTRcvXsy0AQAAAMDdsCw4paena8eOHQoJCfmzGGdnhYSEKC4u7p69TnR0tDw9PW2br6/vPXtuAAAAAI7BsuB09uxZXb9+XT4+PpnafXx8lJCQcM9eZ8iQIUpOTrZt8fHx9+y5AQAAADiGfFYXcL+5ubnd8bA+AAAAALDHsh4nLy8vubi4KDExMVN7YmIiEz8AAAAAyFUsC06urq6qU6eOYmNjbW0ZGRmKjY1Vw4YNrSoLAAAAALKwdKheZGSkwsPDFRQUpHr16mnixIlKSUlRRESEJCksLExly5ZVdHS0pBsTSuzfv9/282+//aZdu3apcOHC8vf3t+x9AAAAAHiwWRqcOnXqpKSkJA0bNkwJCQkKDAzUypUrbRNGnDx5Us7Of3aKnTp1SrVr17Y9/vDDD/Xhhx8qODhYGzZsyOnyAQAAADgIyyeH6Nu3r/r27Wt331/DkJ+fnwzDyIGqAAAAAOBPli6ACwAAAAB5AcEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEwQnAAAAADABMEJAAAAAEzkiuA0bdo0+fn5yd3dXfXr19fWrVtve/zChQtVtWpVubu7q2bNmlqxYkUOVQoAAADAEVkenBYsWKDIyEhFRUVp586dqlWrlkJDQ3XmzBm7x2/ZskWdO3dWz5499eOPP6pDhw7q0KGD9u7dm8OVAwAAAHAU+awuYPz48erVq5ciIiIkSdOnT9fy5cs1Y8YMDR48OMvxkyZN0lNPPaV///vfkqRRo0ZpzZo1mjp1qqZPn57l+LS0NKWlpdkeJycnS5IuXrz4j2vPSEv9x89xr9yL93Ov5KbrInFtssN1sS83XReJa5Mdrkv2uDb2cV2yx7Wxj+tiX266LtI/vzY3zzcMw/xgw0JpaWmGi4uL8d///jdTe1hYmNGuXTu75/j6+hoTJkzI1DZs2DAjICDA7vFRUVGGJDY2NjY2NjY2NjY2NrtbfHy8aXaxtMfp7Nmzun79unx8fDK1+/j46ODBg3bPSUhIsHt8QkKC3eOHDBmiyMhI2+OMjAydP39eJUqUkJOT0z98B//cxYsX5evrq/j4eHl4eFhdTq7BdbGP65I9ro19XJfscW3s47pkj2tjH9cle1wb+3LTdTEMQ3/88YfKlCljeqzlQ/XuNzc3N7m5uWVqK1q0qDXF3IaHh4fl/3ByI66LfVyX7HFt7OO6ZI9rYx/XJXtcG/u4Ltnj2tiXW66Lp6fnHR1n6eQQXl5ecnFxUWJiYqb2xMRElSpVyu45pUqVuqvjAQAAAOCfsjQ4ubq6qk6dOoqNjbW1ZWRkKDY2Vg0bNrR7TsOGDTMdL0lr1qzJ9ngAAAAA+KcsH6oXGRmp8PBwBQUFqV69epo4caJSUlJss+yFhYWpbNmyio6OliT1799fwcHBGjdunFq3bq2YmBht375dn3zyiZVv429zc3NTVFRUluGEjo7rYh/XJXtcG/u4Ltnj2tjHdcke18Y+rkv2uDb25dXr4mQYdzL33v01depUjR07VgkJCQoMDNTkyZNVv359SVLTpk3l5+enWbNm2Y5fuHChhg4dqhMnTqhy5cr64IMP1KpVK4uqBwAAAPCgyxXBCQAAAAByM0vvcQIAAACAvIDgBAAAAAAmCE4AAAAAYILgBAAAAAAmCE4AAAAAYILgBAAAAAAmLF8AF7jp+vXrmjVrlmJjY3XmzBllZGRk2r9u3TqLKkNu9uuvv2rp0qU6efKk0tPTM+0bP368RVVZLzw8XD179tTjjz9udSl5QkZGhlasWKE2bdpYXQqQp6Smptr9/A0ICLCootwhIyNDR44csfv3jCN/LqekpGjjxo12/8289tprFlV15whOFihWrJicnJyytDs5Ocnd3V3+/v7q3r27IiIiLKjOOv3799esWbPUunVr1ahRw+41cmQEhKxiY2PVrl07VaxYUQcPHlSNGjV04sQJGYahRx991OryLJWcnKyQkBCVL19eERERCg8PV9myZa0uK9c5cuSIZsyYoVmzZikpKUlXr161uiRLLVq0SF999ZXdz5mdO3daVFXusH//frvXpV27dhZVZK2kpCRFRETo//7v/+zuv379eg5XlHt8//336tKli3755Rf9dblUJycnh702P/74o1q1aqXU1FSlpKSoePHiOnv2rAoWLChvb+88EZxkIMeNHz/eKFGihNGtWzdj8uTJxuTJk41u3boZXl5exnvvvWe8+OKLhpubm/HJJ59YXWqOKlGihLF8+XKry8iV1q5daxQsWNCoUaOGkS9fPiMwMNAoWrSo4enpaTzxxBNWl2eZunXrGsOGDTMMwzAKFy5sHD161Pjjjz+Mdu3aGf/5z38srs56Z86cMcaNG2cEBAQY+fLlM5566ilj4cKFRnp6utWlWSo1NdWYPXu20aRJE8PZ2dkIDg42PvroIyMhIcHq0iw1adIko3Dhwkbfvn0NV1dX4+WXXzZCQkIMT09P46233rK6PMscPXrUCAgIMJycnAxnZ2fDycnJ9rOzs7PV5VmmS5cuRqNGjYxt27YZhQoVMlavXm3MnTvXqFKlivHtt99aXZ6latWqZTz77LPG/v37jd9//924cOFCps1RBQcHG7169TKuX79u+5198uRJ4/HHHze+/vprq8u7IwQnC3Ts2NH46KOPsrRPnz7d6Nixo2EYhjF58mSjRo0aOV2apUqXLm0cOnTI6jJyJQKCfYULFzaOHDliGIZhFC1a1Ni7d69hGIaxa9cuo3z58hZWlvvs2LHD6Nu3r+Hu7m54eXkZr7/+unH48GGry8pRW7duNV566SXDw8PDqF27tvHhhx8aLi4uxr59+6wuLVeoUqWK8cUXXxiG8efnjGEYxjvvvGP06dPHytIs1aZNG6N9+/ZGUlKSUbhwYWP//v3G//73P6NevXrGd999Z3V5lilVqpTxww8/GIZhGEWKFLH9/v7mm2+MRo0aWVma5QoWLGj8/PPPVpeR63h6ehoHDx60/bx//37DMAzj+++/N6pUqWJlaXeMySEssGrVKoWEhGRpb968uVatWiVJatWqlY4dO5bTpVlq4MCBmjRpUpZubUgHDhxQWFiYJClfvny6fPmyChcurJEjR+r999+3uDrrFCpUyDZspnTp0jp69Kht39mzZ60qK9c5ffq01qxZozVr1sjFxUWtWrXSnj17VL16dU2YMMHq8nJEQECAnn32WZUoUUJbtmzRzp07NXDgQIYE3+LkyZN67LHHJEkFChTQH3/8IUl64YUX9OWXX1pZmqXi4uI0cuRIeXl5ydnZWc7OzmrcuLGio6PzxtCi+yQlJUXe3t6SbtyCkJSUJEmqWbOmww/rrF+/vo4cOWJ1GblO/vz55ex8I3p4e3vr5MmTkiRPT0/Fx8dbWdod4x4nCxQvXlzLli3TgAEDMrUvW7ZMxYsXl3TjA6lIkSJWlGeZTZs2af369fq///s/PfLII8qfP3+m/YsXL7aoMuvZCwiPPPKIJMcOCA0aNNCmTZtUrVo1tWrVSgMHDtSePXu0ePFiNWjQwOryLHX16lUtXbpUM2fO1OrVqxUQEKDXX39dXbp0kYeHhyTpv//9r3r06JHls+hBdOjQIXXq1ElPPPGEqlevbnU5uVKpUqV0/vx5lS9fXuXKldP333+vWrVq6fjx4w79hdb169dtv4+9vLx06tQpValSReXLl9ehQ4csrs46VapU0aFDh+Tn56datWrp448/lp+fn6ZPn67SpUtbXZ6l+vXrp4EDByohIUE1a9bM8veMo06cUbt2bW3btk2VK1dWcHCwhg0bprNnz2ru3LmqUaOG1eXdEYKTBd555x317t1b69evV7169SRJ27Zt04oVKzR9+nRJ0po1axQcHGxlmTmuaNGievrpp60uI1ciINg3fvx4Xbp0SZI0YsQIXbp0SQsWLFDlypUddsKMm0qXLq2MjAx17txZW7duVWBgYJZjnnjiCRUtWjTHa7PCsWPHNGvWLPXu3VuXL19W586d1bVrV3qcbtGsWTMtXbpUtWvXVkREhAYMGKBFixZp+/bt6tixo9XlWaZGjRravXu3KlSooPr16+uDDz6Qq6urPvnkE1WsWNHq8izTv39/nT59WpIUFRWlp556SvPnz5erq6tmzZplbXEWe+aZZyRJPXr0sLU5OTnJMAyHnhxi9OjRtp7s9957T2FhYerdu7cqV66sGTNmWFzdnXEyHPlrJAtt3rxZU6dOtX1bVaVKFfXr1882TAK41bFjx3Tp0iUFBAQoJSVFAwcO1JYtW2wBoXz58laXaImrV69m+SbvprNnz8rLyyuHK8o95s6dq2effVbu7u5Wl5LrrFu3TjNmzNDixYt15coVDRo0SC+++KIefvhhq0uzVEZGhjIyMpQv343vVGNiYmyfMy+//LJcXV0trtAaq1atUkpKijp27KgjR46oTZs2Onz4sEqUKKEFCxaoWbNmVpeYK6SmpurgwYMqV66cQ3/2StIvv/xy2/2O+jv7QUBwApBnPfPMM1q0aFGWXoPExEQ1b95ce/futagy5AXJycmaP3++ZsyYoZ07d6pGjRr66aefrC4LecD58+ezXVoEwIOL4GQRFka74dFHH1VsbKyKFSum2rVr3/aXkKPfbIqs6tatq4CAAH3++ee2ttOnT6tZs2Z65JFHtGjRIgurs9727duzXZPHke8ZtGfXrl2aMWOGJk+ebHUpOeqnn35SjRo15OzsbBoaHfW+DNjHovXmWPvrwfs7j3ucLMDCaH9q37693NzcJEkdOnSwtphcpnjx4jp8+LC8vLxMv9k8f/58DlaWe6xYsUKPP/64IiMjNX78eJ06dUpPPPGEatWqpZiYGKvLs1RMTIzCwsIUGhqq1atX68knn9Thw4eVmJjIvYS3uHbtmq5cuaLAwECHC02SFBgYqISEBHl7eyswMNB2H8ZfOdrvpo4dO2rWrFny8PAwvb/LUb+EYNH67B07dkxPP/209uzZk+n/qZvXyJH+X3rQ/s4jOFnglVdeUVBQkJYvX67SpUs79IdNVFSU3Z8hTZgwwTaT08SJE60tJpcqWbKkVq9ercaNG0uSvv32Wz366KOaP3++bcpTRzV69GhNmDBBffr0UZEiRTRp0iRVqFBBL7/8skPOeLVs2TKdO3dO3bt3t7W99957GjVqlK5du6ZmzZppwYIFKlasmHVFWuD48eMqWbKk7Wfc4Onpafvd7OnpaXE1uVNMTIy++uortWrVyupScp3+/furQoUKio2NVYUKFbR161adO3dOAwcO1Icffmh1eTnqQfs7j6F6FihUqJB2794tf39/q0tBHnDt2jV98cUXCg0NlY+Pj9Xl5EqHDx9WkyZN1KJFC82dO9ehv4y4qVChQtq3b5/8/PxUokQJbdiwQTVr1tSBAwfUrFkz22xYjuKJJ57Qv/71L/Xp00eStGXLFjVp0kQjR45UtWrV9Pbbb6tly5YOPxsjcKfKlCmjDRs2OPykKvZ4eXlp3bp1CggIkKenp7Zu3aoqVapo3bp1GjhwoH788UerS8TfRI+TBW4ujEZwyuz69euaMGFCtvdkOOpwtHz58umVV17RgQMHrC4lV8hu2GJqaqqWLVumEiVK2Noc9d+MdOM63Zz2tWzZstq7d69q1qypCxcuKDU11eLqct6+ffsyhaJFixapRYsWevvttyVJ7u7u6t+/v8MFp6VLl97xsY50X8at3n33XXXt2lUVKlSwupRc5eai9VOnTuXLqr9g7a8/3c0kKnnhdzbByQIsjGbfiBEj9Nlnn2ngwIEaOnSo3n77bZ04cUJLlizRsGHDrC7PUvXq1dOPP/7IFKZi2OKdevzxx7VmzRrVrFlTzz77rPr3769169ZpzZo1at68udXl5bg//vgjU6jetGmTnn32WdvjRx55RKdOnbKiNEv99Z6Dv97jdOsfPI50X8atFi5cqKioKNWvX1/dunXTc8895/DTbUssWn87rP31pwftdzZD9Sxg794LFkaTKlWqpMmTJ6t169YqUqSIdu3aZWv7/vvv9cUXX1hdomW++uorDRkyRAMGDFCdOnVUqFChTPsdNWwje+fPn9eVK1dUpkwZZWRk6IMPPrCtyTN06FCHu5fH399f06ZNU2hoqC5duqQSJUpo3bp1atSokaQbszmFhoYqKSnJ4kqts3btWr355psaPXq0GjZsKEmKi4vT0KFDNXr0aLVo0cLiCq2zb98+zZ8/XzExMfr111/VokULde3aVR06dFDBggWtLs8SERERt90/c+bMHKok97nd2l8xMTEO+eXVg4LgZAEWRrOvUKFCOnDggMqVK6fSpUtr+fLlevTRR3Xs2DHVrl1bycnJVpdoGcJ29pjaH3diyJAhWrJkid566y2tWLFCW7Zs0bFjx+Ti4iJJ+uSTTzRnzhxt2rTJ4kqtU6NGDU2fPt022cpN//vf//TSSy8xXPj/27x5s7744gstXLhQV65c0cWLF60uCXkAa39lduXKlSy3ZHh4eFhUzZ1jqJ4FHDUYmXnooYd0+vRplStXTpUqVdLq1av16KOPatu2bbapLB0Vs13Zx9T+2Tt58uRt95crVy6HKskdhg0bpt9++02vvfaaSpUqpXnz5tlCkyR9+eWXatu2rYUVWu/o0aMqWrRolnZPT0+dOHEix+vJrQoVKqQCBQrI1dXVdh8hcKsePXpo0qRJtvucpBtLjKSkpKhfv36aMWOGhdVZJyUlRW+++aa++uornTt3Lsv+vPA7mx4nixw9elQTJ060fYNXvXp19e/fX5UqVbK4MusMHjxYHh4eeuutt7RgwQJ169ZNfn5+OnnypAYMGKAxY8ZYXSJymcDAQD388MMaMWKE3an9HXkaYWdn59t+s5kXfkEhZz3++ONyd3fX3LlzbTN4JiYmKiwsTFeuXNHGjRstrtA6x48f1xdffKEvvvhChw4dUnBwsLp06aJ//etfDv05s2jRomwndMoLi5neLy4uLjp9+rS8vb0ztZ89e1alSpXStWvXLKrMWn369NH69es1atQovfDCC5o2bZp+++03ffzxxxozZoy6du1qdYmm6HGywKpVq9SuXTsFBgbaxtdv3rxZjzzyiJYtW+aw48hvDUadOnVSuXLlFBcXp8qVKzv8N8GSNHfuXE2fPl3Hjx9XXFycypcvr4kTJ6pChQpq37691eVZ4ueff9aiRYuYodKOv053e/XqVf34448aP3683nvvPYuqsk52Q2Q8PT318MMPa9CgQQ772XvTjBkz9PTTT6tcuXLy9fWVJMXHx6ty5cpasmSJtcVZqEGDBtq2bZsCAgIUERGhzp07q2zZslaXZbnJkyfr7bffVvfu3fXNN98oIiJCR48e1bZt22zT/juaixcvyjAMGYahP/74Q+7u7rZ9169f14oVK7KEKUeybNkyzZkzR02bNlVERISaNGkif39/lS9fXvPnz88TwYkeJwvUrl1boaGhWXpQBg8erNWrVzv0tzSw76OPPtKwYcP0+uuv67333tPevXtVsWJFzZo1S7Nnz9b69eutLtESzZo10xtvvKGnnnrK6lLyjOXLl2vs2LHasGGD1aXkqNmzZ9ttv3Dhgnbs2KEFCxZo0aJFDv8ljWEYWrNmjQ4ePChJqlatmkJCQhz6voy3335bXbt2VfXq1a0uJVepWrWqoqKi1LlzZxUpUkS7d+9WxYoVNWzYMJ0/f15Tp061usQcZ9bT7+TkpBEjRtiWQXA0hQsX1v79+1WuXDk99NBDWrx4serVq6fjx4+rZs2aunTpktUlmiI4WcDd3V179uxR5cqVM7UfPnxYAQEBunLlikWVWe/QoUOaMmWKbQhjtWrV1K9fP1WpUsXiyqxVvXp1jR49Wh06dMj0C2rv3r1q2rSpzp49a3WJlvjvf/+roUOH6t///jdT+9+hI0eOqFatWkpJSbG6lFxl/PjxWrRokbZs2WJ1KUCeULBgQR04cEDly5eXt7e31qxZo1q1aunnn39WgwYN7N7D8qDbuHGjDMNQs2bN9PXXX6t48eK2fa6uripfvrzKlCljYYXWCggI0JQpUxQcHKyQkBAFBgbqww8/1OTJk/XBBx/o119/tbpEUwzVs0DJkiW1a9euLMFp165dDt2F+/XXX+v5559XUFCQbSrc77//XjVq1FBMTIyeeeYZiyu0zvHjx1W7du0s7W5ubg79B/DNfxM9evSwtTHb4A1/nenLMAydPn1aw4cPz/LZA6lNmzZ69913rS7DcrGxsYqNjbU7S6Uj3dAeGRmpUaNGqVChQoqMjLztsY62aPJNpUqV0vnz51W+fHmVK1dO33//vWrVqqXjx49nmazHUQQHB0u68Tu7XLlyDt1Ta09ERIR2796t4OBgDR48WG3bttXUqVN19erVPPP/EcHJAr169dJLL72kY8eO6bHHHpN04x6n999/3/QD+kH2xhtvaMiQIRo5cmSm9qioKL3xxhsOHZwqVKigXbt2ZZmRceXKlapWrZpFVVmP2QazV7Ro0Sy/tA3DkK+vr2JiYiyqKvdKS0uTq6ur1WVYasSIERo5cqSCgoLsTrbiSH788UddvXrV9nN2HPkaNWvWTEuXLlXt2rUVERGhAQMGaNGiRdq+fbs6duxodXmWOnDggOLj421T+0+bNk2ffvqpqlevrmnTpjncOno3DRgwwPZzSEiIDh48qB07dsjf3z/PjBBhqJ4FDMPQxIkTNW7cONtK9WXKlNG///1vvfbaaw77QVywYEH99NNPWW70//nnn1WrVi2lpqZaVJn1PvvsMw0fPlzjxo1Tz5499dlnn+no0aOKjo7WZ599pueff97qEpHL/HUGNGdnZ5UsWVL+/v7Kl4/vzP7q9ddf18GDB7Vy5UqrS7FM6dKl9cEHH+iFF16wuhTkARkZGcrIyLB9nsTExNgW2X755Zcd+ouImjVr6v3331erVq20Z88eBQUFaeDAgVq/fr2qVq3q0IsD53UEJwtcvHjRtsjXzTUgbs71f+TIEYedIaxVq1Z69tlns6xGPnPmTMXExGjVqlUWVZY7zJ8/X8OHD9fRo0cl3QjbI0aMUM+ePS2uzHr79++3Ox1uu3btLKoIuU12vfnJycnauXOnDh8+rO+++0516tTJ4cpyjxIlSmjr1q0OvSwGcC8ULlxYe/fulZ+fn4YPH669e/dq0aJF2rlzp1q1aqWEhASrS7TMtm3btH79ervDgfPCcD2+drRA69attXbtWrm5uWVaHO3QoUNq3rx5nrg57n5o166d3nzzTe3YsUMNGjSQdOMep4ULF2rEiBFaunRppmMdTdeuXdW1a1elpqbq0qVLDn0/3E3Hjh3T008/rT179tjubZL+HD7jyPc43fr/y62cnJzk7u4uf39/VahQIYersk52w608PDzUokULLV682KGuhz0vvviivvjiC73zzjtWl2K5uxlqtnjx4vtYSe524cIFbd261e4fwWFhYRZVZT1XV1fbKJm1a9farkXx4sWz3H/qSEaPHq2hQ4eqSpUq8vHxyTTCKq+MtqLHyQItW7aUk5OTli5dauviPnDggJo1a6bnnntOkyZNsrhCazg7O9/RcY5+0z/+1LZtW7m4uOizzz5ThQoVtHXrVp07d04DBw7Uhx9+qCZNmlhdomVuTov714/4WyfPaNy4sZYsWeKw4+2RWf/+/TVnzhwFBAQoICAgyyyVeeHb4HvlryMfbsdRh10tW7ZMXbt21aVLl+Th4ZHlj+Dz589bWJ212rVrp/T0dDVq1EijRo3S8ePHVbZsWa1evVp9+/bV4cOHrS7REj4+Pnr//ffVvXt3q0v52whOFrh8+bJCQkL00EMPKSYmRvv27VPz5s3VtWtXh/rFhDtXu3Ztu9/G3Np70L17dz3xxBMWVGcdLy8vrVu3TgEBAfL09NTWrVtVpUoVrVu3TgMHDrztTd0PutjYWL399tt67733VK9ePUnS1q1b9c4772jo0KHy9PTUyy+/rPr16+vzzz+3uFrkBmafH466Xhzse/jhh9WqVSuNHj1aBQsWtLqcXOXkyZN69dVXFR8fr9dee802pH7AgAG6fv26Jk+ebHGF1ihdurS+++67PD2zK8HJIhcuXFDTpk1VuXJlfffddwoLC9PYsWOtLssScXFxOnfunNq0aWNrmzNnjqKiopSSkqIOHTpoypQpcnNzs7BKaw0ZMkQfffSRatasafsjeNu2bfrpp5/UvXt37d+/X7GxsVq8eLHat29vcbU5p1ixYtq5c6cqVKigSpUq6bPPPtMTTzyho0ePqmbNmg49oUiNGjX0ySef2GbuvGnz5s166aWXtG/fPq1du1Y9evTQyZMnLaoSyDuSkpJ06NAhSVKVKlVUsmRJiyuyVqFChbRnzx5VrFjR6lKQR3zwwQc6deqUJk6caHUpfxv3OOWQv45pdXZ21oIFC9SiRQs988wzeuedd2zH3Jw4wlGMHDlSTZs2tQWnPXv2qGfPnurevbuqVaumsWPHqkyZMho+fLi1hVro7NmzGjhwYJZ7D95991398ssvWr16taKiojRq1CiHCk41atTQ7t27VaFCBdWvX18ffPCBXF1d9cknnzj8L/OjR4/a/Szx8PDQsWPHJEmVK1d22MWT8ac7uZ/HyclJX3/9dQ5Uk/ukpKSoX79+mjNnju0+HhcXF4WFhWnKlCkO29sSGhqq7du3O/xn7U23Tvxldh+To/2dd9OgQYPUunVrVapUSdWrV88yHDgv3C9Ij1MOuXm/wV/dejO7oy7aWbp0aS1btkxBQUGSpLffflsbN27Upk2bJEkLFy5UVFSU9u/fb2WZlvL09LStdXCrI0eOqE6dOkpOTtbBgwdVt25d20yNjmDVqlVKSUlRx44ddeTIEbVp00aHDx9WiRIlFBMTo+bNm1tdomUaN26sIkWKaM6cObZvxpOSkhQWFqaUlBR99913Wrt2rfr06WP7Fh2O6U7v53HUe3lefvllrV27VlOnTlWjRo0kSZs2bdJrr72mFi1a6KOPPrK4wpxz66QzSUlJGjlypCIiIlSzZs0sfwQ72iROLi4uOn36tLy9vW/7N58j/p13U9++fW0jQ/46OYSUNz5j6HHKIYwNz97vv/8uHx8f2+ONGzeqZcuWtsd169ZVfHy8FaXlGu7u7tqyZUuW4LRlyxa5u7tLurGmxs2fHUVoaKjtZ39/fx08eFDnz59XsWLF8swMPffL559/rvbt2+uhhx6Sr6+vJCk+Pl4VK1bUN998I0m6dOmShg4damWZyAXywh8rVvr666+1aNEiNW3a1NbWqlUrFShQQM8995xDBacOHTpkafvrovWSY07itG7dOhUvXtz2s6P/DrJn9uzZ+vrrr9W6dWurS/nbCE45JDg42OoSci0fHx8dP35cvr6+Sk9P186dOzVixAjb/j/++CPLN1mOpl+/fnrllVe0Y8cO1a1bV9KNe5w+++wzvfXWW5Ju9L4EBgZaWGXuULx4cR08eFDt2rVz2JmLpBv3YOzfv1+rV6+2XYcqVaqoRYsWthks7f0RBCCz1NTUTF/u3eTt7e1w91H+dcpx/OnWv/MaNWqU7d8tjjw8unjx4nl+nTiG6lnkf//7nz7++GMdO3ZMCxcuVNmyZTV37lxVqFBBjRs3trq8HNW7d2/t3r1b77//vpYsWaLZs2fr1KlTtlXH58+fr4kTJ2rbtm0WV2qt+fPna+rUqZluTu7Xr5+6dOki6cZsjTdn2XN0u3fv1qOPPupw33gCuPeaN2+uEiVKaM6cObbP18uXLys8PFznz5/X2rVrLa4wZ125ckVr16613Zc8ZMgQpaWl2fbny5dPI0eOdOjfRc8884wWLVqUpdcpMTFRzZs31969ey2qzFozZ87UypUrNXPmzDx7byA9Thb4+uuv9cILL6hr167auXOn7QMnOTlZo0eP1ooVKyyuMGeNGjVKHTt2VHBwsAoXLqzZs2fbQpMkzZgxQ08++aSFFeYONxfAzU6BAgVysBrkBSkpKdq4caNOnjyp9PT0TPtee+01i6oC8pZJkyYpNDRUDz30kGrVqiXpxpczbm5uWr16tcXV5bxZs2Zp+fLltuA0depUPfLII7bfQQcPHlSpUqUUGRlpZZmWOnnypF588cVMSz2cPn1azZo10yOPPGJhZdaaPHmyjh49Kh8fH/n5+WXpldu5c6dFld05epwsULt2bQ0YMEBhYWEqUqSIdu/erYoVK+rHH39Uy5YtlZCQYHWJlkhOTlbhwoXl4uKSqf38+fMqXLhwpjAF3A49TtKPP/6oVq1aKTU1VSkpKSpevLjOnj2rggULytvb2zazHgBzqampmj9/vg4ePChJqlatmrp27eqQX1g1adJEb7zxhtq2bStJmf6OkaR58+Zp2rRpiouLs7JMSyUlJenxxx9Xy5YtNX78eJ06dUpPPPGEatWqpZiYGNtwaUdz620Y9kRFReVQJX8fPU4WOHTokB5//PEs7Z6enrpw4ULOF5RLeHp62m2/ebOloylevLgOHz4sLy8v08kOHHmFdtg3YMAAtW3bVtOnT5enp6e+//575c+fX926dVP//v2tLg/IM86dO6cSJUqoV69eOnnypD777DMdOnRI27dvV5MmTawuL8cdOXJENWvWtD12d3fPFATq1aunPn36WFFarlGyZEmtXr3aduvFt99+q0cffVTz58932NAk5Y1gZIbgZIFSpUrpyJEj8vPzy9S+adMm1kOAzYQJE1SkSBHbz8zQ8yezIHnt2rUcrCZ32rVrlz7++GM5OzvLxcVFaWlpqlixoj744AOFh4ff0do9gCPbs2eP2rZtq/j4eFWuXFkxMTF66qmnlJKSImdnZ02YMEGLFi1yuElWLly4kOmepqSkpEz7MzIyMu13VL6+vlqzZo2aNGmiFi1aaO7cufwe//927NihAwcOSJIeeeQR1a5d2+KK7hzByQK9evVS//79NWPGDDk5OenUqVOKi4vToEGDsixwCscVHh5u+7l79+7WFZIL5eVVx3NK/vz5bd9sent76+TJk6pWrZo8PT0dfnp/4E688cYbqlmzpubPn6+5c+eqTZs2at26tT799FNJN2Y7HTNmjMMFp4ceekh79+5VlSpV7O7/6aef9NBDD+VwVdbL7gu91NRULVu2TCVKlLC1OeookTNnzuj555/Xhg0bVLRoUUk3gvgTTzyhmJgY25qDuRn3OFnAMAyNHj1a0dHRtqlM3dzcNGjQII0aNcri6pCbZLeI3q2cnJzoYUEWTz75pLp3764uXbqoV69e+umnn/Taa69p7ty5+v333/XDDz9YXSKQq3l5eWndunUKCAjQpUuX5OHhoW3btqlOnTqSbkyC0KBBA4cbYt+/f3+tXbtWO3bsyDJz3uXLlxUUFKSQkBBNmjTJogqtMXv27Ds+9tYvRh1Jp06ddOzYMc2ZM0fVqlWTJO3fv1/h4eHy9/fXl19+aXGF5ghOFkpPT9eRI0d06dIlVa9eXYULF7a6JOQyNxcqtScuLk6TJ09WRkaGrly5koNV5U6vvvqqRo4cKS8vL6tLyRW2b9+uP/74Q0888YTOnDmjsLAwbdmyRZUrV9aMGTNss4MBsM/Z2VkJCQny9vaWlHUShMTERJUpU8bhJqFJTExUYGCgXF1d1bdvXz388MOSbty/PXXqVF27dk0//vij3bWv4Ng8PT21du1a23qUN23dulVPPvlknvgSgqF6OahHjx53dNyMGTPucyXIK9q3b5+l7dChQxo8eLCWLVumrl272l213RHNmzdPgwYNIjjpRq+2t7e3atSoIenGUL2VK1daXBWQ9/y1x597VG4sWr9lyxb17t1bgwcP1s3v352cnNSiRQv95z//ITTd4sqVK1mWg/Dw8LCoGmtlZGTYXRg4f/78eWZxZYJTDpo1a5bKly+v2rVri44+3K1Tp04pKipKs2fPVmhoqHbt2mX7wxji/6lbGIYhf39/7du3T5UrV7a6HCDP6t69u9zc3CTd+AP4lVdeUaFChSTJoSdAqFChglauXKnz58/ryJEjkiR/f3+HnQX3r1JSUvTmm2/qq6++0rlz57Lsd7ReypuaNWum/v3768svv1SZMmUkSb/99psGDBig5s2bW1zdnSE45aDevXvryy+/1PHjxxUREaFu3brxIQNTNxdGnjJligIDAxUbG+uQU+Dizjk7O6ty5co6d+4cwQn4m/56H0q3bt2yHBMWFpZT5eRKxYsXV7169awuI9d54403tH79en300Ud64YUXNG3aNP3222/6+OOPNWbMGKvLs8zUqVPVrl07+fn5ydfXV9KNxYJr1qypefPmWVzdneEepxyWlpamxYsXa8aMGdqyZYtat26tnj176sknn2QIALL44IMP9P7776tUqVIaPXq03aF7gD3Lli3TBx98oI8++oieSQDIQeXKldOcOXPUtGlTeXh4aOfOnfL399fcuXP15ZdfasWKFVaXaBnDMLR27VrbYtLVq1fPM71NEsHJUr/88otmzZqlOXPm6Nq1a9q3bx8TRCATZ2dnFShQQCEhIXJxccn2uMWLF+dgVda6ePGibXz4xYsXb3uso44jl25MjZuamqpr167J1dVVBQoUyLTfUafDBYD7rXDhwtq/f7/KlSunhx56SIsXL1a9evV0/Phx1axZU5cuXbK6xBwVFxenc+fOqU2bNra22bNnKyoqSqmpqerQoYOmTJliGxabmzFUz0I3p5o2DMNhx7vi9sLCwuiJ/ItixYrp9OnT8vb2VtGiRe1eH8Mw5OTk5ND/X7HWFQBYo2LFijp+/LjKlSunqlWr6quvvlK9evW0bNky2/pFjmTkyJFq2rSpLTjt2bNHvXr1Unh4uKpVq6axY8eqTJkyGj58uLWF3gF6nHLYrUP1Nm3apDZt2igiIkJPPfWUbbFKANnbuHGjGjVqpHz58mnjxo23PTY4ODiHqgIA4IYJEybIxcVFr732mtauXau2bdvKMAxdvXpV48ePV//+/a0uMUeVLl1ay5YtU1BQkCTp7bff1saNG7Vp0yZJ0sKFCxUVFaX9+/dbWeYdoccpB7366quKiYmRr6+vevTooS+//JKpk4G7dDMMXbt2TRs3blSPHj0ccpX6u8F0uABw/2VkZGjs2LFaunSp0tPTbbPhHjx4UDt27JC/v78CAgKsLjPH/f7775mmqN+4caNatmxpe1y3bl3Fx8dbUdpdo8cpBzk7O6tcuXKqXbv2bYdfOdL9KsA/UaRIEe3Zs0d+fn5Wl5LrMB0uAOSsUaNGafjw4QoJCVGBAgW0atUqde7c2eHX5yxfvrzmzp2rxx9/XOnp6SpatKiWLVtmmxRiz549Cg4OzhP33tLjlIO4XwW4t5o1a6aNGzcSnOxgOlwAyFlz5szRf/7zH7388suSpLVr16p169b67LPPHPp2jFatWmnw4MF6//33tWTJEhUsWDDTsio//fSTKlWqZGGFd44eJwB51vTp0zVixAh17dpVderUsS1MeVO7du0sqsx6TIcLADnLzc1NR44csa1RJEnu7u46cuSIQw8pP3v2rDp27KhNmzapcOHCmj17tp5++mnb/ubNm6tBgwZ67733LKzyzhCcAORZt/sGz9Fn1WM6XADIWS4uLkpISFDJkiVtbUWKFNFPP/2kChUqWFhZ7pCcnKzChQtnWV7l/PnzKly4sFxdXS2q7M4xVA9AnpWRkWF1CbkW0+ECQM4yDEPdu3fPtB7RlStX9Morr2QaEeGo97J7enrabS9evHgOV/L3Oe6ASwB5VlxcnL799ttMbXPmzFGFChXk7e2tl156SWlpaRZVlztERERo9+7dkqTBgwdr2rRpcnd314ABA/Tvf//b4uoA4METHh4ub29veXp62rZu3bqpTJkymdqQdzFUD0Ce07JlSzVt2lRvvvmmpBsz8jz66KPq3r27bTG9l19+OU8spnev/XU63ObNmysqKkpnzpxx6OlwAQD4pwhOAPKcB2kxvXuN6XABALg/GKoHIM95kBbTu9duToe7atUqLVmyRMuWLdP8+fO5HwwAgH+I4AQgz/Hx8dHx48clSenp6dq5c6caNGhg2//HH38of/78VpVnqZMnT6pVq1a2xyEhIXJyctKpU6csrAoAgLyP4AQgz7m5mN7//vc/DRkyJE8vpnevXbt2Te7u7pna8ufPr6tXr1pUEQAADwamIweQ54waNUodO3ZUcHCwbTG9W9d/mDFjhp588kkLK7QO0+ECAHB/MDkEgDzrQVhM716LiIi4o+Nmzpx5nysBAODBQnACAAAAABPc4wQAAAAAJghOAAAAAGCC4AQAAAAAJghOAAAAAGCC4AQAAAAAJghOAIB7pnv37urQoYPVZfwjR44cUY8ePVSuXDm5ubmpbNmyat68uebPn69r165ZXR4AwCIsgAsAwP+3detWhYSE6JFHHtG0adNUtWpVSdL27ds1bdo01ahRQ7Vq1bJ77tWrV5U/f/6cLBcAkIPocQIA3DdNmzZVv3799Prrr6tYsWLy8fHRp59+qpSUFEVERKhIkSLy9/fX//3f/9nOuX79unr27KkKFSqoQIECqlKliiZNmpTpea9du6bXXntNRYsWVYkSJfTmm28qPDw8U29XRkaGoqOjbc9Tq1YtLVq0KNtaDcNQ9+7d9fDDD2vz5s1q27atKleurMqVK6tz587atGmTAgICJEknTpyQk5OTFixYoODgYLm7u2v+/PnKyMjQyJEj9dBDD8nNzU2BgYFauXKl7TU2bNggJycnXbhwwda2a9cuOTk56cSJE5KkWbNmqWjRolqyZIkqV64sd3d3hYaGKj4+/h/8lwAA/FMEJwDAfTV79mx5eXlp69at6tevn3r37q1nn31Wjz32mHbu3Kknn3xSL7zwglJTUyXdCDwPPfSQFi5cqP3792vYsGF666239NVXX9me8/3339f8+fM1c+ZMbd68WRcvXtSSJUsyvW50dLTmzJmj6dOna9++fRowYIC6deumjRs32q1z165dOnDggAYNGiRnZ/u/Hp2cnDI9Hjx4sPr3768DBw4oNDRUkyZN0rhx4/Thhx/qp59+UmhoqNq1a6eff/75rq5Zamqq3nvvPc2ZM0ebN2/WhQsX9Pzzz9/VcwAA7jEDAIB7JDw83Gjfvr3tcXBwsNG4cWPb42vXrhmFChUyXnjhBVvb6dOnDUlGXFxcts/bp08f45lnnrE99vHxMcaOHZvpecuVK2d77StXrhgFCxY0tmzZkul5evbsaXTu3Nnua8TExBiSjJ07d9raEhMTjUKFCtm2adOmGYZhGMePHzckGRMnTsz0HGXKlDHee++9TG1169Y1Xn31VcMwDGP9+vWGJOP333+37f/xxx8NScbx48cNwzCMmTNnGpKM77//3nbMgQMHDEnGDz/8kO01AgDcX9zjBAC4r24Ob5MkFxcXlShRQjVr1rS1+fj4SJLOnDlja5s2bZpmzJihkydP6vLly0pPT1dgYKAkKTk5WYmJiapXr16m561Tp44yMjIk3ZjgITU1VS1atMhUS3p6umrXrn3HtZcoUUK7du2SdGPYYXp6eqb9QUFBtp8vXryoU6dOqVGjRpmOadSokXbv3n3HrylJ+fLlU926dW2Pq1atqqJFi+rAgQOZ3jcAIOcQnAAA99VfJ0xwcnLK1HZz+NvN0BMTE6NBgwZp3LhxatiwoYoUKaKxY8fqhx9+uOPXvHTpkiRp+fLlKlu2bKZ9bm5uds+pXLmyJOnQoUO2cOXi4iJ/f39JN8LMXxUqVOiOa5JkGwJoGIat7erVq3f1HAAAa3CPEwAgV9m8ebMee+wxvfrqq6pdu7b8/f119OhR235PT0/5+Pho27Zttrbr169r586dtsfVq1eXm5ubTp48KX9//0ybr6+v3detXbu2qlatqg8//NAW4u6Gh4eHypQpo82bN2d5P9WrV5cklSxZUpJ0+vRp2/6bPVq3unbtmrZv3257fOjQIV24cEHVqlW767oAAPcGPU4AgFylcuXKmjNnjlatWqUKFSpo7ty52rZtmypUqGA7pl+/foqOjpa/v7+qVq2qKVOm6Pfff7f1XhUpUkSDBg3SgAEDlJGRocaNGys5OVmbN2+Wh4eHwsPDs7yuk5OTZs6cqRYtWqhRo0YaMmSIqlWrpqtXr+q7775TUlKSXFxcblv7v//9b0VFRalSpUoKDAzUzJkztWvXLs2fP1+SbMFt+PDheu+993T48GGNGzcuy/Pkz59f/fr10+TJk5UvXz717dtXDRo0YJgeAFiI4AQAyFVefvll/fjjj+rUqZOcnJzUuXNnvfrqq5mmLH/zzTeVkJCgsLAwubi46KWXXlJoaGimYDNq1CiVLFlS0dHROnbsmIoWLapHH31Ub731Vrav3aBBA+3YsUOjR49Wnz59lJCQoEKFCqlWrVqaMGGCevTocdvaX3vtNSUnJ2vgwIE6c+aMqlevrqVLl9qGAebPn19ffvmlevfurYCAANWtW1fvvvuunn322UzPU7BgQb355pvq0qWLfvvtNzVp0kSff/7537mcAIB7xMm4daA1AAB5UEZGhqpVq6bnnntOo0aNsrqcf2TWrFl6/fXXM631BACwHj1OAIA855dfftHq1asVHBystLQ0TZ06VcePH1eXLl2sLg0A8IBicggAQJ7j7OysWbNmqW7dumrUqJH27NmjtWvXMnkCAOC+YageAAAAAJigxwkAAAAATBCcAAAAAMAEwQkAAAAATBCcAAAAAMAEwQkAAAAATBCcAAAAAMAEwQkAAAAATBCcAAAAAMDE/wMO6Ht5KCihHgAAAABJRU5ErkJggg==
"
class="
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p><a href="https://www.nvidia.com/dli"> <img src="images/combined_logo.png" alt="Header" style="width: 400px;"/> </a></p>

</div>
</div>
</div>
</div>
</body>







</html>