
<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Final Project</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>




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

.highlight  {
  margin: 0.4em;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.CodeMirror pre {
  margin: 0;
  padding: 0;
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
<h1 id="Difference-in-Win-Percentage-Between-Home-and-Away-Games-in-Basketball-Through-the-Years">Difference in Win Percentage Between Home and Away Games in Basketball Through the Years<a class="anchor-link" href="#Difference-in-Win-Percentage-Between-Home-and-Away-Games-in-Basketball-Through-the-Years">&#182;</a></h1><p>Takeshi Sui
12/16/2022</p>

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
<h1 id="Introduction-and-Motivation">Introduction and Motivation<a class="anchor-link" href="#Introduction-and-Motivation">&#182;</a></h1><p>In every sports league, when two teams are set to play against each other, there must be a decision made between which of the two teams' playing field the game is played in. Almost every sports team have a stadium or arena located in the city that the team is based in. For example, the New York Knicks is located in New York City and their sports arena the Madison Square Garden is located in the same city. Similarly, the Los Angeles Lakers is located in Los Angeles and their sports arena the Staples Center is also located in the same city. When a team plays a game in the arena located in their city, it is considered a home game, and when a team plays a game in the opponent team's arena, it is considered an away game. Historically, teams have had a lower winning percentage when playing in the opponent teams' arenas due to reasons including fatigue from travel, worse living accomodations, and lack of fans in the crowd. However, as technology and standard of living have improved through the years, the gap of winning percentages between home and away games have supposedly decreased. It has always fascinated me that a team can play at vastly different skill levels just by being at a different location. I have been wanting to explore more about this topic and see if time has made a difference in this disparity.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">sqlite3</span>
<span class="kn">import</span> <span class="nn">pandas</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">scipy.stats</span> <span class="k">as</span> <span class="nn">stats</span>
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
<h1 id="The-Process">The Process<a class="anchor-link" href="#The-Process">&#182;</a></h1><p><strong>1. The Dataset Used</strong>
The dataset I used comes from Kaggle (<a href="https://www.kaggle.com/datasets/wyattowalsh/basketball">https://www.kaggle.com/datasets/wyattowalsh/basketball</a>) and was compiled by a user named Wyatt Walsh. The dataset contains data from the league's conception in 1946 until 2020 on all nba games, teams, and players including over 60,000 games with box scores, information of current and past teams, and over 4,500 players' information throughout their career. The SQL database includes 16 different tables, but I only used one of these which is the table that includes every game played since 1946. The original dataset includes 149 features, but I am only utilizing five of them in this project:</p>
<ol>
<li>Season ID - the season the game was played in</li>
<li>Team Name Home - the name of the home team that played in the game</li>
<li>WL Home - whether the home team won the game or not (W = win, L = loss)</li>
<li>Team Name Away - the name of the away team that played in the game</li>
<li>WL Away - whether the away team won the game or not (W = win, L = loss)</li>
</ol>
<p><strong>2. Data Loading and Pre-processing</strong>
For this project, I decided to focus on arguably the three most iconic teams in the NBA which are also the teams that have been a part of the league for the longest time: the New York Knicks, the Los Angeles Lakers, and the Boston Celtics. Since all the data is stored in an SQL database, I used a query to get the table I want and store it into a pandas dataframe. Then I removed all the columns that I don't need for this project.</p>

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#create connection to SQL database</span>
<span class="n">sqlite_file</span> <span class="o">=</span> <span class="s1">&#39;basketball.sqlite&#39;</span>
<span class="n">conn</span> <span class="o">=</span> <span class="n">sqlite3</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">sqlite_file</span><span class="p">)</span>

<span class="c1">#Create the query</span>
<span class="n">query</span> <span class="o">=</span> <span class="s2">&quot;SELECT * FROM Game&quot;</span>

<span class="c1">#Store the Game table into a pandas dataframe</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">pandas</span><span class="o">.</span><span class="n">read_sql</span><span class="p">(</span><span class="n">query</span><span class="p">,</span> <span class="n">conn</span><span class="p">)</span>
<span class="n">df</span> <span class="o">=</span> <span class="n">df</span><span class="p">[[</span><span class="s1">&#39;SEASON_ID&#39;</span><span class="p">,</span> <span class="s1">&#39;TEAM_NAME_HOME&#39;</span><span class="p">,</span> <span class="s1">&#39;WL_HOME&#39;</span><span class="p">,</span> <span class="s1">&#39;TEAM_NAME_AWAY&#39;</span><span class="p">,</span> <span class="s1">&#39;WL_AWAY&#39;</span><span class="p">]]</span>

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

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[2]:</div>



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
      <th>SEASON_ID</th>
      <th>TEAM_NAME_HOME</th>
      <th>WL_HOME</th>
      <th>TEAM_NAME_AWAY</th>
      <th>WL_AWAY</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>21946</td>
      <td>Toronto Huskies</td>
      <td>L</td>
      <td>New York Knicks</td>
      <td>W</td>
    </tr>
    <tr>
      <th>1</th>
      <td>21946</td>
      <td>St. Louis Bombers</td>
      <td>W</td>
      <td>Pittsburgh Ironmen</td>
      <td>L</td>
    </tr>
    <tr>
      <th>2</th>
      <td>21946</td>
      <td>Chicago Stags</td>
      <td>W</td>
      <td>New York Knicks</td>
      <td>L</td>
    </tr>
    <tr>
      <th>3</th>
      <td>21946</td>
      <td>Providence Steamrollers</td>
      <td>W</td>
      <td>Boston Celtics</td>
      <td>L</td>
    </tr>
    <tr>
      <th>4</th>
      <td>21946</td>
      <td>Detroit Falcons</td>
      <td>L</td>
      <td>Washington Capitols</td>
      <td>W</td>
    </tr>
  </tbody>
</table>
</div>
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
<p>Thankfully, there are no missing values in our dataset, so we can go straight into organizing our data. I first created a dictionary for each of the three teams to store the number of wins and losses in their home and away games each season. Notice that the Lakers didn't become a team in the NBA until 1948 so I had to delete the first two elements of the dictionary.</p>
<p>The next step is to simply iterate through the dataframe and count the number of wins and losses for each team. It is important to note that in 1960, the Lakers basketball team moved from the city of Minneapolis to Los Angeles which is where they are now. As a result, the official team name changed from the Minneapolis Lakers to the Los Angeles Lakers. To take this into account I simply checked if the team name contained the string "lakers" since the name "lakers" remained the same before and after the move.</p>

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1">#Initialize dictionaries for all three teams</span>
<span class="n">lakers</span> <span class="o">=</span> <span class="p">{}</span>
<span class="n">celtics</span> <span class="o">=</span> <span class="p">{}</span>
<span class="n">knicks</span> <span class="o">=</span> <span class="p">{}</span>

<span class="k">for</span> <span class="n">season</span> <span class="ow">in</span> <span class="n">df</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">():</span>
    <span class="n">lakers</span><span class="o">.</span><span class="n">update</span><span class="p">({</span><span class="n">season</span><span class="p">:</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">]})</span>
    <span class="n">celtics</span><span class="o">.</span><span class="n">update</span><span class="p">({</span><span class="n">season</span><span class="p">:</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">]})</span>
    <span class="n">knicks</span><span class="o">.</span><span class="n">update</span><span class="p">({</span><span class="n">season</span><span class="p">:</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">]})</span>
    
<span class="c1">#Delete the first two years when Lakers haven&#39;t been formed</span>
<span class="k">del</span> <span class="n">lakers</span><span class="p">[</span><span class="s2">&quot;21946&quot;</span><span class="p">]</span>
<span class="k">del</span> <span class="n">lakers</span><span class="p">[</span><span class="s2">&quot;21947&quot;</span><span class="p">]</span>

<span class="c1">#Count number of wins and losses for each team each season</span>
<span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">df</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
    <span class="k">if</span> <span class="s2">&quot;Lakers&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_HOME&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_HOME&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">lakers</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">lakers</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="k">elif</span> <span class="s2">&quot;Lakers&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_AWAY&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_AWAY&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">lakers</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">lakers</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">3</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
            
    <span class="k">if</span> <span class="s2">&quot;Celtics&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_HOME&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_HOME&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">celtics</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">celtics</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="k">elif</span> <span class="s2">&quot;Celtics&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_AWAY&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_AWAY&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">celtics</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">celtics</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">3</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
            
    <span class="k">if</span> <span class="s2">&quot;Knicks&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_HOME&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_HOME&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">knicks</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">knicks</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
    <span class="k">elif</span> <span class="s2">&quot;Knicks&quot;</span> <span class="ow">in</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;TEAM_NAME_AWAY&quot;</span><span class="p">]:</span>
        <span class="k">if</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;WL_AWAY&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;W&quot;</span><span class="p">:</span>
            <span class="n">knicks</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="n">knicks</span><span class="p">[</span><span class="n">row</span><span class="p">[</span><span class="s2">&quot;SEASON_ID&quot;</span><span class="p">]][</span><span class="mi">3</span><span class="p">]</span> <span class="o">+=</span> <span class="mi">1</span>
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
<p>Finally, now that we have information on the number of wins and losses for home and away games for each season the three teams existed in the NBA, we can calculate the win percentages of each of the teams when they played at home vs when they played in away games. For each team, I iterated through the dictionary created in the previous step, and for each season, I took the number wins and divided it by the total number of games they played. I did this for both the home and away games. I also calculated the difference in win percentage between home and away games for each season. I did this by simply taking the win percentage at home and subtracting it by the win percentage at away games.</p>
<p>Here I calculate the win percentages for the New York Knicks:</p>

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">knicks_home</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">knicks_away</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">knicks_difference</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">knicks_years</span> <span class="o">=</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1946</span><span class="p">,</span> <span class="mi">2021</span><span class="p">)</span>

<span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">knicks</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
    <span class="n">knicks_home</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">knicks_away</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">knicks_difference</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">-</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">))</span>
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
<p>Here I calculate the win percentages for the Boston Celtics:</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">celtics_home</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">celtics_away</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">celtics_difference</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">celtics_years</span> <span class="o">=</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1946</span><span class="p">,</span> <span class="mi">2021</span><span class="p">)</span>

<span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">celtics</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
    <span class="n">celtics_home</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">celtics_away</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">celtics_difference</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">-</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">))</span>
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
<p>Here I calculated the win percentages for the Los Angeles Lakers (Previously the Minneapolis Lakers):</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">lakers_home</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">lakers_away</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">lakers_difference</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">lakers_years</span> <span class="o">=</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1948</span><span class="p">,</span> <span class="mi">2021</span><span class="p">)</span>

<span class="k">for</span> <span class="n">n</span> <span class="ow">in</span> <span class="n">lakers</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
    <span class="n">lakers_home</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">lakers_away</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span>
    <span class="n">lakers_difference</span><span class="o">.</span><span class="n">append</span><span class="p">((</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">)</span> <span class="o">-</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="p">(</span><span class="n">n</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="n">n</span><span class="p">[</span><span class="mi">3</span><span class="p">])</span> <span class="o">*</span> <span class="mi">100</span><span class="p">))</span>
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
<p><strong>3. Exploratory Data Analysis</strong>
After preprocessing and organizing our data, we can now create graphs and charts to be able to visualize our data better. To start off, I created double bar graphs for each team with one bar displaying the win percentage at home and one bar displaying the win percentage at away games. There is a pair of bars for each season that the team played in the NBA.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X_axis</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">knicks_years</span><span class="p">))</span>
    
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Knicks Away and Home Game Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season Since 1946&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">-</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">knicks_home</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Home&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">+</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">knicks_away</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Away&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">loc</span><span class="o">=</span><span class="s2">&quot;upper right&quot;</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[7]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>&lt;matplotlib.legend.Legend at 0x1f4d9771820&gt;</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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7Ut3drov6i/ub/bP6Yad/U+S89O9XuukD7AHpguNP0n3+n8gXQ/P6pyerif4yyPzvtzPm3QvXVprn0h38JkT+tfz3HRDe1d3+2+mPxhHup6z03NrL+wh6ULG+em2m49mZPjrGrwj3Xv76qp6Z7p9xj6d5Ifp2ufXWXmI5d+m2y5/km4b+Gi68LWu7XBErXyeuiv7+WvaPl6V5Jx0Pa4/T/darsv3o82TfCLd/nw/TveaPqV/Ppek6y18bbrwdkm6A9VsNMbnxn3SvT7XpzvAz3taa6e11n7TP/4T070+70lyyEhvMbCAVPcdCIC50vdY3Le1dpuACQtVVb043UFIxu0ZBKCnpw5gDvVDKZ+X5P3TrgWmqap2qKp9+2Ge90vXC/+JadcFMERCHcAcqar/k27Y1adbaxMflgfz3B3SHV3zunTnjzwp634gJYAFzfBLAACAAdNTBwAAMGBCHQAAwIBtMu0CxrHddtu1JUuWTLsMAACAqTjrrLOubK1tv6plgwh1S5YsyZlnnjntMgAAAKaiqi5a3TLDLwEAAAZMqAMAABgwoQ4AAGDABrFPHQAAsDDceOONWbZsWX79619Pu5SpWLRoUXbcccdsuummY99HqAMAAOaNZcuWZcstt8ySJUtSVdMuZ0611nLVVVdl2bJl2Xnnnce+n+GXAADAvPHrX/8622677YILdElSVdl2223XupdSqAMAAOaVhRjoVliX5y7UAQAAjNhiiy1Wmj7mmGPykpe8ZErVrJl96gAAgHlryZGnrNfHW3r0Aev18eYDPXUAAABjuuiii7L//vtn9913z/7775+LL744SXLYYYflxS9+cR7zmMdkl112yemnn54/+ZM/yf3vf/8cdthht9z/1FNPzd57752HPOQhOeigg3L99dff7pqEOgAAgBG/+tWvsscee9xyed3rXnfLspe85CU55JBD8r3vfS/Petazcvjhh9+y7Oqrr84Xv/jFvO1tb8uBBx6YV7ziFTnvvPNyzjnn5Oyzz86VV16ZN77xjfn85z+fb3/729lzzz3z1re+9XbXa/glAADAiM022yxnn332LdPHHHNMzjzzzCTJ1772tXz84x9PkjznOc/JEUccccvtDjzwwFRVdtttt9z1rnfNbrvtliR5wAMekKVLl2bZsmU5//zzs++++yZJfvOb32Tvvfe+3fUKdQAAAOto9GiVd7zjHZMkG2200S3XV0zfdNNN2XjjjfO4xz0uxx9//HqtwfBLAACAMe2zzz454YQTkiTHHXdcHvnIR45937322itf+cpXcuGFFyZJfvnLX+aHP/zh7a5JqAMAABjTO9/5znz4wx/O7rvvno985CN5xzveMfZ9t99++xxzzDF5xjOekd133z177bVXvv/979/umqq1drsfZNL23HPPtmIMKwAAsOG64IILcv/733/aZUzVql6Dqjqrtbbnqm6vpw4AAGDAhDoAAIABE+oAAAAGzCkNAICpWnLkKStNLz36gClVAjBMeuoAAAAGTKgDAAAYMKEOAABghk984hOpqvVyHrlJs08dAAAwfx21eD0/3vKxbnb88cfnkY98ZE444YQcddRR67eG9UxPHQAAwIjrr78+X/nKV/LBD34wJ5xwQm6++ebssssuaa3lmmuuyUYbbZQzzjgjSbLffvvlwgsvzDe/+c3ss88+efCDH5x99tknP/jBD25ZfvbZZ9/y2Pvuu2++973vrdd69dSxVhyhDACADd0nP/nJPOEJT8h973vfbLPNNvnud7+b+973vjn//PPzk5/8JA996EPzpS99KY94xCOybNmy3Pve9861116bM844I5tsskk+//nP57WvfW0+9rGP5fnPf36OOeaYvP3tb88Pf/jD3HDDDdl9993Xa7166gAAAEYcf/zxOfjgg5MkBx98cI4//vjst99+OeOMM3LGGWfkNa95Tb785S/nW9/6Vh72sIclSZYvX56DDjooD3zgA/OKV7wi5513XpLkoIMOyqc+9anceOON+dCHPpTDDjtsvderpw4AAKB31VVX5Ytf/GLOPffcVFVuvvnmVFU+8pGP5H3ve18uvfTS/O3f/m3e8pa35LTTTsujHvWoJMlf//Vf5zGPeUw+8YlPZOnSpXn0ox+dJNl8883zuMc9LieddFJOPPHEnHnmmeu9Zj11AAAAvY9+9KM55JBDctFFF2Xp0qW55JJLsvPOOydJvvrVr2ajjTbKokWLsscee+R973tf9ttvvyRdT93d7373JMkxxxyz0mM+//nPz+GHH56HPexh2WabbdZ7zUIdAABA7/jjj88f/uEfrjTv6U9/ek444YTstNNO2WuvvZJ0B0C57rrrsttuuyVJjjjiiLzmNa/Jvvvum5tvvnml+z/0oQ/NVlttlec+97kT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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X_axis</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">celtics_years</span><span class="p">))</span>
    
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Celtics Away and Home Game Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season Since 1946&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">-</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">celtics_home</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Home&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">+</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">celtics_away</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Away&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">loc</span><span class="o">=</span><span class="s2">&quot;upper right&quot;</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[8]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>&lt;matplotlib.legend.Legend at 0x1f4d7c63d90&gt;</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA3sAAAHwCAYAAAAfJXbRAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjUuMSwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/YYfK9AAAACXBIWXMAAAsTAAALEwEAmpwYAAA4Q0lEQVR4nO3de5gkZX33//eHBVkQ5LgSZMEFxQMCoizIUTFEg0GEHIiICqiEGA94SnDxiboxkh+P5mc8RKPGAwQRJIpCJFEUA4hnEJCzEl1gA3JmAVFg4fv8UTXQO8zMzu5MT8/UvF/X1dd0VVdXfburu6c/fd91V6oKSZIkSVK3rDHoAiRJkiRJk8+wJ0mSJEkdZNiTJEmSpA4y7EmSJElSBxn2JEmSJKmDDHuSJEmS1EGGPUkzTpIFSSrJmmMsc2+SbaayrpkqyRFJLhh0HbNdkncl+cyg69D4JDkhyfsHXYckjcWwJ2lgkhya5MI2mN2U5L+S7LUa6zk3yZG986pqvar65eRVu8K27kyy9mSvezoaLVhPpy+6SQ5J8qMkv0lyS3v9DUky4Lq+meSYnukt2udypHm/V1X/UFVHjry2lW7rhCQPtO+lO5J8K8kzJuNxTIYk+yRZOqBtD72G7x12efkU1/G6JFcnuSfJzUnOSrL+VNYgafYx7EkaiCRvBz4M/AOwGbAV8AngwAGWNaYkC4C9gQJeNthqBJDkHcBHgA8Cv0fzWno9sCfwuAGWBnA+8IKe6ecDV48w7xdV9etJ2N4Hqmo9YD5wC3DCqq5grNbyDtiw/RFo6PKlqdpwkhfQfNa9oqrWB54JnDZV25c0exn2JE25JBsA7wPeWFWnV9VvqurBqvqPqvqbdpk1kixK8j9Jbk9yWpKNR1jXcTQB7J/bX+v/uZ1fSZ7aXl8nyf+f5Loky5Jc0M6bm+QL7frvSvKTJJuNUfphwA9pvkQf3lPDiW3o6G2peUM7/dS2pSVJNkry9SS3tq2DX08yv13u4CQXDXts70jytVGew9ckuaptJfhlkr/suW2fJEvb+9/Stpq+puf2TZKcmeTuJD8GnjLGYx6XJC9LckX7PJ6b5Jk9ty1J8jdJfta2vn02yWZpWnLvSfLtJBv1LL9bku+367o0yT6jbHPodfSGqvpyVd1TjYur6pVVdX+73P5JLm4f7w1JFvesY6jV5zXtbXcmeX2SXdp67xp6TfXc57Xtc39nmta7J4/ytJwP7Jlk6H/t3jQ/cCwcNu/8dr2Lk3xhWF2HJ7k+yW1J/s949kVV3Qd8Edi+XdeTknylfd39KsnRPY9lcZIvt++Du4Ejkmyc5PNJbmwf49d6ln9pkkva5+X7SXbsuW1Jkr9un7dlSb7UvsceD/wX8KQ82qr2pCS7JvlBu66bkvxzksf1rO/FSa5p1/WJJOelpwV/FfbDmMZ6fbS379XzerwhyRE9N2+UpoXunjQtyqO9l3YBflBVFwNU1R1VdWJV3dNuY+0k/9ju65uTfDLJOu1tG2WUz4329iPSfAbc0+7fV7bz10jyt2k+925J8m/te2ZCry9JM0xVefHixcuUXoD9gOXAmmMs81aaYDUfWBv4FHBKe9sCmta1Ndvpc4Ejh92/gKe21z/eLrMFMAfYo13nXwL/Aazbzt8ZeMIYNV0LvKFd7kFgs3b+a4H/aK8fCvwP8KWe285or28C/Gm7vfWBfwe+1t62NnAH8Mye7V0M/OkotexPE9JC01J0H/Dc9rZ92uf3fcBawB+1t2/U3n4qTavC42kCwf8CF4yynRWe6575JwDvb68/DfgN8KJ2e8e0z9Xj2tuXtPtys3Yf3AL8FHhO+7i/A7y3XXYL4Pa25jXadd4OzFud11HP87FDu74dgZuBg4Y9vk8Cc4EXA78DvgY8safeF7TLH9Q+tmcCawJ/C3x/lO2uDfwWeE47fTmwDfC9YfMOa68vBr4wrK5/BdYBng3c3/v6GGN/rEcT9r7bPuaLgPfQtHRuA/wS+MOebT7YPq412m2dBXwJ2Kjdn0OP/bntc/E8mvfL4e2+XbtnP/8YeBKwMXAV8PqefbB0WM07A7u1z+OCdvm3trdtCtwN/El7+1vaOo9cjf0w9FyO+Dph7NfHVsA9wCva52ITYKee5/wOYNe2hpOBU0fZxt7ta+HvaFqd1x52+4eBM9vnbX2az6X/bxyfG49vn6ent9ObA8/q+ey5tt3n6wGnAyetzuvLixcvM/cy8AK8ePEy+y7AK4Ffr2SZq4B9e6Y3b7/srckqhL32C9xvgWePsI3XAt8HdhxHzXu129+0nb4aeFt7/SnAXe22PkkTIpe2t50IvH2Ude4E3Nkz/S/Ace31ZwF3Dv9SOEZ9XwPe0l7fp33Ma/bcfgvNF+s57eN4Rs9t/8DKw95dwy4P8Gi4eDdwWs991qAJkPu000uAV/bc/hXgX3qm38yjX17fOfSFtOf2bwKHj1Dbq4a/jtr9eVf7+J8/ymP6MPBPwx7fFj233w68fFi9b22v/xfwumGP9T7gyaNs61yaoLJxz2vi+J55Dw/dl5HD3vyedf0YOGSU7ZxAE1LvAn5NExyeQhPMrh+27LHA53u2ef6w99nDtD8MDLvfvwB/P2zeNTwaBpcAr+q57QPAJ3tek0tHqr1n+bcCX22vH0bTEjZ0W4AbeDTsjXs/MPpreLTg3Pv6OHaoplGe88/0TP8RcPUYj+8lNCHuLuBe4EM078fQ/FjylJ5ldwd+Ncp6dqL93KAJe3fRhMF1hi13Dk2r99D003nsZ+i4Xl9evHiZuRe7cUoahNuBTTP28UFPBr7adp26iyb8PUTTOrQqNqVpsfmfEW47iSZInNp2WftAkrVGWc/hwNlVdVs7/cV2HlX1PzRf3nai+QX/68CNSZ5O0+p2HkCSdZN8qu1WdTdN970Nk8xp13kicGiSAK+mCVD3j1RMkpck+WGaLqJ30XzR3LRnkdurannP9H00v+7Po/myd0PPbdeN8ph7bVpVGw5d2sc/5Em966iqh9v1b9GzzM091387wvR67fUnAwcP7ff2se1FE0KGe8zrqKr2aOu7nfZQhSTPS/LfbTe4ZTTH9G06bF2rUt9Hemq7g+bLeu9j7XU+zXF5ewNDI55e0DPvhqoa6/nvPZZvaB+O5h/b/fN7VfWy9nX5ZJruk73P57tY8X3U+1rYErijqu4cYf1PBt4xbF1b0uz/Va43ydPaLom/bt8P/8Cj++VJvXVVVQG9A7ys6n6AYa/hqrqqrWOs18eWjPzZscqPt6r+q6oOoAn5BwJHAEfSvCfXBS7qeTzfaOeP+blRVb8BXt7WfFPbpXRoYJ4V3pft9TVZcd+vyutL0gxk2JM0CD+gaYU4aIxlbgBeMuzL2dyq+t8Rlq0x1nNbu63HHEtTzXGCf1dV29F07XwpTYvCCtpjZ/4ceEH7xfTXwNuAZyd5drvYecCf0XRd/N92+jCarnCXtMu8g+bX9edV1RNovvBD8yWVqvohTYvZ3jTdQU8a6QGlGQn0K8A/0nQl3RD4z6H1rMStNF0ft+yZt9U47jeWG2m+fA/Vl3b9I+2rlbmBpmWvd78/vqqOH2HZH9B0PTtwJev8Ik1L15ZVtQFN6+vqjtR5A/CXw+pbp6q+P8ry59Psz+fTdKuEphvnnu2881ezjlWp91fD6l2/qv6oZ5katvzGSTYcZV3HDVvXulV1yjjqGOk9+i80LeTbtu+Hd/HofrmJpgs38Mhran7PfVd1P4xlrNfHDUzCMa29qurhqjqHpvvy9jSfUb+l6X459Fg2qGawHVj558Y3q+pFND+IXE3TNROGvS9p3ufLWfGHDEkdZ9iTNOWqahnNMUQfT3JQ+8v1Wm1r1QfaxT4JHDc06EKSeUlG+1J/M81xKSNt62Hgc8CH0gwKMSfJ7u2ACC9MskPbsnY3TRenh0ZYzUHt/O1oWu92ojlW6Ls8Gg7PA97Eo1/ez6XpnnhBVQ2tc32aL3V3pRls5r0jbOvfgH8GllfVaOe+exzN8WC3AsuTvITmWLOVams5HVjcPu/b0TPYzGo6Ddg/yb5ty+g7aELY6nzx/gJwQJI/bPfV3DQDzswfvmBV3UVzDNQnkvxZkvXaQSl2ouneNmR9mtaq3yXZlSZIr65PAscmeRY0g8QkOXiM5b8PbEjT5fS7bd130uy7V9H/sPdj4O4k70wzKNGcJNsn2WWkhavqJpoukp9IMzDIWkmGwsW/Aq9vW8KS5PFpBjcZz+kDbgY2GRogpLU+zfvu3rY16q96bjsL2KH9fFgTeCPNaKtDVnU/jGWs18fJwB8k+fMka6YZ3GinVd1AkgPTnCJko/a525Wm1f+H7WfUvwL/lOSJ7fJbJPnDnvpG/NxIM9DRy9IMgnM/TQ+Doc+bU4C3Jdk6yXo0LadfGtbiL6njDHuSBqKqPgS8nWZghVtpfkF/E82xZ9AMp38mcHaSe2gG+HjeKKv7CPBnaUaq++gIt/81cBnwE5ruXv+X5vPv94Av03zhvIomsH1hhPsfTnOM0/VV9euhC00oe2X7ZfQ8mi9lQ1/eL6DpmtX7Zf7DNIMh3NY+nm+MsK2TaH7tH7FVD6CaEfyOpglZd9J8OT1ztOVH8Caa7lq/pjnu6POrcN+R6rmGJrh8jOaxHQAcUFUPrMa6bqBpqXsXj74u/oZR/l9V1QdoXkfH0ByXeDPNYD7v5NGw+Qbgfe3r6D1MYMj7qvoqzevn1LZL3eU0x2KNtvx9NAOkrN0uO+S7NAPA9DXsteH+AJofKH5Fs38+A2wwxt1eTfPDx9U0z+lb23VdCPwFzev+TprBP44YZx1X04SPX7ZdFZ9E8748lGYAlH+lGRRmaPnbgINpjvu7neaHlgtpAs0q74fWXVnxPHtvb+eP+vqoqutpuki/g+az4xKawUxW1Z00z90vaD5vvgB8sKpObm9/J83z+cP28XybpjUPxv7cWKOt7ca2vhe0jweaH7lOonmN/Yqmh8ObV6N2STNYmm7wkqTpoO0yegvNyJq/GHQ90nSQ5lQVS2kG+vnvQdcjSTOFLXuSNL38FfATg55mu7Yr74btMapDx/P9cMBlSdKMMtZIeJKkKZRkCc0X2oMGW4k0LexOM3jK44Arac5999vBliRJM4vdOCVJkiSpg+zGKUmSJEkdZNiTJEmSpA6a0cfsbbrpprVgwYJBlyFJkiRJA3HRRRfdVlXzRrptRoe9BQsWcOGFFw66DEmSJEkaiCTXjXab3TglSZIkqYMMe5IkSZLUQYY9SZIkSeqgGX3MniRJkqTZ4cEHH2Tp0qX87ne/G3QpAzF37lzmz5/PWmutNe77GPYkSZIkTXtLly5l/fXXZ8GCBSQZdDlTqqq4/fbbWbp0KVtvvfW479e3bpxJPpfkliSX98zbOMm3kvyi/btRz23HJrk2yTVJ/rBfdUmSJEmaeX73u9+xySabzLqgB5CETTbZZJVbNft5zN4JwH7D5i0CzqmqbYFz2mmSbAccAjyrvc8nkszpY22SJEmSZpjZGPSGrM5j71vYq6rzgTuGzT4QOLG9fiJwUM/8U6vq/qr6FXAtsGu/apMkSZKkVbXeeuutMH3CCSfwpje9aUDVrNxUH7O3WVXdBFBVNyV5Yjt/C+CHPcstbec9RpKjgKMAttpqqz6WKkmSJGm6WrDorEld35Lj95/U9U0H0+XUCyO1SdZIC1bVp6tqYVUtnDdvXp/LkiRJkqSVu+6669h3333Zcccd2Xfffbn++usBOOKII/irv/orXvjCF7LNNttw3nnn8drXvpZnPvOZHHHEEY/c/+yzz2b33Xfnuc99LgcffDD33nvvhGua6rB3c5LNAdq/t7TzlwJb9iw3H7hximuTJEmSpFH99re/Zaeddnrk8p73vOeR2970pjdx2GGH8bOf/YxXvvKVHH300Y/cduedd/Kd73yHf/qnf+KAAw7gbW97G1dccQWXXXYZl1xyCbfddhvvf//7+fa3v81Pf/pTFi5cyIc+9KEJ1zvV3TjPBA4Hjm//ntEz/4tJPgQ8CdgW+PEU1yZJkiRJo1pnnXW45JJLHpk+4YQTuPDCCwH4wQ9+wOmnnw7Aq1/9ao455phHljvggANIwg477MBmm23GDjvsAMCznvUslixZwtKlS7nyyivZc889AXjggQfYfffdJ1xv38JeklOAfYBNkywF3ksT8k5L8jrgeuBggKq6IslpwJXAcuCNVfVQv2qTJEmSpH7qHT1z7bXXBmCNNdZ45PrQ9PLly5kzZw4vetGLOOWUUya1hn6OxvmKqtq8qtaqqvlV9dmqur2q9q2qbdu/d/Qsf1xVPaWqnl5V/9WvuiRJkiRpsu2xxx6ceuqpAJx88snstdde477vbrvtxve+9z2uvfZaAO677z5+/vOfT7im6TJAiyRJkiTNWB/96Ef5/Oc/z4477shJJ53ERz7ykXHfd968eZxwwgm84hWvYMcdd2S33Xbj6quvnnBNqRpx0MsZYeHChTXUR1aSJElSd1111VU885nPHHQZAzXSc5DkoqpaONLytuxJkiRJUgcZ9iRJkiSpgwx7kiRJktRBU32ePUmS1GPBorNWmF5y/P4DqkSS1DW27EmSJElSBxn2JEmSJKmDDHuSJEmSNE5f/epXSTIp58HrN4/ZkyRJkjTzLN5gkte3bFyLnXLKKey1116ceuqpLF68eHJrmGS27EmSJEnSONx7771873vf47Of/SynnnoqDz30ENtssw1VxV133cUaa6zB+eefD8Dee+/Ntddey49//GP22GMPnvOc57DHHntwzTXXPHL7JZdc8si699xzT372s59Nar2GPUmSJEkah6997Wvst99+PO1pT2PjjTfm0ksv5WlPexpXXnklF1xwATvvvDPf/e53uf/++1m6dClPfepTecYznsH555/PxRdfzPve9z7e9a53AXDkkUdywgknAPDzn/+c+++/nx133HFS6zXsSZIkSdI4nHLKKRxyyCEAHHLIIZxyyinsvffenH/++Zx//vkce+yxXHDBBfzkJz9hl112AWDZsmUcfPDBbL/99rztbW/jiiuuAODggw/m61//Og8++CCf+9znOOKIIya9Xo/ZkyRJkqSVuP322/nOd77D5ZdfThIeeughknDSSSfxqU99ihtvvJH3ve99fPCDH+Tcc8/l+c9/PgDvfve7eeELX8hXv/pVlixZwj777APAuuuuy4te9CLO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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[9]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">X_axis</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">lakers_years</span><span class="p">))</span>
    
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Lakers Away and Home Game Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season Since 1948&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">-</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">lakers_home</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Home&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">bar</span><span class="p">(</span><span class="n">X_axis</span> <span class="o">+</span> <span class="mf">0.2</span><span class="p">,</span> <span class="n">lakers_away</span><span class="p">,</span> <span class="mf">0.4</span><span class="p">,</span> <span class="n">label</span> <span class="o">=</span> <span class="s1">&#39;Away&#39;</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">legend</span><span class="p">(</span><span class="n">loc</span><span class="o">=</span><span class="s2">&quot;upper right&quot;</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[9]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>&lt;matplotlib.legend.Legend at 0x1f4d7ac7d00&gt;</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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krDTTjux+eabs9NOOwHwpCc9icWLF7NkyRKuuOIK9tprLwDuvvtu9thjjzWu17AnSZIkSROs9+yZD3/4wwFYa6217r+/Yvree+9l7bXX5rnPfS6nnnrqhNYwLJdekCRJkqRpa8899+S0004D4JRTTuGZz3xm38/dfffdueCCC7jmmmsA+O1vf8tPfvKTNa7JsCdJkiRJa+iDH/wgn/70p9l55505+eST+cAHPtD3c2fPns2JJ57IoYceys4778zuu+/OVVddtcY1pWrUa5dPC/PmzasVY2QlSZIkddeVV17JDjvsMOgyBmq09yDJhVU1b7Tl7dmTJEmSpA4y7EmSJElSBxn2JEmSJKmDvPTCgM2df+aDphcff8CAKpEkSZLUJfbsSZIkSVIHGfYkSZIkqYMMe5IkSZLUpy996UskmZDr4E02j9mTJEmSNP0s2HiC17e8r8VOPfVUnvnMZ3LaaaexYMGCia1hgtmzJ0mSJEl9uOOOO7jgggv45Cc/yWmnncZ9993HtttuS1Vx2223sdZaa3HeeecBsPfee3PNNdfwwx/+kD333JOnPvWp7Lnnnlx99dX3P75o0aL7173XXntxySWXTGi9hj1JkiRJ6sOXv/xl9t9/fx7/+Mez6aabcvHFF/P4xz+eK664gvPPP59dd92V7373u9x1110sWbKE7bbbjic+8Ymcd955/PjHP+Zd73oXb3/72wF4zWtew4knngjAT37yE+666y523nnnCa3XsCdJkiRJfTj11FM55JBDADjkkEM49dRT2XvvvTnvvPM477zzOOaYYzj//PP50Y9+xG677QbA8uXLOfjgg3nyk5/Mm970Ji6//HIADj74YL72ta9xzz338KlPfYojjjhiwuv1mD1JkiRJWombb76Z73znO1x22WUk4b777iMJJ598Mh/72MdYunQp73rXu3jve9/LOeecw7Oe9SwA3vGOd7DvvvvypS99icWLF7PPPvsAsP766/Pc5z6Xr3zlK5x++uksXLhwwmu2Z0+SJEmSVuLzn/88hx12GNdeey2LFy/m+uuvZ5tttgHge9/7HmuttRazZs1il1124WMf+xh777030PTsbbXVVgD3D9tc4TWveQ1HHXUUu+22G5tuuumE12zYkyRJkqSVOPXUU3nxi1/8oHl/+qd/ymmnncbWW2/N7rvvDjQnXvn1r3/NTjvt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
"
class="
jp-needs-light-background
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
<p>Looking at these graphs, we can clearly see that for all three teams, the winning percentage at home is much higher on average than the winning percentage at away games. It is interesting to note that the for the last couple of years, especially in 2020, the Los Angeles Lakers actually had a higher winning percentage at away games than home games. A very plausible explanation for this could be that a portion of that season's games were played at the Disney resort in Orlando, Florida due to the pandemic. Toward the end of the season, every nba team that still had a chance to make playoffs were brought together inside a bubble where they would play the remaining games that season in the same arena without in person attendance by fans.</p>
<p>Overall, we can definitely see that early on in the 40s, 50s, 60s, and even the 70s, the discrepancy between the winning percentages of home and away games was very high. If we compare that to season in the 2000s and 2010s, we can see that in more recent seasons, there is less of a discrepancy between the winning at home vs away.</p>
<p>To more accurately and visually represent this information, I created a scatterplot for each team where every plot represents the difference in winning percentage between home and away games that season. For each plot I added a regression line to see the overall trend.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[10]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Difference in Knicks Away and Home Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Difference in Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">knicks_years</span><span class="p">,</span> <span class="n">knicks_difference</span><span class="p">,</span> <span class="s1">&#39;o&#39;</span><span class="p">)</span>
<span class="n">m</span><span class="p">,</span> <span class="n">b</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">polyfit</span><span class="p">(</span><span class="n">knicks_years</span><span class="p">,</span> <span class="n">knicks_difference</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">knicks_years</span><span class="p">,</span> <span class="n">m</span><span class="o">*</span><span class="n">knicks_years</span><span class="o">+</span><span class="n">b</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[10]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>[&lt;matplotlib.lines.Line2D at 0x1f4ce4e2e50&gt;]</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Difference in Celtics Away and Home Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Difference in Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">celtics_years</span><span class="p">,</span> <span class="n">celtics_difference</span><span class="p">,</span> <span class="s1">&#39;o&#39;</span><span class="p">)</span>
<span class="n">m</span><span class="p">,</span> <span class="n">b</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">polyfit</span><span class="p">(</span><span class="n">celtics_years</span><span class="p">,</span> <span class="n">celtics_difference</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">celtics_years</span><span class="p">,</span> <span class="n">m</span><span class="o">*</span><span class="n">celtics_years</span><span class="o">+</span><span class="n">b</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[11]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>[&lt;matplotlib.lines.Line2D at 0x1f4cd9701c0&gt;]</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
"
>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[12]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span> <span class="o">=</span> <span class="p">(</span><span class="mi">15</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">&#39;Difference in Lakers Away and Home Win Percentage Each Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">&#39;Difference in Win Percentage (%)&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">&#39;Season&#39;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">lakers_years</span><span class="p">,</span> <span class="n">lakers_difference</span><span class="p">,</span> <span class="s1">&#39;o&#39;</span><span class="p">)</span>
<span class="n">m</span><span class="p">,</span> <span class="n">b</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">polyfit</span><span class="p">(</span><span class="n">lakers_years</span><span class="p">,</span> <span class="n">lakers_difference</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">lakers_years</span><span class="p">,</span> <span class="n">m</span><span class="o">*</span><span class="n">lakers_years</span><span class="o">+</span><span class="n">b</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[12]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>[&lt;matplotlib.lines.Line2D at 0x1f4d702b4c0&gt;]</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
class="
jp-needs-light-background
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
<p>In all three plots, there is a clear negative trend between the difference in winning percentage over the years. The difference in winning percentage ranged from 30 to 50 in the mid 1900s while in the 2000s to 2010s, the difference in winning percentage ranged from 0 to 20.</p>
<p><strong>4. Hypothesis Testing</strong>
For the last part of this project, we will use hypothesis testing to formally conclude if there was a significant enough difference in the winning percentage between home and away games. More crucially, we want to see if the difference in winning percentage have signficantly changed from the start of the NBA to the current NBA.</p>
<p>To start off, we want to first test if there is a signficant enough difference in winning percentage between home and away games. To perform this test, I used paired T-test since we have the same sample, but we are taking data from two different categories: games played at home and games played away. I performed this test once for the first 20 years of the NBA and once for the last 10 years of the NBA. For both tests, I combined the data for all three teams. Note that for the Lakers, I only did the first 18 years since they were not a part of the league in 1946 and 1947.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[13]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">past_home</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">past_away</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">past_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_home</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_home</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_home</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">18</span><span class="p">])</span>
<span class="n">past_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_away</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_away</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_away</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">18</span><span class="p">])</span>

<span class="n">stats</span><span class="o">.</span><span class="n">ttest_rel</span><span class="p">(</span><span class="n">past_home</span><span class="p">,</span> <span class="n">past_away</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[13]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>Ttest_relResult(statistic=18.88947090772941, pvalue=3.285894870937929e-26)</pre>
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
<p>After doing the test for the first 20 years of the NBA, we get an astronomically small p-value. Even if we choose a significance level of 0.01 for this test, we are still able to reject the null hypothesis that there is not a significant difference between winning percentages at home vs at away games.</p>

</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[14]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">present_home</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">present_away</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">present_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_home</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>
<span class="n">present_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_home</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>
<span class="n">present_home</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_home</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>
<span class="n">present_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_away</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>
<span class="n">present_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_away</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>
<span class="n">present_away</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_away</span><span class="p">[</span><span class="o">-</span><span class="mi">10</span><span class="p">:])</span>

<span class="n">stats</span><span class="o">.</span><span class="n">ttest_rel</span><span class="p">(</span><span class="n">present_home</span><span class="p">,</span> <span class="n">present_away</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[14]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>Ttest_relResult(statistic=6.76598792246629, pvalue=1.9955753002962043e-07)</pre>
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
<p>For the last 10 years of the NBA, although we get a pvalue that is larger, it is still exponentially smaller than a value of 0.01 if we set that as our significance level. So we also reject the null hypothesis here that there is not a significant difference between winning percentages at home vs at away games.</p>
<p>Although we have concluded that there is in fact a significant difference between winning percentages at home vs away, we need to see if this difference has changed over the years. To do this, we are going to take the difference in winning percentage of the first 20 years of the league and compare to the difference in winning percentage of the last 20 years of the league. Here, we are going to perform a two sample T-test as opposed to a paired T-test because our data is no longer one-to-one paired, but it is from two different samples.</p>

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
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">past_difference</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">present_difference</span> <span class="o">=</span> <span class="p">[]</span>

<span class="n">past_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_difference</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_difference</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">20</span><span class="p">])</span>
<span class="n">past_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_difference</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="mi">18</span><span class="p">])</span>
<span class="n">present_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">knicks_difference</span><span class="p">[</span><span class="o">-</span><span class="mi">20</span><span class="p">:])</span>
<span class="n">present_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">celtics_difference</span><span class="p">[</span><span class="o">-</span><span class="mi">20</span><span class="p">:])</span>
<span class="n">present_difference</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">lakers_difference</span><span class="p">[</span><span class="o">-</span><span class="mi">20</span><span class="p">:])</span>

<span class="n">stats</span><span class="o">.</span><span class="n">ttest_ind</span><span class="p">(</span><span class="n">a</span><span class="o">=</span><span class="n">past_difference</span><span class="p">,</span> <span class="n">b</span><span class="o">=</span><span class="n">present_difference</span><span class="p">,</span> <span class="n">equal_var</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
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

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[15]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>Ttest_indResult(statistic=9.250212061951238, pvalue=1.3560781445309718e-15)</pre>
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
<p>After performing this test, we once again get an astronomically low pvalue. So finally, we are able to reject the null hypothesis that there is no signficant difference between difference in winning percentage at home and away games in the past vs now.</p>

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
<h1 id="Conclusion">Conclusion<a class="anchor-link" href="#Conclusion">&#182;</a></h1><p>In the end, we have found that as time passed, the discrepancy between winning percentage at home vs winning percentage at away games have in fact decreased. In this project, we first obtained a dataset, then processed it, made calculations, visualized the information, performed hypothesis testing, and finally came to a conclusion. There is a lot of nuance in sports and only when we analyze the data do we get to visualize the signficance in the small details.</p>

</div>
</div>
</div>
</div>
</body>







</html>
