<!DOCTYPE html>

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Notebook</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
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
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
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

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
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
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

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

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

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
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
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
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
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
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
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

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
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

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
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

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
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

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
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

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
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

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
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

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
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

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
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

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

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

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

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

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
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

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
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

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
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
  padding: 0 12px;
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

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
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
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
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
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
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
  z-index: 8;
  overflow-x: hidden;
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
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
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

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
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

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
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
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
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

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
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
  padding-bottom: 0;
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
  padding: 0 9px;
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
  padding: 5px 5px 1px;
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
  margin-top: 0;
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

.lm-CommandPalette-content:empty::after {
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
  padding: 0 8px;
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
  top: 0;
  left: 0;
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
  padding: 24px 24px 12px;
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

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
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
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
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
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

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

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

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
  --md-purple-A700: #a0f;
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
  --md-yellow-A200: #ff0;
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
  --md-grey-200: #eee;
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
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

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
  margin: 0;
  padding: 0;
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

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

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
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

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
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
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
  padding: 0.5em;
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

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
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
  font-size: var(--jp-ui-font-size0);
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

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
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
  border-radius: 0;
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

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
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

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
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

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
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

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
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

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
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

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
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

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
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
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
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

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
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
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
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
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
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

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
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
  margin: 0;
  padding: 0;
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

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
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
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
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
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
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
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
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
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
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
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

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

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
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
  margin: 0;
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
  padding: 0;
  margin: 0;

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
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
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

:root {
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
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

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

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

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

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

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
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

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
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
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
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
  margin: 4px 4px 4px 0;
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
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
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

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
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
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
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
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
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
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
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
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

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
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
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

  --jp-inverse-layout-color0: #111;
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
  --jp-cell-prompt-letter-spacing: 0;
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
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
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
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
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

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

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

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
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

.cm-editor.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
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

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@page {
    margin: 0.5in; /* Margin for each printed piece of paper */
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
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
                messageStyle: 'none',
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
<!-- End of mathjax configuration --><script type="module">
  document.addEventListener("DOMContentLoaded", async () => {
    const diagrams = document.querySelectorAll(".jp-Mermaid > pre.mermaid");
    // do not load mermaidjs if not needed
    if (!diagrams.length) {
      return;
    }
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.7.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      maxEdges: 100000,
      startOnLoad: false,
      fontFamily: window
        .getComputedStyle(document.body)
        .getPropertyValue("--jp-ui-font-family"),
      theme: document.querySelector("body[data-jp-theme-light='true']")
        ? "default"
        : "dark",
    });

    let _nextMermaidId = 0;

    function makeMermaidImage(svg) {
      const img = document.createElement("img");
      const doc = parser.parseFromString(svg, "image/svg+xml");
      const svgEl = doc.querySelector("svg");
      const { maxWidth } = svgEl?.style || {};
      const firstTitle = doc.querySelector("title");
      const firstDesc = doc.querySelector("desc");

      img.setAttribute("src", `data:image/svg+xml,${encodeURIComponent(svg)}`);
      if (maxWidth) {
        img.width = parseInt(maxWidth);
      }
      if (firstTitle) {
        img.setAttribute("alt", firstTitle.textContent);
      }
      if (firstDesc) {
        const caption = document.createElement("figcaption");
        caption.className = "sr-only";
        caption.textContent = firstDesc.textContent;
        return [img, caption];
      }
      return [img];
    }

    async function makeMermaidError(text) {
      let errorMessage = "";
      try {
        await mermaid.parse(text);
      } catch (err) {
        errorMessage = `${err}`;
      }

      const result = document.createElement("details");
      result.className = 'jp-RenderedMermaid-Details';
      const summary = document.createElement("summary");
      summary.className = 'jp-RenderedMermaid-Summary';
      const pre = document.createElement("pre");
      const code = document.createElement("code");
      code.innerText = text;
      pre.appendChild(code);
      summary.appendChild(pre);
      result.appendChild(summary);

      const warning = document.createElement("pre");
      warning.innerText = errorMessage;
      result.appendChild(warning);
      return [result];
    }

    async function renderOneMarmaid(src) {
      const id = `jp-mermaid-${_nextMermaidId++}`;
      const parent = src.parentNode;
      let raw = src.textContent.trim();
      const el = document.createElement("div");
      el.style.visibility = "hidden";
      document.body.appendChild(el);
      let results = null;
      let output = null;
      try {
        let { svg } = await mermaid.render(id, raw, el);
        svg = cleanMermaidSvg(svg);
        results = makeMermaidImage(svg);
        output = document.createElement("figure");
        results.map(output.appendChild, output);
      } catch (err) {
        parent.classList.add("jp-mod-warning");
        results = await makeMermaidError(raw);
        output = results[0];
      } finally {
        el.remove();
      }
      parent.classList.add("jp-RenderedMermaid");
      parent.appendChild(output);
    }


    /**
     * Post-process to ensure mermaid diagrams contain only valid SVG and XHTML.
     */
    function cleanMermaidSvg(svg) {
      return svg.replace(RE_VOID_ELEMENT, replaceVoidElement);
    }


    /**
     * A regular expression for all void elements, which may include attributes and
     * a slash.
     *
     * @see https://developer.mozilla.org/en-US/docs/Glossary/Void_element
     *
     * Of these, only `<br>` is generated by Mermaid in place of `\n`,
     * but _any_ "malformed" tag will break the SVG rendering entirely.
     */
    const RE_VOID_ELEMENT =
      /<\s*(area|base|br|col|embed|hr|img|input|link|meta|param|source|track|wbr)\s*([^>]*?)\s*>/gi;

    /**
     * Ensure a void element is closed with a slash, preserving any attributes.
     */
    function replaceVoidElement(match, tag, rest) {
      rest = rest.trim();
      if (!rest.endsWith('/')) {
        rest = `${rest} /`;
      }
      return `<${tag} ${rest}>`;
    }

    void Promise.all([...diagrams].map(renderOneMarmaid));
  });
</script>
<style>
  .jp-Mermaid:not(.jp-RenderedMermaid) {
    display: none;
  }

  .jp-RenderedMermaid {
    overflow: auto;
    display: flex;
  }

  .jp-RenderedMermaid.jp-mod-warning {
    width: auto;
    padding: 0.5em;
    margin-top: 0.5em;
    border: var(--jp-border-width) solid var(--jp-warn-color2);
    border-radius: var(--jp-border-radius);
    color: var(--jp-ui-font-color1);
    font-size: var(--jp-ui-font-size1);
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  .jp-RenderedMermaid figure {
    margin: 0;
    overflow: auto;
    max-width: 100%;
  }

  .jp-RenderedMermaid img {
    max-width: 100%;
  }

  .jp-RenderedMermaid-Details > pre {
    margin-top: 1em;
  }

  .jp-RenderedMermaid-Summary {
    color: var(--jp-warn-color2);
  }

  .jp-RenderedMermaid:not(.jp-mod-warning) pre {
    display: none;
  }

  .jp-RenderedMermaid-Summary > pre {
    display: inline-block;
    white-space: normal;
  }
</style>
<!-- End of mermaid configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=32efb7ab">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="Supply-Chain-Emissions-Modeling-Using-Industry-and-Commodity-Data-(2010%E2%80%932016)">Supply Chain Emissions Modeling Using Industry and Commodity Data (2010–2016)<a class="anchor-link" href="#Supply-Chain-Emissions-Modeling-Using-Industry-and-Commodity-Data-(2010%E2%80%932016)">¶</a></h1>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=a7c1c6fc">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Problem Statement:</p>
<p>You have annual supply chain emission data from 2010–2016 categorized into industries and commodities. The goal is to develop a regression model that can predict the Supply Chain Emission Factors with Margins based on descriptive and quality metrics (substance, unit, reliability, temporal/geographical/technological/data collection correlations, etc.).</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=0eae1c80">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="%F0%9F%8C%B1-Greenhouse-Gas-Emission-Prediction-Project">🌱 Greenhouse Gas Emission Prediction Project<a class="anchor-link" href="#%F0%9F%8C%B1-Greenhouse-Gas-Emission-Prediction-Project">¶</a></h1><p><img alt="GHG Emissions" src="https://www.shalom-education.com/wp-content/uploads/2022/12/Shutterstock_1667551381-1-1024x1006.jpg"/></p>
<p><strong>Project Goal:</strong><br/>
To analyze and predict greenhouse gas (GHG) emissions from various U.S. industries and commodities using the official dataset from <a href="https://catalog.data.gov/dataset/supply-chain-greenhouse-gas-emission-factors-for-us-industries-and-commodities">data.gov</a>.</p>
<p><img alt="GHG Emissions" src="https://edg.epa.gov/EPALogo.svg"/></p>
<p><strong>Source:</strong><br/>
<a href="https://catalog.data.gov/dataset/supply-chain-greenhouse-gas-emission-factors-for-us-industries-and-commodities">Supply Chain Greenhouse Gas Emission Factors</a></p>
<p><strong>Tools:</strong> Python, Pandas, Scikit-learn, Matplotlib, Seaborn</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=d2cc9ed5">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="%F0%9F%93%82-Dataset-Overview">📂 Dataset Overview<a class="anchor-link" href="#%F0%9F%93%82-Dataset-Overview">¶</a></h2><p>This dataset contains supply chain emission factors associated with various U.S. industries and commodities.</p>
<p><strong>Key Columns:</strong></p>
<ul>
<li><code>Code</code>: Industry classification code</li>
<li><code>Industry_Name</code>: Name of the industry</li>
<li><code>Commodity</code>: Item or commodity name</li>
<li><code>GHG_Emissions_kgCO2e</code>: GHG emissions per unit (kg CO2 equivalent)</li>
<li><code>Units</code>: Measurement units (e.g., [kg/2018 USD, purchaser price])</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=409dc066">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="%F0%9F%A7%B9-Data-Preprocessing">🧹 Data Preprocessing<a class="anchor-link" href="#%F0%9F%A7%B9-Data-Preprocessing">¶</a></h2><p>Steps:</p>
<ul>
<li>Handle missing values</li>
<li>Convert units where needed</li>
<li>Encode categorical features</li>
<li>Normalize/scale numeric columns</li>
</ul>
<h2 id="%F0%9F%A4%96-Model-Building-&amp;-Evaluation">🤖 Model Building &amp; Evaluation<a class="anchor-link" href="#%F0%9F%A4%96-Model-Building-&amp;-Evaluation">¶</a></h2><p>We aim to predict <code>GHG_Emissions_kgCO2e</code> using regression models.</p>
<p>Models to try:</p>
<ul>
<li>Linear Regression</li>
<li>Random Forest</li>
</ul>
<p><strong>Evaluation Metrics:</strong></p>
<ul>
<li>RMSE (Root Mean Squared Error)</li>
<li>MAE (Mean Absolute Error)</li>
<li>R² Score</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=c2558455">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Steps:">Steps:<a class="anchor-link" href="#Steps:">¶</a></h5><ul>
<li>Step 1: Import Required Libraries</li>
<li>Step 2: Load Dataset</li>
<li>Step 3: Data Preprocessing (EDA+Cleaning+Encoding)</li>
<li>Step 4: Training</li>
<li>Step 5: Prediction and Evaluation</li>
<li>Step 6: Hyperparameter Tuning</li>
<li>Step 7: Comapartive Study and Slecting the Best model</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=118424af">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="Step-1:-Import-Required-Libraries">Step 1: Import Required Libraries<a class="anchor-link" href="#Step-1:-Import-Required-Libraries">¶</a></h1>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=a2e58624">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [1]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="kn">import</span><span class="w"> </span><span class="nn">pandas</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">pd</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">numpy</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">np</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">seaborn</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">sns</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">matplotlib.pyplot</span><span class="w"> </span><span class="k">as</span><span class="w"> </span><span class="nn">plt</span>

<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.model_selection</span><span class="w"> </span><span class="kn">import</span> <span class="n">train_test_split</span><span class="p">,</span> <span class="n">GridSearchCV</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.preprocessing</span><span class="w"> </span><span class="kn">import</span> <span class="n">StandardScaler</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.ensemble</span><span class="w"> </span><span class="kn">import</span> <span class="n">RandomForestRegressor</span>
<span class="kn">from</span><span class="w"> </span><span class="nn">sklearn.metrics</span><span class="w"> </span><span class="kn">import</span> <span class="n">mean_squared_error</span><span class="p">,</span> <span class="n">r2_score</span>
<span class="kn">import</span><span class="w"> </span><span class="nn">joblib</span>
</pre></div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=c670b39a">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="Step-2:-Load-Dataset">Step 2: Load Dataset<a class="anchor-link" href="#Step-2:-Load-Dataset">¶</a></h1>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=3d7223e5">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [2]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">excel_file</span> <span class="o">=</span> <span class="s1">'SupplyChainEmissionFactorsforUSIndustriesCommodities.xlsx'</span>  <span class="c1"># Replace with actual path</span>
<span class="n">years</span> <span class="o">=</span> <span class="nb">range</span><span class="p">(</span><span class="mi">2010</span><span class="p">,</span> <span class="mi">2017</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=aba2c82e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [3]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">years</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[3]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>2010</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=3739f73a">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [4]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df_1</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">excel_file</span><span class="p">,</span> <span class="n">sheet_name</span><span class="o">=</span><span class="sa">f</span><span class="s1">'</span><span class="si">{</span><span class="n">years</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">_Detail_Commodity'</span><span class="p">)</span>
<span class="n">df_1</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[4]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Commodity Code</th>
<th>Commodity Name</th>
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>Unnamed: 7</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.398</td>
<td>0.073</td>
<td>0.470</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
<tr>
<th>1</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>methane</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.001</td>
<td>0.001</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>1</td>
<td>1</td>
</tr>
<tr>
<th>2</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>nitrous oxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
<tr>
<th>3</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>3</td>
<td>3</td>
<td>1</td>
<td>3</td>
<td>1</td>
</tr>
<tr>
<th>4</th>
<td>1111B0</td>
<td>Fresh wheat, corn, rice, and other grains</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.659</td>
<td>0.081</td>
<td>0.740</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=b3da39b5">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [5]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df_2</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">excel_file</span><span class="p">,</span> <span class="n">sheet_name</span><span class="o">=</span><span class="sa">f</span><span class="s1">'</span><span class="si">{</span><span class="n">years</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">_Detail_Industry'</span><span class="p">)</span>
<span class="n">df_2</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[5]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Industry Code</th>
<th>Industry Name</th>
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>Unnamed: 7</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>1111A0</td>
<td>Oilseed farming</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.414</td>
<td>0.073</td>
<td>0.487</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
<tr>
<th>1</th>
<td>1111A0</td>
<td>Oilseed farming</td>
<td>methane</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.001</td>
<td>0.001</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>1</td>
<td>1</td>
</tr>
<tr>
<th>2</th>
<td>1111A0</td>
<td>Oilseed farming</td>
<td>nitrous oxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
<tr>
<th>3</th>
<td>1111A0</td>
<td>Oilseed farming</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>3</td>
<td>3</td>
<td>1</td>
<td>3</td>
<td>1</td>
</tr>
<tr>
<th>4</th>
<td>1111B0</td>
<td>Grain farming</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.680</td>
<td>0.082</td>
<td>0.762</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=464213c7">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [6]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">all_data</span> <span class="o">=</span> <span class="p">[]</span>

<span class="k">for</span> <span class="n">year</span> <span class="ow">in</span> <span class="n">years</span><span class="p">:</span>
    <span class="k">try</span><span class="p">:</span>
        <span class="n">df_com</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">excel_file</span><span class="p">,</span> <span class="n">sheet_name</span><span class="o">=</span><span class="sa">f</span><span class="s1">'</span><span class="si">{</span><span class="n">year</span><span class="si">}</span><span class="s1">_Detail_Commodity'</span><span class="p">)</span>
        <span class="n">df_ind</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_excel</span><span class="p">(</span><span class="n">excel_file</span><span class="p">,</span> <span class="n">sheet_name</span><span class="o">=</span><span class="sa">f</span><span class="s1">'</span><span class="si">{</span><span class="n">year</span><span class="si">}</span><span class="s1">_Detail_Industry'</span><span class="p">)</span>
        
        <span class="n">df_com</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span> <span class="o">=</span> <span class="s1">'Commodity'</span>
        <span class="n">df_ind</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span> <span class="o">=</span> <span class="s1">'Industry'</span>
        <span class="n">df_com</span><span class="p">[</span><span class="s1">'Year'</span><span class="p">]</span> <span class="o">=</span> <span class="n">df_ind</span><span class="p">[</span><span class="s1">'Year'</span><span class="p">]</span> <span class="o">=</span> <span class="n">year</span>
        
        <span class="n">df_com</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">df_com</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>
        <span class="n">df_ind</span><span class="o">.</span><span class="n">columns</span> <span class="o">=</span> <span class="n">df_ind</span><span class="o">.</span><span class="n">columns</span><span class="o">.</span><span class="n">str</span><span class="o">.</span><span class="n">strip</span><span class="p">()</span>

        <span class="n">df_com</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">{</span>
            <span class="s1">'Commodity Code'</span><span class="p">:</span> <span class="s1">'Code'</span><span class="p">,</span>
            <span class="s1">'Commodity Name'</span><span class="p">:</span> <span class="s1">'Name'</span>
        <span class="p">},</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
        
        <span class="n">df_ind</span><span class="o">.</span><span class="n">rename</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">{</span>
            <span class="s1">'Industry Code'</span><span class="p">:</span> <span class="s1">'Code'</span><span class="p">,</span>
            <span class="s1">'Industry Name'</span><span class="p">:</span> <span class="s1">'Name'</span>
        <span class="p">},</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
        
        <span class="n">all_data</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">pd</span><span class="o">.</span><span class="n">concat</span><span class="p">([</span><span class="n">df_com</span><span class="p">,</span> <span class="n">df_ind</span><span class="p">],</span> <span class="n">ignore_index</span><span class="o">=</span><span class="kc">True</span><span class="p">))</span>
        
    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">"Error processing year </span><span class="si">{</span><span class="n">year</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">"</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=4079554d-36f7-4163-b1af-f8fddcdc1c65">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [7]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">all_data</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[7]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Code</th>
<th>Name</th>
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>Unnamed: 7</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
<th>Source</th>
<th>Year</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.373</td>
<td>0.072</td>
<td>0.444</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2013</td>
</tr>
<tr>
<th>1</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>methane</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.001</td>
<td>0.001</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>Commodity</td>
<td>2013</td>
</tr>
<tr>
<th>2</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>nitrous oxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2013</td>
</tr>
<tr>
<th>3</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>3</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2013</td>
</tr>
<tr>
<th>4</th>
<td>1111B0</td>
<td>Fresh wheat, corn, rice, and other grains</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.722</td>
<td>0.079</td>
<td>0.801</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2013</td>
</tr>
<tr>
<th>...</th>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
<td>...</td>
</tr>
<tr>
<th>3151</th>
<td>813B00</td>
<td>Civic, social, professional, and similar organ...</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.008</td>
<td>0.000</td>
<td>0.008</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>5</td>
<td>1</td>
<td>Industry</td>
<td>2013</td>
</tr>
<tr>
<th>3152</th>
<td>814000</td>
<td>Private households</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.000</td>
<td>0.000</td>
<td>0.000</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>5</td>
<td>1</td>
<td>Industry</td>
<td>2013</td>
</tr>
<tr>
<th>3153</th>
<td>814000</td>
<td>Private households</td>
<td>methane</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.000</td>
<td>0.000</td>
<td>0.000</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>5</td>
<td>1</td>
<td>Industry</td>
<td>2013</td>
</tr>
<tr>
<th>3154</th>
<td>814000</td>
<td>Private households</td>
<td>nitrous oxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.000</td>
<td>0.000</td>
<td>0.000</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>5</td>
<td>1</td>
<td>Industry</td>
<td>2013</td>
</tr>
<tr>
<th>3155</th>
<td>814000</td>
<td>Private households</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.000</td>
<td>0.000</td>
<td>0.000</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>5</td>
<td>1</td>
<td>Industry</td>
<td>2013</td>
</tr>
</tbody>
</table>
<p>3156 rows × 15 columns</p>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=a4ddac28">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [8]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">len</span><span class="p">(</span><span class="n">all_data</span><span class="p">)</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[8]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>7</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d99bcf77">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [9]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">concat</span><span class="p">(</span><span class="n">all_data</span><span class="p">,</span> <span class="n">ignore_index</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[9]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Code</th>
<th>Name</th>
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>Unnamed: 7</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
<th>Source</th>
<th>Year</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.398</td>
<td>0.073</td>
<td>0.470</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2010</td>
</tr>
<tr>
<th>1</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>methane</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.001</td>
<td>0.001</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>Commodity</td>
<td>2010</td>
</tr>
<tr>
<th>2</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>nitrous oxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2010</td>
</tr>
<tr>
<th>3</th>
<td>1111A0</td>
<td>Fresh soybeans, canola, flaxseeds, and other o...</td>
<td>other GHGs</td>
<td>kg CO2e/2018 USD, purchaser price</td>
<td>0.002</td>
<td>0.000</td>
<td>0.002</td>
<td>NaN</td>
<td>3</td>
<td>3</td>
<td>1</td>
<td>3</td>
<td>1</td>
<td>Commodity</td>
<td>2010</td>
</tr>
<tr>
<th>4</th>
<td>1111B0</td>
<td>Fresh wheat, corn, rice, and other grains</td>
<td>carbon dioxide</td>
<td>kg/2018 USD, purchaser price</td>
<td>0.659</td>
<td>0.081</td>
<td>0.740</td>
<td>NaN</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>Commodity</td>
<td>2010</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=333b762c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [10]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">len</span><span class="p">(</span><span class="n">df</span><span class="p">)</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[10]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>22092</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=12443c98">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="Step-3:-Data-Preprocessing">Step 3: Data Preprocessing<a class="anchor-link" href="#Step-3:-Data-Preprocessing">¶</a></h1>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=0912c587">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [11]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span> <span class="c1"># Checking columns</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[11]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Index(['Code', 'Name', 'Substance', 'Unit',
       'Supply Chain Emission Factors without Margins',
       'Margins of Supply Chain Emission Factors',
       'Supply Chain Emission Factors with Margins', 'Unnamed: 7',
       'DQ ReliabilityScore of Factors without Margins',
       'DQ TemporalCorrelation of Factors without Margins',
       'DQ GeographicalCorrelation of Factors without Margins',
       'DQ TechnologicalCorrelation of Factors without Margins',
       'DQ DataCollection of Factors without Margins', 'Source', 'Year'],
      dtype='object')</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=3e9957db">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [12]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">isnull</span><span class="p">()</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[12]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Code                                                          0
Name                                                          0
Substance                                                     0
Unit                                                          0
Supply Chain Emission Factors without Margins                 0
Margins of Supply Chain Emission Factors                      0
Supply Chain Emission Factors with Margins                    0
Unnamed: 7                                                22092
DQ ReliabilityScore of Factors without Margins                0
DQ TemporalCorrelation of Factors without Margins             0
DQ GeographicalCorrelation of Factors without Margins         0
DQ TechnologicalCorrelation of Factors without Margins        0
DQ DataCollection of Factors without Margins                  0
Source                                                        0
Year                                                          0
dtype: int64</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=4eb85b0a">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="Week-2---23-June-2025---S4F">Week 2 - 23 June 2025 - S4F<a class="anchor-link" href="#Week-2---23-June-2025---S4F">¶</a></h2>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=7ced9ceb">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [13]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># As there is no data avaialble in Unnamed coulmn so we will drop the column</span>
<span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">'Unnamed: 7'</span><span class="p">],</span><span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d4adb54b">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [14]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[14]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Index(['Code', 'Name', 'Substance', 'Unit',
       'Supply Chain Emission Factors without Margins',
       'Margins of Supply Chain Emission Factors',
       'Supply Chain Emission Factors with Margins',
       'DQ ReliabilityScore of Factors without Margins',
       'DQ TemporalCorrelation of Factors without Margins',
       'DQ GeographicalCorrelation of Factors without Margins',
       'DQ TechnologicalCorrelation of Factors without Margins',
       'DQ DataCollection of Factors without Margins', 'Source', 'Year'],
      dtype='object')</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c48cbbe3">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [15]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">())</span>   <span class="c1"># Checking data types and non-null counts </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 22092 entries, 0 to 22091
Data columns (total 14 columns):
 #   Column                                                  Non-Null Count  Dtype  
---  ------                                                  --------------  -----  
 0   Code                                                    22092 non-null  object 
 1   Name                                                    22092 non-null  object 
 2   Substance                                               22092 non-null  object 
 3   Unit                                                    22092 non-null  object 
 4   Supply Chain Emission Factors without Margins           22092 non-null  float64
 5   Margins of Supply Chain Emission Factors                22092 non-null  float64
 6   Supply Chain Emission Factors with Margins              22092 non-null  float64
 7   DQ ReliabilityScore of Factors without Margins          22092 non-null  int64  
 8   DQ TemporalCorrelation of Factors without Margins       22092 non-null  int64  
 9   DQ GeographicalCorrelation of Factors without Margins   22092 non-null  int64  
 10  DQ TechnologicalCorrelation of Factors without Margins  22092 non-null  int64  
 11  DQ DataCollection of Factors without Margins            22092 non-null  int64  
 12  Source                                                  22092 non-null  object 
 13  Year                                                    22092 non-null  int64  
dtypes: float64(3), int64(6), object(5)
memory usage: 2.4+ MB
None
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=bc6edbcd">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [18]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">describe</span><span class="p">()</span><span class="o">.</span><span class="n">T</span> <span class="c1"># Checking summary statistics </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[18]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>count</th>
<th>mean</th>
<th>std</th>
<th>min</th>
<th>25%</th>
<th>50%</th>
<th>75%</th>
<th>max</th>
</tr>
</thead>
<tbody>
<tr>
<th>Supply Chain Emission Factors without Margins</th>
<td>22092.0</td>
<td>0.084807</td>
<td>0.267039</td>
<td>0.0</td>
<td>0.0</td>
<td>0.002</td>
<td>0.044</td>
<td>7.228</td>
</tr>
<tr>
<th>Margins of Supply Chain Emission Factors</th>
<td>22092.0</td>
<td>0.012857</td>
<td>0.078720</td>
<td>0.0</td>
<td>0.0</td>
<td>0.000</td>
<td>0.000</td>
<td>3.349</td>
</tr>
<tr>
<th>Supply Chain Emission Factors with Margins</th>
<td>22092.0</td>
<td>0.097681</td>
<td>0.288992</td>
<td>0.0</td>
<td>0.0</td>
<td>0.003</td>
<td>0.052</td>
<td>7.290</td>
</tr>
<tr>
<th>DQ ReliabilityScore of Factors without Margins</th>
<td>22092.0</td>
<td>3.308030</td>
<td>0.499643</td>
<td>2.0</td>
<td>3.0</td>
<td>3.000</td>
<td>4.000</td>
<td>4.000</td>
</tr>
<tr>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<td>22092.0</td>
<td>2.571429</td>
<td>0.494883</td>
<td>2.0</td>
<td>2.0</td>
<td>3.000</td>
<td>3.000</td>
<td>3.000</td>
</tr>
<tr>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<td>22092.0</td>
<td>1.000000</td>
<td>0.000000</td>
<td>1.0</td>
<td>1.0</td>
<td>1.000</td>
<td>1.000</td>
<td>1.000</td>
</tr>
<tr>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<td>22092.0</td>
<td>2.632129</td>
<td>1.135661</td>
<td>1.0</td>
<td>1.0</td>
<td>3.000</td>
<td>3.000</td>
<td>5.000</td>
</tr>
<tr>
<th>DQ DataCollection of Factors without Margins</th>
<td>22092.0</td>
<td>1.000000</td>
<td>0.000000</td>
<td>1.0</td>
<td>1.0</td>
<td>1.000</td>
<td>1.000</td>
<td>1.000</td>
</tr>
<tr>
<th>Year</th>
<td>22092.0</td>
<td>2013.000000</td>
<td>2.000045</td>
<td>2010.0</td>
<td>2011.0</td>
<td>2013.000</td>
<td>2015.000</td>
<td>2016.000</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=f1b30be9">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [19]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">isnull</span><span class="p">()</span><span class="o">.</span><span class="n">sum</span><span class="p">()</span> <span class="c1"># Checking for null values in each column </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[19]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Code                                                      0
Name                                                      0
Substance                                                 0
Unit                                                      0
Supply Chain Emission Factors without Margins             0
Margins of Supply Chain Emission Factors                  0
Supply Chain Emission Factors with Margins                0
DQ ReliabilityScore of Factors without Margins            0
DQ TemporalCorrelation of Factors without Margins         0
DQ GeographicalCorrelation of Factors without Margins     0
DQ TechnologicalCorrelation of Factors without Margins    0
DQ DataCollection of Factors without Margins              0
Source                                                    0
Year                                                      0
dtype: int64</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=ccf7fbe1">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [20]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Visualize distribution</span>
<span class="n">sns</span><span class="o">.</span><span class="n">histplot</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">],</span> <span class="n">bins</span><span class="o">=</span><span class="mi">50</span><span class="p">,</span> <span class="n">kde</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Target Variable Distribution'</span><span class="p">)</span>
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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAk0AAAHHCAYAAACiOWx7AAAAOnRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjEwLjEsIGh0dHBzOi8vbWF0cGxvdGxpYi5vcmcvc2/+5QAAAAlwSFlzAAAPYQAAD2EBqD+naQAAS95JREFUeJzt3QecE2X+x/HfZitFOiygdJDem1hQBEFQT5S/J1iOo3kiKEVBUQTUOzkLNkA5zhP0FEU8QQWlNxUQRJAioCgI0hYEFkHKsjv/1++BiUk2u+zCbiaTfN53cTfJk8lkkmW++T3PPBNjWZYlAAAAyJYn+7sBAACgCE0AAAA5QGgCAADIAUITAABADhCaAAAAcoDQBAAAkAOEJgAAgBwgNAEAAOQAoQkAACAHCE0AXGnUqFESExNzXo+tXLmy3Hjjjedst3jxYvMc+tMpoVyHYNtUr/fv319CYfLkyeb5tm/fHpLnA3KL0ASEgO4IcnJxcucczLJly8yO9PDhw9m2S0tLk1KlSsmVV16ZZRs9Y1OFChWkSZMmEq00DPi+3/Hx8Wa7XX755fLoo4/Kjh078uy5nn76aZkxY4aEo3BeNyA7MZx7Dsh/b7/9tt/1t956S+bNmyf//e9//W6/7rrrJDk5WcLF888/L0OGDJFt27aZ6kx2+vbtK//6179M20qVKmW6f8mSJXLNNdfImDFjZPDgwRe8bqdPnzaXpKSkXD9WX0u9evVk5syZ2bbTENumTRtZtGiRWfe8CE1VqlSRbt26SadOnSQjI0MOHTokq1atkg8//NAEqf/85z/StWtX72O0zalTpyQhIUE8npx/zy1cuLD83//9n6neXMg21XXq16+fjBs3Lhev9PzWLT093QTwxMTE864iAvkpLl+XDsC46667/K6vWLHChKbA28+Hfu85ceKEFChQQJx05513yoQJE+Tdd9+VRx55JNP9U6ZMMTt930BwPo4dOyaFChWSuLg4c3EjrbYFvvc///yztG/fXrp37y61a9eWhg0bmtt1m51PMHTjNo2NjTUXIFzRPQeEiUmTJsm1114rZcqUMd+069SpI6+99lqW43HmzJkjzZo1M2FJKzz2jvdPf/qT2QHqcgYNGmTaBev6++qrr+T666+XokWLSsGCBeXqq6+WL7/80nu/dstplUlpdcTuUspqvMkVV1xh1k3DUSCtHnzwwQemalO+fHlZt26d/PWvf5WqVauaQFC2bFnp2bOn/Prrr0HH2Hz33Xdyxx13SPHixb1dgMHG3+R0G9rmzp0rjRo1MuugbbXakxPn2nbnQ6tzWnnRqtKzzz6b7ZimH374Qbp06WK2m677JZdcYsJoamqquV/baxB68803ve+bbu/z2aa2d955R2rWrGmer2nTprJ06VK/+3X5waqRgcvMbt2yGtP06quvSt26dc17qp8frXwFdhlrJVCrh/q69HOm78vFF1/sty2BC+XOr2lABNKdu+4YNPTot/1PPvlE7rvvPtM9ozsJX1u2bDFdPH/729+kT58+ZmemOyINDHv27JEBAwaYHaoGGO1aCrRw4ULp2LGj2fmNHDnSVDPswPH5559LixYt5NZbb5Xvv//eVI5efPFFM/ZGlS5dOuj6685Od8I6XmXjxo3mtdhmz54tBw8eNNUopVW2n376SXr06GHWU9tPnDjR/NQqXOCO+7bbbpMaNWqYZWc3oiA321CDx+233y733nuvqe7o69fn0XXVbtKs5GTbna9WrVpJtWrVzPbJioaqDh06yMmTJ+X+++8322/Xrl2mq1GDhAY57fbt3bu3WZd77rnHPE6Xez7b1O5anTp1qjzwwAMmuGiI0dC4cuVKE1RyIyfrFhi6nnjiCWnXrp3pAtbPvr7P2qWpQVXHhdm0q1PXSz+7f/7zn01Qf/jhh6V+/frmPQMumI5pAhBa/fr1072U322///57pnYdOnSwqlat6ndbpUqVzGNnz57td/uYMWPM7TNmzPDedvz4catWrVrm9kWLFpnbMjIyrBo1aphl6+++z1+lShXruuuu89723HPPmcdu27YtR69r48aNpv2wYcP8bu/atauVlJRkpaamZvla3333XfPYpUuXem8bOXKkua1bt26Z2tv3Xcg2/N///ue9TdetXLlyVuPGjb236TY7320XjG5HXZ5u16zcfPPNpo29rQLXYc2aNeb6tGnTsn2uQoUKWd27d890e263qV7Xy9dff+297eeffzbv5y233OK9TZ9Lt2tOlpnVuk2aNMnv85aSkmIlJCRY7du3t9LT073txo0bZ9q98cYb3tuuvvpqc9tbb73lve3kyZNW2bJlrS5dumSxlYDcoXsOCBO+Y5K0m+XAgQOm20crMna3i027y7Ta4EsrJNodoVUWm3alaCXK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Dz4wJ83WMV6RGpx27twpAwYMMGM89ACPaNKxY0fv7zqOS0NUpUqV5P3335devXpJpH4J0krT008/ba5rpUn/vidMmGA+69HgP//5j3nvtcLodlSawlSpUqUkNjZW9u3b53e7Xi9btqxj64X8pec9nDlzpixatMgMko4GCQkJUr16dWnatKmpvOhBAC+//LJEKu1214M5mjRpInFxceaiIfGVV14xv2uFOVoUK1ZMLr30Utm6datEqnLlymX6AlC7du2I75a0/fzzzzJ//nzp3bu3RAJCUxjvSHQnsmDBAr9vLHo9GsZ7RBsd866BSbumFi5cKFWqVJFopZ/zkydPSqRq27at6ZLU6pp90UqEju/R3/XLUrQ4evSo/PjjjyZYRCrtZg+cPuT77783FbZoMGnSJDOWS8fvRQK658KYTjeg5Vv9B7VFixby0ksvmUGyPXr0kEj/h9T3m6eOe9CdiQ6KrlixokRql9yUKVPko48+MnM12ePWihYtauZ1iVTDhg0zZXt9X3Vci26DxYsXm7EfkUrf38CxaoUKFTJz+ET6GLaHHnrIzMGmgWH37t1mOhUNid26dZNINWjQILn88stN99yf//xnM9fexIkTzSUavgBNmjTJ7Me0ihoRnD58D9kbO3asVbFiRSshIcFMQbBixQor0i1atMgcbh946d69uxWpgr1evUyaNMmKZD179rQqVapkPt+lS5e22rZta82dO9eKNtEy5cDtt99ulStXzrzfF198sbm+detWK9J98sknVr169azExESrVq1a1sSJE61oMGfOHPPv2JYtW6xIEaP/cTq4AQAAhDvGNAEAAOQAoQkAACAHCE0AAAA5QGgCAADIAUITAABADhCaAAAAcoDQBAAAkAOEJiCfjBo1Sho1apTvz6MzaMfExJiziF+IypUrm1nnw5GeHb1z586ueU8gMnnyZHNuuXPRz+6MGTPErcL57wZ5j9CEiLJ//37p27evOS1HYmKiOblxhw4d5MsvvxS3WrNmjdx2222SnJwsSUlJUqNGDenTp485f1VeWrVqldxzzz0XtIxrrrnG7AQDL/fee+8FLVdP4Ks74bw4jYfv+Rzzc0cauA3y6gTMbgkZt99+u99nNC8Dq/05++c//5npPj3Hmd6nzxcKefF3A/cgNCGidOnSxYSMN9980/yD/fHHH5t/YH/99Vdxo5kzZ8pll11mTmD7zjvvyKZNm+Ttt98256R7/PHH8/S5SpcuLQULFrzg5Wig27Nnj9/l2WefvaBl6uvNSdXiXAoXLmzO8RYKTz75pN820M9lOElLS8vX5es5E/VErfmlQoUKmYL0rl27TCi+0BMA64kyTp8+HdK/G7gDoQkRQ7unPv/8c3nmmWekTZs25qSgeqJjPSnsn/70J9Nm+/bt5luongDY93F6m3Zz+XZ3zZo1Sxo0aGCqOxpcNmzYkKnrQb/xa+VH22hFa+fOnUHXbenSpRIfH+89Ea9t4MCBctVVVwV9zO+//25OztypUycT/tq1aydVqlSRli1byvPPPy//+te//NqvXr3anNxZ/wHXE4T6nlldzyR/8803m2qVBofmzZvL/Pnzs+1m0G3w+uuvyy233GKWqa9T1+NctK1W+HwvRYoU8dv+77//vnndumPVddGAq9/Ydf11/fQkvlo1zKp77oMPPpD69eubx2sI0m2jJ7O23z993/UkuPoe6Vnmf/7556DVDj2hqIYbrQJpZVLvmz17tvd+e30//PBD85nS19awYUNZvnx5jk7M67sNdOeanp4uvXr1Mu+jrnvNmjVNFS3QG2+8IXXr1jXrpAGgf//+3vdI6Xui62VfV6+99ppUq1ZNEhISzHL/+9//+i1T22sb/VvQbfOPf/xDDh06JHfeeadZN10ffY/1BKtZBXjdnvoalP4N6TIfeeQRb5vevXvLXXfdlal7Tn9/4okn5Ntvv/VW3nwDz4EDB3L9ObvxxhvN43yryPplqX379pnCmm4L/WzZ78kdd9whKSkp3vvtv/nPPvtMmjZtarb7F198YU4irdtHt5e+Dy+++KL5EqZ/t+f7d5ObbY7wQ2hCxNCdrV40yGhl5kINGTJExowZY3bm+g+cnp3d99u5hhrd8bz11lvmH24NX127dg26rNatW0vVqlX9dmS6LK0e9ezZM+hj5syZY3YKQ4cODXp/YOXlscceM+v79ddfmzOK+y736NGjJnzpt3CteFx//fXm9ezYsSPbbaA7Oj0z+7p168zj9R/7gwcPyoXSs9sPHz5cvvnmG7OuuhPT16kBQoPv1q1bZcSIEUEfq1Wbbt26mdenlTfd4d16663e6oCGq6uvvtqss4Yb7TrRHVkw+ny6zTSEansNvhoqfvjhh0zbVrv2NChceuml5vlzWonwpSFNA9q0adPku+++M6/x0UcfNSHSpsGmX79+Zr3Xr19vdrjVq1c39+lnUelOVreDfX369OkyYMAAefDBB024/9vf/mYC96JFi/yeX0Oj7sx1ubr9tFqp66FhQbelPnepUqWCrruGXA0RdsVsyZIlpq39ZcO+TUNFsK46XTcNgnblTW+7kM+ZhkNt5xs4NIgF+3vSv7WnnnrKhDb990HDsAbxQBoAtctPt4V+YRo8eLD529b3YN68eeazqZ/Zc8nu9eRmmyMMOX3GYCAvffDBB1bx4sWtpKQk6/LLL7eGDRtmffvtt977t23bZs66vWbNGu9thw4dMrctWrTIXNefev29997ztvn111+tAgUKWFOnTjXXJ02aZNqsWLHC22bTpk3mtq+++spcHzlypNWwYUPv/c8884xVu3Zt7/X//e9/VuHCha2jR48GfS3aXpd38ODBbF+zvb7z58/33jZr1ixz2/Hjx7N8XN26da2xY8d6r1eqVMl68cUXvdf18cOHD/de1/XU2z777LMsl3n11Vdb8fHxVqFChfwub7/9tt/2f/31172Peffdd81tCxYs8N42evRoq2bNmt7r3bt3t26++Wbz++rVq0377du3Z3p+fZ/0vsWLFwddv8D3pHz58tY//vEPvzbNmze37rvvvizXd+PGjeY2fb+zotsyISHBbxu8/PLLQdv269fP6tKli986PfbYY1kuW597+vTpfrfpZ71Pnz5+t912221Wp06d/B43cOBAvzY33XST1aNHDyunmjRpYj333HPm986dO5ttp6/zt99+s3755RfzHN9//733b6Ro0aJZbvsL/ZwNGDDAWrt2rXXRRReZxyxZssQqU6aMlZaWZp5Hny8rq1atMs+h6+37NzRjxgxvmyNHjpjP8rRp07y3HT582CpYsKB57vP9u8ntNkd4odKEiBvTtHv3bvPNUKsp+i24SZMm5zWIuFWrVt7fS5QoYbo89JuhTSsk2rVkq1Wrlqn++Lbxpd9stYKyYsUKc13XSb+Nauk/mDP//uacfjO22WM67C4IrTRppaR27dpmHbUip+t5rkqT7zJ1PbWbzbdbIxj9Vq0VGd+L3T0abLnaZai0u833tqyeR7vH2rZta9rrAPl///vfpsvDfp90O2vFSCtpWknSqkYwR44cMZ8V7b7zpdcD38Pstm12lUrfbfCXv/zF3D5+/HjT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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d637be90">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [21]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Check categorical variables</span>
<span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Substance'</span><span class="p">]</span><span class="o">.</span><span class="n">value_counts</span><span class="p">())</span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>carbon dioxide    5523
methane           5523
nitrous oxide     5523
other GHGs        5523
Name: Substance, dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=8ff1fc9d">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [22]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">.</span><span class="n">value_counts</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Unit' with count </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>kg/2018 USD, purchaser price         16569
kg CO2e/2018 USD, purchaser price     5523
Name: Unit, dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=7bd9109b">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [25]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Unit'</span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>['kg/2018 USD, purchaser price' 'kg CO2e/2018 USD, purchaser price']
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=fc83fed6">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [26]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span><span class="o">.</span><span class="n">value_counts</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Source' with count </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Industry     11060
Commodity    11032
Name: Source, dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=e93721db">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [27]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="p">[</span><span class="s1">'Substance'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">()</span> <span class="c1"># Checking unique values in 'Substance' </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[27]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>array(['carbon dioxide', 'methane', 'nitrous oxide', 'other GHGs'],
      dtype=object)</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=4826a3bc">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [28]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">substance_map</span><span class="o">=</span><span class="p">{</span><span class="s1">'carbon dioxide'</span><span class="p">:</span><span class="mi">0</span><span class="p">,</span> <span class="s1">'methane'</span><span class="p">:</span><span class="mi">1</span><span class="p">,</span> <span class="s1">'nitrous oxide'</span><span class="p">:</span><span class="mi">2</span><span class="p">,</span> <span class="s1">'other GHGs'</span><span class="p">:</span><span class="mi">3</span><span class="p">}</span> <span class="c1"># Mapping substances to integers </span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=9c7fc8a6">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [29]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="p">[</span><span class="s1">'Substance'</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">'Substance'</span><span class="p">]</span><span class="o">.</span><span class="n">map</span><span class="p">(</span><span class="n">substance_map</span><span class="p">)</span> 
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=88fdb187">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [30]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="p">[</span><span class="s1">'Substance'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">()</span> <span class="c1"># Checking unique values in 'Substance' </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[30]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>array([0, 1, 2, 3])</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=fc042f93">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [31]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Unit' </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>['kg/2018 USD, purchaser price' 'kg CO2e/2018 USD, purchaser price']
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=5f897a7c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [32]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">unit_map</span><span class="o">=</span><span class="p">{</span><span class="s1">'kg/2018 USD, purchaser price'</span><span class="p">:</span><span class="mi">0</span><span class="p">,</span> <span class="s1">'kg CO2e/2018 USD, purchaser price'</span><span class="p">:</span><span class="mi">1</span><span class="p">}</span> <span class="c1"># Mapping units to integers </span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=a454db80">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [33]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">.</span><span class="n">map</span><span class="p">(</span><span class="n">unit_map</span><span class="p">)</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=1243c8e1">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [34]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Unit'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Unit' </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>[0 1]
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=84076edc">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [35]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Source' </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>['Commodity' 'Industry']
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=58c7d327">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [36]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">source_map</span><span class="o">=</span><span class="p">{</span><span class="s1">'Commodity'</span><span class="p">:</span><span class="mi">0</span><span class="p">,</span> <span class="s1">'Industry'</span><span class="p">:</span><span class="mi">1</span><span class="p">}</span> <span class="c1"># Mapping sources to integers </span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=f0b3e63e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [37]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span><span class="o">.</span><span class="n">map</span><span class="p">(</span><span class="n">source_map</span><span class="p">)</span>   <span class="c1"># applying the mapping to 'Source' column </span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=cec5c804">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [38]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">print</span><span class="p">(</span><span class="n">df</span><span class="p">[</span><span class="s1">'Source'</span><span class="p">]</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking unique values in 'Source' </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>[0 1]
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=e39744e3">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [39]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">()</span> <span class="c1"># Checking data types and non-null counts after mapping </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 22092 entries, 0 to 22091
Data columns (total 14 columns):
 #   Column                                                  Non-Null Count  Dtype  
---  ------                                                  --------------  -----  
 0   Code                                                    22092 non-null  object 
 1   Name                                                    22092 non-null  object 
 2   Substance                                               22092 non-null  int64  
 3   Unit                                                    22092 non-null  int64  
 4   Supply Chain Emission Factors without Margins           22092 non-null  float64
 5   Margins of Supply Chain Emission Factors                22092 non-null  float64
 6   Supply Chain Emission Factors with Margins              22092 non-null  float64
 7   DQ ReliabilityScore of Factors without Margins          22092 non-null  int64  
 8   DQ TemporalCorrelation of Factors without Margins       22092 non-null  int64  
 9   DQ GeographicalCorrelation of Factors without Margins   22092 non-null  int64  
 10  DQ TechnologicalCorrelation of Factors without Margins  22092 non-null  int64  
 11  DQ DataCollection of Factors without Margins            22092 non-null  int64  
 12  Source                                                  22092 non-null  int64  
 13  Year                                                    22092 non-null  int64  
dtypes: float64(3), int64(9), object(2)
memory usage: 2.4+ MB
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=17a70cb5">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [40]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">Code</span><span class="o">.</span><span class="n">unique</span><span class="p">()</span> <span class="c1"># Checking unique values in 'Code' df['Code']</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[40]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>array(['1111A0', '1111B0', '111200', '111300', '111400', '111900',
       '112120', '1121A0', '112300', '112A00', '113000', '114000',
       '115000', '211000', '212100', '212230', '2122A0', '212310',
       '2123A0', '213111', '21311A', '221100', '221200', '221300',
       '230301', '230302', '233210', '233230', '233240', '233262',
       '2332A0', '2332C0', '2332D0', '233411', '233412', '2334A0',
       '311111', '311119', '311210', '311221', '311224', '311225',
       '311230', '311300', '311410', '311420', '311513', '311514',
       '31151A', '311520', '311615', '31161A', '311700', '311810',
       '3118A0', '311910', '311920', '311930', '311940', '311990',
       '312110', '312120', '312130', '312140', '312200', '313100',
       '313200', '313300', '314110', '314120', '314900', '315000',
       '316000', '321100', '321200', '321910', '3219A0', '322110',
       '322120', '322130', '322210', '322220', '322230', '322291',
       '322299', '323110', '323120', '324110', '324121', '324122',
       '324190', '325110', '325120', '325130', '325180', '325190',
       '325211', '3252A0', '325310', '325320', '325411', '325412',
       '325413', '325414', '325510', '325520', '325610', '325620',
       '325910', '3259A0', '326110', '326120', '326130', '326140',
       '326150', '326160', '326190', '326210', '326220', '326290',
       '327100', '327200', '327310', '327320', '327330', '327390',
       '327400', '327910', '327991', '327992', '327993', '327999',
       '331110', '331200', '331313', '33131B', '331410', '331420',
       '331490', '331510', '331520', '332114', '332119', '33211A',
       '332200', '332310', '332320', '332410', '332420', '332430',
       '332500', '332600', '332710', '332720', '332800', '332913',
       '33291A', '332991', '332996', '332999', '33299A', '333111',
       '333112', '333120', '333130', '333242', '33329A', '333314',
       '333316', '333318', '333413', '333414', '333415', '333511',
       '333514', '333517', '33351B', '333611', '333612', '333613',
       '333618', '333912', '33391A', '333920', '333991', '333993',
       '333994', '33399A', '33399B', '334111', '334112', '334118',
       '334210', '334220', '334290', '334300', '334413', '334418',
       '33441A', '334510', '334511', '334512', '334513', '334514',
       '334515', '334516', '334517', '33451A', '334610', '335110',
       '335120', '335210', '335221', '335222', '335224', '335228',
       '335311', '335312', '335313', '335314', '335911', '335912',
       '335920', '335930', '335991', '335999', '336111', '336112',
       '336120', '336211', '336212', '336213', '336214', '336310',
       '336320', '336350', '336360', '336370', '336390', '3363A0',
       '336411', '336412', '336413', '336414', '33641A', '336500',
       '336611', '336612', '336991', '336992', '336999', '337110',
       '337121', '337122', '337127', '33712N', '337215', '33721A',
       '337900', '339112', '339113', '339114', '339115', '339116',
       '339910', '339920', '339930', '339940', '339950', '339990',
       '4200ID', '423100', '423400', '423600', '423800', '423A00',
       '424200', '424400', '424700', '424A00', '425000', '441000',
       '444000', '445000', '446000', '447000', '448000', '452000',
       '454000', '481000', '482000', '483000', '484000', '485000',
       '486000', '48A000', '491000', '492000', '493000', '4B0000',
       '511110', '511120', '511130', '5111A0', '511200', '512100',
       '512200', '515100', '515200', '517110', '517210', '517A00',
       '518200', '519130', '5191A0', '522A00', '523900', '523A00',
       '524113', '5241XX', '524200', '525000', '52A000', '531HSO',
       '531HST', '531ORE', '532100', '532400', '532A00', '533000',
       '541100', '541200', '541300', '541400', '541511', '541512',
       '54151A', '541610', '5416A0', '541700', '541800', '541920',
       '541940', '5419A0', '550000', '561100', '561200', '561300',
       '561400', '561500', '561600', '561700', '561900', '562000',
       '611100', '611A00', '611B00', '621100', '621200', '621300',
       '621400', '621500', '621600', '621900', '622000', '623A00',
       '623B00', '624100', '624400', '624A00', '711100', '711200',
       '711500', '711A00', '712000', '713100', '713200', '713900',
       '721000', '722110', '722211', '722A00', '811100', '811200',
       '811300', '811400', '812100', '812200', '812300', '812900',
       '813100', '813A00', '813B00', '814000', '331314'], dtype=object)</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=aa8a6391">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [41]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">Name</span><span class="o">.</span><span class="n">unique</span><span class="p">()</span> <span class="c1"># Checking unique values in 'Name' </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[41]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>array(['Fresh soybeans, canola, flaxseeds, and other oilseeds',
       'Fresh wheat, corn, rice, and other grains',
       'Fresh vegetables, melons, and potatoes',
       'Fresh fruits and tree nuts',
       'Greenhouse crops, mushrooms, nurseries, and flowers',
       'Tobacco, cotton, sugarcane, peanuts, sugar beets, herbs and spices, and other crops',
       'Dairies', 'Cattle ranches and feedlots', 'Poultry farms',
       'Animal farms and aquaculture ponds (except cattle and poultry)',
       'Timber and raw forest products', 'Wild-caught fish and game',
       'Agriculture and forestry support', 'Unrefined oil and gas',
       'Coal', 'Copper, nickel, lead, and zinc',
       'Iron, gold, silver, and other metal ores', 'Dimensional stone',
       'Sand, gravel, clay, phosphate, other nonmetallic minerals',
       'Well drilling', 'Other support activities for mining',
       'Electricity', 'Natural gas',
       'Drinking water and wastewater treatment',
       'Nonresidential maintenance and repair',
       'Residential maintenance and repair', 'Health care structures',
       'Manufacturing structures', 'Power and communication structures',
       'Educational and vocational structures',
       'Commercial structures, including farm structures',
       'Transportation structures and highways and streets',
       'Other nonresidential structures',
       'Single-family residential structures',
       'Multifamily residential structures',
       'Other residential structures', 'Dog and cat food',
       'Other animal food', 'Flours and malts', 'Corn products',
       'Soybean and other oilseed processing',
       'Refined vegetable, olive, and seed oils', 'Breakfast cereals',
       'Sugar, candy, and chocolate', 'Frozen food',
       'Fruit and vegetable preservation', 'Cheese',
       'Dry, condensed, and evaporated dairy', 'Fluid milk and butter',
       'Ice cream and frozen desserts', 'Packaged poultry',
       'Packaged meat (except poultry)', 'Seafood',
       'Bread and other baked goods',
       'Cookies, crackers, pastas, and tortillas', 'Snack foods',
       'Coffee and tea', 'Flavored drink concentrates',
       'Seasonings and dressings', 'All other foods',
       'Soft drinks, bottled water, and ice', 'Breweries and beer',
       'Wineries and wine', 'Distilleries and spirits',
       'Tobacco products', 'Fiber, yarn, and thread', 'Fabric',
       'Finished and coated fabric', 'Carpets and rugs',
       'Curtains and linens', 'Other textiles', 'Clothing', 'Leather',
       'Lumber and treated lumber', 'Plywood and veneer',
       'Wooden windows, door, and flooring',
       'Veneer, plywood, and engineered wood', 'Wood pulp', 'Paper',
       'Cardboard', 'Cardboard containers', 'Paper bags and coated paper',
       'Stationery', 'Sanitary paper (tissues, napkins, diapers, etc.)',
       'All other converted paper products',
       'Books, newspapers, magazines, and other print media',
       'Printing support',
       'Gasoline, fuels, and by-products of petroleum refining',
       'Asphalt pavement', 'Asphalt shingles',
       'Other petroleum and coal products', 'Petrochemicals',
       'Compressed Gases', 'Synthetic dyes and pigments',
       'Other basic inorganic chemicals', 'Other basic organic chemicals',
       'Plastics', 'Synthetic rubber and artificial and synthetic fibers',
       'Fertilizers', 'Pesticides', 'Medicinal and botanical ingredients',
       'Pharmaceutical products (pills, powders, solutions, etc.)',
       'Blood sugar, pregnancy, and other diagnostic test kits',
       'Vaccines and other biological medical products',
       'Paints and coatings', 'Adhesives', 'Soap and cleaning compounds',
       'Toiletries', 'Ink and ink cartridges',
       'Chemicals (except basic chemicals, agrichemicals, polymers, paints, pharmaceuticals,soaps, cleaning compounds)',
       'Plastic bags, films, and sheets',
       'Plastic pipe, fittings, and sausage casings',
       'Laminated plastic plates and shapes', 'Polystyrene foam products',
       'Urethane and other foam products', 'Plastic bottles',
       'Other plastic products', 'Rubber tires',
       'Rubber and plastic belts and hoses', 'Other rubber products',
       'Clay and ceramic products', 'Glass and glass products', 'Cement',
       'Ready-mix concrete', 'Concrete pipe, bricks, and blocks',
       'Other concrete products', 'Lime and gypsum products',
       'Abrasive products', 'Cut stone and stone products',
       'Ground or treated minerals and earth', 'Mineral wool',
       'Other nonmetallic mineral products',
       'Primary iron, steel, and ferroalloy products',
       'Secondary steel products',
       'Alumina refining and primary aluminum production',
       'Aluminum products',
       'Nonferrous Metal (except Aluminum) Smelting and Refining',
       'Secondary copper products',
       'Other secondary nonferrous metal products', 'Cast iron and steel',
       'Nonferrous metal casts', 'Custom metal rolls',
       'Metal crown, closure, and other metal stamping (except automotive)',
       'All other forging, stamping, and sintering',
       'Cutlery and handtools', 'Metal structural products',
       'Metal windows, doors, and architectural products',
       'Power boilers and heat exchangers', 'Heavy gauge metal tanks',
       'Light gauge metal cans, boxes, and containers',
       'Metal hinges, keys, lock, and other hardware',
       'Springs and wires', 'Machine shops', 'Screws, nuts, and bolts',
       'Metal coatings, engravings, and heat treatments',
       'Metal plumbing drains, faucets, valves, and other fittings',
       'Valve and fittings (except for plumbing)',
       'Ball and roller bearings', 'Fabricated pipe and pipe fittings',
       'Other fabricated metal manufacturing',
       'Ammunition, arms, ordnance, and related accessories',
       'Farm machinery and equipment', 'Lawn and garden equipment',
       'Construction machinery', 'Mining and oil/gas field machinery',
       'Semiconductor machinery',
       'Machinery for the paper, textile, food or other industries (except semiconductor machinery)',
       'Optical instruments and lenses',
       'Photography and photocopying equipment',
       'Other commercial and service industry machinery',
       'Industrial and commercial fan and blower and air purification equipment',
       'Heating equipment other than warm air furnaces',
       'Air conditioning, refrigeration, and warm air heating equipment',
       'Industrial molds', 'Special tools, dies, jigs, and fixtures',
       'Machine tool manufacturing',
       'Cutting and machine tool accessory, rolling mill, and other metalworking machines',
       'Turbines and turbine generator sets',
       'Speed changers, industrial high-speed drives, and gears',
       'Mechanical power transmission equipment',
       'Other engine equipment', 'Air and gas compressors',
       'Pumps and pumping equipment', 'Material handling equipment',
       'Power tools', 'Packaging machinery',
       'Industrial process furnaces and ovens',
       'Welding and Soldering Equipment, Scales and Balances, and other general purpose machinery',
       'Hydraulic pumps, motors, cylinders and actuators', 'Computers',
       'Computer storage device readers',
       'Computer terminals and other computer peripheral equipment',
       'Telephones', 'Wireless communications',
       'Communications equipment', 'Audio and video equipment',
       'Semiconductors', 'Printed circuit and electronic assembly',
       'Electronic capacitors, resistors, coils, transformers, connectors and other components (except  semiconductors and printed circuit assemblies)',
       'Electromedical appartuses', 'Navigation instruments',
       'Automatic controls for HVAC and refrigeration equipment',
       'Industrial process variable instruments',
       'Fluid meters and counting devices', 'Signal testing instruments',
       'Analytical laboratory instruments', 'Irradiation apparatuses',
       'Watches, clocks, and other measuring and controlling devices',
       'External hard drives, CDs, other storage media', 'Light bulbs',
       'Light fixtures', 'Small electrical appliances',
       'Home cooking appliances', 'Home refrigerators and freezers',
       'Home laundry machines',
       'Major home appliances (except ovens, stoves, refrigerators and laundry machines)',
       'Specialty transformers', 'Motors and generators',
       'Switchgear and switchboards', 'Relay and industrial controls',
       'Storage batteries', 'Primary batteries',
       'Communication and energy wire and cable', 'Wiring devices',
       'Carbon and graphite products',
       'other miscellaneous electrical equipment and components',
       'Automobiles', 'Pickup trucks, vans, and SUVs',
       'Heavy duty trucks', 'Vehicle bodies', 'Truck trailers',
       'Motor homes', 'Travel trailer and campers',
       'Vehicle engines and engine parts',
       'Vehicle electrical and electronic equipment',
       'Transmission and power train parts',
       'Vehicle seating and interior trim (upholstery)',
       'Vehicle metal stamping', 'Other vehicle parts',
       'Motor vehicle steering, suspension components (except spring), and brake systems',
       'Aircraft', 'Aircraft engines and parts', 'Other aircraft parts',
       'Guided missiles and space vehicles',
       'Propulsion units and parts for space vehicles and guided missiles',
       'Railroad rolling stock', 'Ships and ship repair', 'Boats',
       'Motorcycle, bicycle, and parts',
       'Military armored vehicles and tanks',
       'Other transportation equipment',
       'Wood kitchen cabinets and countertops',
       'Home furniture - upholstered',
       'Home furniture - wood, nonupholstered', 'Institutional furniture',
       'Other household nonupholstered furniture', 'Shelving and lockers',
       'Office furniture and custom architectural woodwork and millwork',
       'Mattresses, blinds and shades',
       'Surgical and medical instruments',
       'Surgical appliance and supplies', 'Dental equipment and supplies',
       'Ophthalmic goods', 'Dental laboratories',
       'Jewelry and silverware', 'Sporting and athletic goods',
       'Dolls, toys, and games', 'Office supplies (not paper)', 'Signs',
       'Gaskets, seals, musical instruments, fasteners, brooms, brushes, mop and other misc. goods',
       'Customs duties',
       'Motor vehicle and motor vehicle parts and supplies',
       'Professional and commercial equipment and supplies',
       'Household appliances and electrical and electronic goods',
       'Machinery, equipment, and supplies',
       'Other durable goods merchant wholesalers',
       'Drugs and druggists’ sundries',
       'Grocery and related product wholesalers',
       'Petroleum and petroleum products',
       'Other nondurable goods merchant wholesalers',
       'Wholesale electronic markets and agents and brokers',
       'Vehicles and parts sales',
       'Building material and garden equipment and supplies dealers',
       'Food and beverage stores', 'Health and personal care stores',
       'Gasoline stations', 'Clothing and clothing accessories stores',
       'General merchandise stores', 'Nonstore retailers',
       'Air transport', 'Rail transport',
       'Water transport (boats, ships, ferries)', 'Truck transport',
       'Passenger ground transport', 'Pipeline transport',
       'Scenic and sightseeing transportation and support activities for transportation',
       'Postal service', 'Couriers and messengers', 'Warehousing',
       'All other retail', 'Newspapers', 'Magazines and journals',
       'Books', 'Directory, mailing list, and other publishers',
       'Software', 'Movies and film', 'Sound recording',
       'Radio and television', 'Cable and subscription programming',
       'Telecommunications', 'Wireless telecommunications',
       'Satellite, telecommunications resellers, and all other telecommunications',
       'Data processing and hosting',
       'Internet publishing and broadcasting',
       'News syndicates, libraries, archives, Internet publishing and all other information services',
       'Nondepository credit intermediation and related activities',
       'Investment advice, portfolio management, and other financial advising services',
       'Securities and commodities brokerage and exchanges',
       'Direct life insurance carriers',
       'Insurance carriers, except direct life',
       'Insurance agencies and brokerages',
       'Funds, trusts, and financial vehicles',
       'Monetary authorities and depository credit intermediation',
       'Owner-occupied housing', 'Tenant-occupied housing',
       'Other real estate', 'Vehicle rental and leasing',
       'Commercial equipment rental',
       'Consumer goods and general rental centers',
       'Lessors of nonfinancial intangible assets', 'Legal services',
       'Accounting, tax preparation, bookkeeping, and payroll',
       'Architectural, engineering, and related services',
       'Specialized design', 'Custom computer programming',
       'Computer systems design',
       'Other computer related services, including facilities management',
       'Management consulting',
       'Environmental and other technical consulting services',
       'Scientific research and development',
       'Advertising and public relations', 'Photographers',
       'Veterinarians',
       'Marketing research and all other miscellaneous professional, scientific, and technical services',
       'Company and enterprise management', 'Office administration',
       'Facilities support', 'Employment services', 'Business support',
       'Travel arrangement and reservation', 'Investigation and security',
       'Buildings and dwellings services', 'Other support services',
       'Waste management and remediation',
       'Elementary and secondary schools',
       'Colleges, universities, junior colleges, and professional schools',
       'Other educational services', 'Physicians', 'Dentists',
       'Healthcare practitioners (except physicians and dentists)',
       'Outpatient healthcare', 'Medical laboratories', 'Home healthcare',
       'Ambulances', 'Hospitals', 'Nursing and community care facilities',
       'Residential mental retardation, mental health, substance abuse and other facilities',
       'Individual and family services', 'Child day care',
       'Community food, housing, and other relief services, including rehabilitation services',
       'Performances', 'Sports',
       'Independent artists, writers, and performers',
       'Promoters and agents',
       'Museums, historical sites, zoos, and parks',
       'Amusement parks and arcades',
       'Gambling establishments (except casino hotels)',
       'Golf courses, marinas, ski resorts, fitness and other rec centers and industries',
       'Hotels and campgrounds', 'Full-service restaurants',
       'Limited-service restaurants',
       'All other food and drinking places', 'Vehicle repair',
       'Electronic  equipment repair and maintenance',
       'Commercial machinery repair', 'Household goods repair',
       'Salons and barber shops', 'Funerary services',
       'Dry-cleaning and laundry',
       'Pet care, photofinishing, parking and other sundry services',
       'Religious organizations',
       'Grantmaking, giving, and social advocacy organizations',
       'Civic, social, professional, and similar organizations',
       'Household employees', 'Oilseed farming', 'Grain farming',
       'Vegetable and melon farming', 'Fruit and tree nut farming',
       'Greenhouse, nursery, and floriculture production',
       'Other crop farming', 'Dairy cattle and milk production',
       'Beef cattle ranching and farming, including feedlots and dual-purpose ranching and farming',
       'Poultry and egg production',
       'Animal production, except cattle and poultry and eggs',
       'Forestry and logging', 'Fishing, hunting and trapping',
       'Support activities for agriculture and forestry',
       'Oil and gas extraction', 'Coal mining',
       'Copper, nickel, lead, and zinc mining',
       'Iron, gold, silver, and other metal ore mining',
       'Stone mining and quarrying',
       'Other nonmetallic mineral mining and quarrying',
       'Drilling oil and gas wells',
       'Electric power generation, transmission, and distribution',
       'Natural gas distribution', 'Water, sewage and other systems',
       'Office and commercial structures',
       'Dog and cat food manufacturing',
       'Other animal food manufacturing',
       'Flour milling and malt manufacturing', 'Wet corn milling',
       'Fats and oils refining and blending',
       'Breakfast cereal manufacturing',
       'Sugar and confectionery product manufacturing',
       'Frozen food manufacturing',
       'Fruit and vegetable canning, pickling, and drying',
       'Cheese manufacturing',
       'Dry, condensed, and evaporated dairy product manufacturing',
       'Fluid milk and butter manufacturing',
       'Ice cream and frozen dessert manufacturing', 'Poultry processing',
       'Animal (except poultry) slaughtering, rendering, and processing',
       'Seafood product preparation and packaging',
       'Bread and bakery product manufacturing',
       'Cookie, cracker, pasta, and tortilla manufacturing',
       'Snack food manufacturing', 'Coffee and tea manufacturing',
       'Flavoring syrup and concentrate manufacturing',
       'Seasoning and dressing manufacturing',
       'All other food manufacturing', 'Soft drink and ice manufacturing',
       'Breweries', 'Wineries', 'Distilleries',
       'Tobacco product manufacturing', 'Fiber, yarn, and thread mills',
       'Fabric mills',
       'Textile and fabric finishing and fabric coating mills',
       'Carpet and rug mills', 'Curtain and linen mills',
       'Other textile product mills', 'Apparel manufacturing',
       'Leather and allied product manufacturing',
       'Sawmills and wood preservation',
       'Veneer, plywood, and engineered wood product manufacturing',
       'Millwork', 'All other wood product manufacturing', 'Pulp mills',
       'Paper mills', 'Paperboard mills',
       'Paperboard container manufacturing',
       'Paper Bag and Coated and Treated Paper Manufacturing',
       'Stationery product manufacturing',
       'Sanitary paper product manufacturing',
       'All other converted paper product manufacturing', 'Printing',
       'Support activities for printing', 'Petroleum refineries',
       'Asphalt paving mixture and block manufacturing',
       'Asphalt shingle and coating materials manufacturing',
       'Other petroleum and coal products manufacturing',
       'Petrochemical manufacturing', 'Industrial gas manufacturing',
       'Synthetic dye and pigment manufacturing',
       'Other Basic Inorganic Chemical Manufacturing',
       'Other basic organic chemical manufacturing',
       'Plastics material and resin manufacturing',
       'Synthetic rubber and artificial and synthetic fibers and filaments manufacturing',
       'Fertilizer manufacturing',
       'Pesticide and other agricultural chemical manufacturing',
       'Medicinal and botanical manufacturing',
       'Pharmaceutical preparation manufacturing',
       'In-vitro diagnostic substance manufacturing',
       'Biological product (except diagnostic) manufacturing',
       'Paint and coating manufacturing', 'Adhesive manufacturing',
       'Soap and cleaning compound manufacturing',
       'Toilet preparation manufacturing', 'Printing ink manufacturing',
       'All other chemical product and preparation manufacturing',
       'Plastics packaging materials and unlaminated film and sheet manufacturing',
       'Plastics pipe, pipe fitting, and unlaminated profile shape manufacturing',
       'Laminated plastics plate, sheet (except packaging), and shape manufacturing',
       'Polystyrene foam product manufacturing',
       'Urethane and other foam product (except polystyrene) manufacturing',
       'Plastics bottle manufacturing',
       'Other plastics product manufacturing', 'Tire manufacturing',
       'Rubber and plastics hoses and belting manufacturing',
       'Other rubber product manufacturing',
       'Clay product and refractory manufacturing',
       'Glass and glass product manufacturing', 'Cement manufacturing',
       'Ready-mix concrete manufacturing',
       'Concrete pipe, brick, and block manufacturing',
       'Other concrete product manufacturing',
       'Lime and gypsum product manufacturing',
       'Abrasive product manufacturing',
       'Cut stone and stone product manufacturing',
       'Ground or treated mineral and earth manufacturing',
       'Mineral wool manufacturing',
       'Miscellaneous nonmetallic mineral products',
       'Iron and steel mills and ferroalloy manufacturing',
       'Steel product manufacturing from purchased steel',
       'Secondary smelting and alloying of aluminum',
       'Aluminum product manufacturing from purchased aluminum',
       'Copper rolling, drawing, extruding and alloying',
       'Nonferrous metal (except copper and aluminum) rolling, drawing, extruding and alloying',
       'Ferrous metal foundries', 'Nonferrous metal foundries',
       'Custom roll forming', 'Cutlery and handtool manufacturing',
       'Plate work and fabricated structural product manufacturing',
       'Ornamental and architectural metal products manufacturing',
       'Power boiler and heat exchanger manufacturing',
       'Metal tank (heavy gauge) manufacturing',
       'Metal can, box, and other metal container (light gauge) manufacturing',
       'Hardware manufacturing', 'Spring and wire product manufacturing',
       'Turned product and screw, nut, and bolt manufacturing',
       'Coating, engraving, heat treating and allied activities',
       'Plumbing fixture fitting and trim manufacturing',
       'Valve and fittings other than plumbing',
       'Ball and roller bearing manufacturing',
       'Fabricated pipe and pipe fitting manufacturing',
       'Ammunition, arms, ordnance, and accessories manufacturing',
       'Farm machinery and equipment manufacturing',
       'Lawn and garden equipment manufacturing',
       'Construction machinery manufacturing',
       'Mining and oil and gas field machinery manufacturing',
       'Semiconductor machinery manufacturing',
       'Other industrial machinery manufacturing',
       'Optical instrument and lens manufacturing',
       'Photographic and photocopying equipment manufacturing',
       'Other commercial and service industry machinery manufacturing',
       'Industrial and commercial fan and blower and air purification equipment manufacturing',
       'Heating equipment (except warm air furnaces) manufacturing',
       'Air conditioning, refrigeration, and warm air heating equipment manufacturing',
       'Industrial mold manufacturing',
       'Special tool, die, jig, and fixture manufacturing',
       'Cutting and machine tool accessory, rolling mill, and other metalworking machinery manufacturing',
       'Turbine and turbine generator set units manufacturing',
       'Speed changer, industrial high-speed drive, and gear manufacturing',
       'Mechanical power transmission equipment manufacturing',
       'Other engine equipment manufacturing',
       'Air and gas compressor manufacturing',
       'Pump and pumping equipment manufacturing',
       'Material handling equipment manufacturing',
       'Power-driven handtool manufacturing',
       'Packaging machinery manufacturing',
       'Industrial process furnace and oven manufacturing',
       'Other general purpose machinery manufacturing',
       'Fluid power process machinery',
       'Electronic computer manufacturing',
       'Computer storage device manufacturing',
       'Computer terminals and other computer peripheral equipment manufacturing',
       'Telephone apparatus manufacturing',
       'Broadcast and wireless communications equipment',
       'Other communications equipment manufacturing',
       'Audio and video equipment manufacturing',
       'Semiconductor and related device manufacturing',
       'Printed circuit assembly (electronic assembly) manufacturing',
       'Other electronic component manufacturing',
       'Electromedical and electrotherapeutic apparatus manufacturing',
       'Search, detection, and navigation instruments manufacturing',
       'Automatic environmental control manufacturing',
       'Industrial process variable instruments manufacturing',
       'Totalizing fluid meter and counting device manufacturing',
       'Electricity and signal testing instruments manufacturing',
       'Analytical laboratory instrument manufacturing',
       'Irradiation apparatus manufacturing',
       'Watch, clock, and other measuring and controlling device manufacturing',
       'Manufacturing and reproducing magnetic and optical media',
       'Electric lamp bulb and part manufacturing',
       'Lighting fixture manufacturing',
       'Small electrical appliance manufacturing',
       'Household cooking appliance manufacturing',
       'Household refrigerator and home freezer manufacturing',
       'Household laundry equipment manufacturing',
       'Other major household appliance manufacturing',
       'Power, distribution, and specialty transformer manufacturing',
       'Motor and generator manufacturing',
       'Switchgear and switchboard apparatus manufacturing',
       'Relay and industrial control manufacturing',
       'Storage battery manufacturing', 'Primary battery manufacturing',
       'Communication and energy wire and cable manufacturing',
       'Wiring device manufacturing',
       'Carbon and graphite product manufacturing',
       'All other miscellaneous electrical equipment and component manufacturing',
       'Automobile manufacturing',
       'Light truck and utility vehicle manufacturing',
       'Heavy duty truck manufacturing',
       'Motor vehicle body manufacturing', 'Truck trailer manufacturing',
       'Motor home manufacturing',
       'Travel trailer and camper manufacturing',
       'Motor vehicle gasoline engine and engine parts manufacturing',
       'Motor vehicle electrical and electronic equipment manufacturing',
       'Motor vehicle transmission and power train parts manufacturing',
       'Motor vehicle seating and interior trim manufacturing',
       'Motor vehicle metal stamping',
       'Other Motor Vehicle Parts Manufacturing',
       'Motor vehicle steering, suspension component (except spring), and brake systems manufacturing',
       'Aircraft manufacturing',
       'Aircraft engine and engine parts manufacturing',
       'Other aircraft parts and auxiliary equipment manufacturing',
       'Guided missile and space vehicle manufacturing',
       'Railroad rolling stock manufacturing',
       'Ship building and repairing', 'Boat building',
       'Motorcycle, bicycle, and parts manufacturing',
       'Military armored vehicle, tank, and tank component manufacturing',
       'All other transportation equipment manufacturing',
       'Wood kitchen cabinet and countertop manufacturing',
       'Upholstered household furniture manufacturing',
       'Nonupholstered wood household furniture manufacturing',
       'Institutional furniture manufacturing',
       'Showcase, partition, shelving, and locker manufacturing',
       'Office furniture and custom architectural woodwork and millwork manufacturing',
       'Other furniture related product manufacturing',
       'Surgical and medical instrument manufacturing',
       'Surgical appliance and supplies manufacturing',
       'Dental equipment and supplies manufacturing',
       'Ophthalmic goods manufacturing',
       'Jewelry and silverware manufacturing',
       'Sporting and athletic goods manufacturing',
       'Doll, toy, and game manufacturing',
       'Office supplies (except paper) manufacturing',
       'Sign manufacturing', 'All other miscellaneous manufacturing',
       'Motor vehicle and parts dealers', 'Air transportation',
       'Rail transportation', 'Water transportation',
       'Truck transportation',
       'Transit and ground passenger transportation',
       'Pipeline transportation', 'Warehousing and storage',
       'Newspaper publishers', 'Periodical Publishers', 'Book publishers',
       'Software publishers', 'Motion picture and video industries',
       'Sound recording industries', 'Radio and television broadcasting',
       'Cable and other subscription programming',
       'Wired telecommunications carriers',
       'Wireless telecommunications carriers (except satellite)',
       'Data processing, hosting, and related services',
       'Internet publishing and broadcasting and Web search portals',
       'News syndicates, libraries, archives and all other information services',
       'Other financial investment activities',
       'Securities and commodity contracts intermediation and brokerage',
       'Insurance agencies, brokerages, and related activities',
       'Funds, trusts, and other financial vehicles',
       'Automotive equipment rental and leasing',
       'Commercial and industrial machinery and equipment rental and leasing',
       'General and consumer goods rental',
       'Accounting, tax preparation, bookkeeping, and payroll services',
       'Specialized design services',
       'Custom computer programming services',
       'Computer systems design services',
       'Management consulting services',
       'Scientific research and development services',
       'Advertising, public relations, and related services',
       'Photographic services', 'Veterinary services',
       'All other miscellaneous professional, scientific, and technical services',
       'Management of companies and enterprises',
       'Office administrative services', 'Facilities support services',
       'Business support services',
       'Travel arrangement and reservation services',
       'Investigation and security services',
       'Services to buildings and dwellings',
       'Waste management and remediation services',
       'Junior colleges, colleges, universities, and professional schools',
       'Offices of physicians', 'Offices of dentists',
       'Offices of other health practitioners', 'Outpatient care centers',
       'Medical and diagnostic laboratories', 'Home health care services',
       'Other ambulatory health care services',
       'Residential mental health, substance abuse, and other residential care facilities',
       'Child day care services', 'Performing arts companies',
       'Spectator sports',
       'Promoters of performing arts and sports and agents for public figures',
       'Gambling industries (except casino hotels)',
       'Other amusement and recreation industries', 'Accommodation',
       'Automotive repair and maintenance',
       'Electronic and precision equipment repair and maintenance',
       'Commercial and industrial machinery and equipment repair and maintenance',
       'Personal and household goods repair and maintenance',
       'Personal care services', 'Death care services',
       'Dry-cleaning and laundry services', 'Other personal services',
       'Private households'], dtype=object)</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=1876f988">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [42]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="nb">len</span><span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">Name</span><span class="o">.</span><span class="n">unique</span><span class="p">())</span> <span class="c1"># Checking number of unique values in 'Name' </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[42]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>713</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=bdf2992b">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Top-10-Emmiting-Industry">Top 10 Emmiting Industry<a class="anchor-link" href="#Top-10-Emmiting-Industry">¶</a></h5>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=e6d299cd-6903-4c2c-b073-a1ac5a304356">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [43]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">top_emitters</span> <span class="o">=</span> <span class="n">df</span><span class="p">[[</span><span class="s1">'Name'</span><span class="p">,</span> <span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">]]</span><span class="o">.</span><span class="n">groupby</span><span class="p">(</span><span class="s1">'Name'</span><span class="p">)</span><span class="o">.</span><span class="n">mean</span><span class="p">()</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span>
    <span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">,</span> <span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">10</span><span class="p">)</span> 

<span class="c1"># Resetting index for better plotting</span>
<span class="n">top_emitters</span> <span class="o">=</span> <span class="n">top_emitters</span><span class="o">.</span><span class="n">reset_index</span><span class="p">()</span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d63dd05f-6cc0-4291-bc22-afd854999e29">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [44]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">top_emitters</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[44]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Name</th>
<th>Supply Chain Emission Factors with Margins</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>Cement manufacturing</td>
<td>1.686179</td>
</tr>
<tr>
<th>1</th>
<td>Cement</td>
<td>1.324964</td>
</tr>
<tr>
<th>2</th>
<td>Electric power generation, transmission, and d...</td>
<td>1.220357</td>
</tr>
<tr>
<th>3</th>
<td>Electricity</td>
<td>1.016143</td>
</tr>
<tr>
<th>4</th>
<td>Dolls, toys, and games</td>
<td>0.832179</td>
</tr>
<tr>
<th>5</th>
<td>Lime and gypsum products</td>
<td>0.816536</td>
</tr>
<tr>
<th>6</th>
<td>Lime and gypsum product manufacturing</td>
<td>0.799679</td>
</tr>
<tr>
<th>7</th>
<td>Industrial gas manufacturing</td>
<td>0.612929</td>
</tr>
<tr>
<th>8</th>
<td>Compressed Gases</td>
<td>0.539679</td>
</tr>
<tr>
<th>9</th>
<td>Clothing</td>
<td>0.468714</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d42f181c-dc8d-45ce-9b16-65a0eb655c57">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [46]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Plotting the top 10 emitting industries</span>


<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">10</span><span class="p">,</span><span class="mi">6</span><span class="p">))</span>
<span class="c1"># Example: Top emitting industries (already grouped)</span>
<span class="n">sns</span><span class="o">.</span><span class="n">barplot</span><span class="p">(</span>
    <span class="n">x</span><span class="o">=</span><span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">,</span>
    <span class="n">y</span><span class="o">=</span><span class="s1">'Name'</span><span class="p">,</span>
    <span class="n">data</span><span class="o">=</span><span class="n">top_emitters</span><span class="p">,</span>
    <span class="n">hue</span><span class="o">=</span><span class="s1">'Name'</span><span class="p">,</span>
    <span class="n">palette</span><span class="o">=</span><span class="s1">'viridis'</span>  <span class="c1"># Use 'Blues', 'viridis', etc., for other color maps</span>
<span class="p">)</span>

<span class="c1"># Add ranking labels (1, 2, 3...) next to bars</span>
<span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="p">(</span><span class="n">value</span><span class="p">,</span> <span class="n">name</span><span class="p">)</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="nb">zip</span><span class="p">(</span><span class="n">top_emitters</span><span class="p">[</span><span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">],</span> <span class="n">top_emitters</span><span class="o">.</span><span class="n">index</span><span class="p">),</span> <span class="n">start</span><span class="o">=</span><span class="mi">1</span><span class="p">):</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">text</span><span class="p">(</span><span class="n">value</span> <span class="o">+</span> <span class="mf">0.01</span><span class="p">,</span> <span class="n">i</span> <span class="o">-</span> <span class="mi">1</span><span class="p">,</span> <span class="sa">f</span><span class="s1">'#</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">'</span><span class="p">,</span> <span class="n">va</span><span class="o">=</span><span class="s1">'center'</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">11</span><span class="p">,</span> <span class="n">fontweight</span><span class="o">=</span><span class="s1">'bold'</span><span class="p">,</span> <span class="n">color</span><span class="o">=</span><span class="s1">'black'</span><span class="p">)</span>

<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s1">'Top 10 Emitting Industries'</span><span class="p">,</span> <span class="n">fontsize</span><span class="o">=</span><span class="mi">14</span><span class="p">,</span> <span class="n">fontweight</span><span class="o">=</span><span class="s1">'bold'</span><span class="p">)</span> <span class="c1"># Title of the plot </span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s1">'Emission Factor (kg CO2e/unit)'</span><span class="p">)</span> <span class="c1"># X-axis label</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s1">'Industry'</span><span class="p">)</span> <span class="c1"># Y-axis label</span>
<span class="n">plt</span><span class="o">.</span><span class="n">grid</span><span class="p">(</span><span class="n">axis</span><span class="o">=</span><span class="s1">'x'</span><span class="p">,</span> <span class="n">linestyle</span><span class="o">=</span><span class="s1">'--'</span><span class="p">,</span> <span class="n">alpha</span><span class="o">=</span><span class="mf">0.6</span><span class="p">)</span> <span class="c1"># Adding grid lines for better readability</span>
<span class="n">plt</span><span class="o">.</span><span class="n">tight_layout</span><span class="p">()</span> <span class="c1"># Adjust layout to prevent overlap</span>

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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAA94AAAJOCAYAAABBfN/cAAAAOnRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjEwLjEsIGh0dHBzOi8vbWF0cGxvdGxpYi5vcmcvc2/+5QAAAAlwSFlzAAAPYQAAD2EBqD+naQAAwfNJREFUeJzs3Qd4U2X7BvAnbSll702ZskWmbGULiiguUNwL/RBREQURFVBcICoOVETAhQMFcYAoAiJDkWVRNiKoIDJbRhnt+V/3+31v/qchbZO2aZs89++6QkmbJuc+SZPzvOt4HMdxhIiIiIiIiIhCIio0d0tEREREREREwMKbiIiIiIiIKIRYeBMRERERERGFEAtvIiIiIiIiohBi4U1EREREREQUQiy8iYiIiIiIiEKIhTcRERERERFRCLHwJiIiIiIiIgohFt5EREREREREIcTCm4iIiIjyzKJFi8Tj8XgvO3bsCMnj1KhRw/sYo0aNCsljhBvsB7tPsH/CWSRlocjEwpuIiIjClruYCvSCQi8/mDx5stxyyy3SuHFjiYmJCbhoSElJkddff106dOggpUqVkkKFCkmdOnXknnvukd27dwe1DTfddFO+3meBFuWRUlT7Ph+RDs9nfnidEeWGmFx5FCIiIiJK44EHHpDDhw8H9TvJycly6aWXyvz589N8f+vWrTJx4kR599135euvv5aWLVtKuKhdu7aMGzfOe7106dIheZyHH37Yu7/btWsXksegvHPBBRdI0aJFzf9LlCiR15tDdAYW3kRERBS23MUUHDx4UJ588knv9e7du5sDct9CLz+Ijo6WBg0amCI5ISFB1q5dG1BeW3Tj99FjXqlSJZk2bZrs3LlTDhw4IFdddZWsX79eihQpEvQ2uQvg3Npn8fHxMnToUAm122+/PeSPQbkvMTFRihcvbhpT2KBC+ZpDREREFCF+//13B4c39vLYY4+dcZvTp087U6ZMcbp06eKUKVPGiYmJcUqXLu106tTJeeONN5xTp05leJ8LFy503n77bad58+ZOXFycU65cOefmm2929uzZE9S2Hjt2zPv/G2+80Xv/1atX93v7/fv3OwULFvTebsSIEd6fbdy40fF4PN6fvfrqqwFtg/txAz0sxD51b+vff//t3HDDDWZfFitWzLn44oudTZs2mduuWrXK6dGjh1O0aFGnZMmSzpVXXuns3Lkzzf1hf7q3Afsb3N/zd8G2+26/v4uFbfX3uvB9/G3btjmvvPKK07hxY7O/8fzeeuutzoEDB87YF0ePHnWGDx/uxMfHm9s2bNjQmTRpkrN9+/YzXjPZfT7cP+vYsaPZ77fffrtTsWJFJzY21qlfv755/frzyy+/OL169TLPDy54TvDc+D6Xbu7tmDp1aobb4vtY1157rbk/bBf+RrB/OnfubPbVn3/+ecbz4e9i79ff39+bb77pNGvWzNx3kyZNzO0yygKHDx92nnzySadVq1ZO8eLFnQIFCpjtQpb169efcXu8Dzz//PNOmzZtnBIlSjjR0dHmfQLP8fXXX+/MmDEjoOeUyGLhTURERGoK7yNHjjjnn39+hgf8HTp0cJKSktK9TxTs/n6vVq1azt69e7O03YEU3jjQdz8eCic3FIr2Zz179syVwhuFSI0aNc7YFyhWZ82alaahwF7q1KnjHD9+PN8W3nj+/d0PXjduJ0+edM477zy/t+3du3dIC2+81ipVquT3sdGo5LZy5UrT8OF7OxStXbt2zdHC+9dff3UKFy6c4fMxd+7cbBXevvs8kMJ78+bNfl+n9oLX6UcffZThc+F7ad26dUDPKZHFoeZERESkxuDBg+X777/3Xscw9LZt28qKFSvM3Gj44YcfzO3eeustv/fx3XffSefOneW8886TpUuXyoIFC8z3t2/fLsOGDUv397Lrl19+SXO9Vq1aZ1zHkHV/tw3U+PHjz/ge5sumN0wbQ9uPHz9uFnY7evSovPnmm+b7//77r1x22WVmzu2gQYPkjz/+kJkzZ5qfbdmyRWbPni1XX311psPet23bJq+99pr3eyNGjDALysHZZ5/t/YrpBZhmkN70gmDg+e/atasZtozttPsUrxu8Ttq0aWOuv/jii7JkyRLv751zzjlm/v26detkzpw5Ekp4rcXFxcl//vMfs7jepEmTzPMAzz77rJmCAKif8f8jR46Y61jArH///mYxuk8++cT72s0p06dPl2PHjpn/V61aVa677joz5eHPP/800x+w/9zTJrC4mntqyJ133umd1oApCP5gn1evXl2uuOIKKVy4sOzduzfTxQjxWrQL85UrV87sA6wlgL/5ZcuWyYkTJ+SGG26QFi1amL8j7C+sl2DhsZo3b26mteC1vHjx4mzuKVLJW4ITERERRXCP9759+8xw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N998k+Z2uN6vXz+Jj483P8elTZs2WXrMmBzZciIiIiIiIqIw8OOPP8rJkyelQ4cO5vrixYslJiZG2rVrl+Z2X375pXz00Uc58pjs8SYiCgNLly6Vxo0bS4ECBaRPnz6SH6EVePbs2Xm9GUREREQZWrJkifnqLrybNWsmRYoUSXO7li1bytNPPy3ff/+9ZBd7vIkoQ3v27JGxY8eaFr+//vpLypcvL02bNpV7771XunbtKvldp06dzPa+8MILEs6GDBlicsydO1eKFi2aY4XyrFmzcqyQ3717t5QqVUrygpPqiOT9yLVczbvnj4P/za2ExszA3Hpya8wMzK0nt5PHmXfs2CE1a9ZM870mTZp4/799+3ZzbNSxY0dZtGiR+d51112XY4/PwpuIMnyDat++vZQsWVLGjRtnelxPnTolX3/9tdx1112ycePGvN5ENbZt2yZ33nmnVK1aVfIbDNWKjY2VihUr5tk2pKY6Eh0taiDvlrV/iyYaMwNz66ExMzC3HqkKM7txqDkRpWvgwIGm5e+nn36SK664QurWrSuNGjUyva8rVqzw3u7QoUNy2223Sbly5cypFLp06SLr1q3z/nzUqFGmt/att96SatWqmR5b3HdKSoo8++yzpmBDTzp61t0Cvd933nlHatSoYU7ncPXVV0tSUpL5+U033WSGDr344oveBTHQmOAPfv+JJ56QG264wWxf9erVZc6cOfLvv//KpZdear53zjnnyM8//+z9nf3798s111wjVapUkcKFC5uGiRkzZpzR4z548GB58MEHpXTp0iYrttvC9mC71q5dmyY3vofWVvtzPNYtt9xi/j9t2jSz72699VbTcluoUCGpV6+eyekL+xzPGRYQqVSpkgwaNMibFy677DJzn/Y69plvDzhGNyCHOxPuB98vW7as9OjR44yh5na7P/30U+ncubPZP2hVXr58eZr7njx5slmwBD/HtkyYMME09AQrPyzUkpuQt07Tyqpya8wMzK0nt8bMwNx6ckflcWYc6+BM2ps3bzbXR44caa6PGDHCXEeHEq7b3u6cxsKbiPw6cOCAzJs3z/Rs+853AXdxdNVVV8nevXvNMOhVq1ZJ8+bNzTB03Ie7xxY/x32iOJ0yZYr06tVL/vzzT1McP/PMM+YNEItdBHu/KPa++OILc8F9YS4OoBBt27at3H777WYYNC4o8tLz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hZnddDY3EBFRRPE4uipvO98ZX7XQmBmw+m9CQoK6VYA15taYGZhbT+4UhZnddH16ERERRQhtBajWzKD1IFVjbo2Zgbn1SFGY2dL5CUZERERERESUS1h4ExEREREREYUQC28iIgp7Glc131/4N1UrfGvMDFj9t169eupWAdaYW2NmYG49uaMUZnbTmZqIiCjMpXhOijYaM0NsbKxopDG3xszA3HrEKsxssfAmIqKw51F2PjGP/G+Fb0Uf4xozQ2pqqlkFGF810ZhbY2Zgbj25UxVmdtP16UVERERERESUy1h4ExEREREREYUQC28iIiKiXHb8+HEpWLCg9O/f31yfPn26eDwe+eabb9LcznEcef/996VJkyYSFxcnpUuXlssvv1w2bNiQR1tORERZEZPXG0BERJRdGlc131tkraoVviMt848//ignT56UDh06mOuLFy+WmJgYadeuXZrb/ec//5E333zTe/3EiRMya9YsWbhwoSxbtkwaNGggkQirHjdu3FjV6scaMwNz68kdpTCzm87UREQRbtq0aVKyZMm83gwKoWhH38qwkZR5yZIl5qu78G7WrJkUKVLEe5t169Z5i+6uXbvK/v375eeff5ZixYrJoUOH5N5775VIhoYJbTRmBubW46TCzBYLbyLKd/bs2SN333231KpVywzFjI+Pl969e8uCBQvyetMiDnrNLr74YilXrpwZxlq7dm3p16+ffP/99xJONK5qXuZYQ1UrfEdC5h07dpjh5Lg8+uij5nsYQo7r27dvl5UrV5r/d+rUyfv3ad16661mmHmLFi1MEQ4Ylr53716JRFj1eNOmTapWP9aYGZhbT+5UhZndwvfTi4giEg5McWD53Xffybhx48xpJ+bNmyedO3eWu+66S/KjU6dOSTh69dVXzQF8mTJl5MMPPzQfhhjCiqGu9913X15vHpF6ycnJGf4c87/Xrl2ba9tDRERZx8KbiPKVgQMHmh6fn376Sa644gqpW7euNGrUSIYMGSIrVqzw3m7nzp1y6aWXStGiRaV48eLSt29f+eeff7w/HzVqlDRt2lTeeustqVatmrkd7jslJUWeffZZqVixopQvX17Gjh2b5vHx2JMmTZILL7xQChUqZHrdZ86ceUaPFQrVjh07ml7i9957z/wMQ0Ix3xLfq1+/vils3UOrBg0aJJUqVTI/r169ujz11FPe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"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=9d361b2c">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Drop-non-numeric-columns-not-needed,">Drop non-numeric columns not needed,<a class="anchor-link" href="#Drop-non-numeric-columns-not-needed,">¶</a></h5><h5 id="Alos-drop-Code-and-Year-columns-since-there-is-no-need-of-both-of-the-columns">Alos drop Code and Year columns since there is no need of both of the columns<a class="anchor-link" href="#Alos-drop-Code-and-Year-columns-since-there-is-no-need-of-both-of-the-columns">¶</a></h5>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=35951b28">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [47]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">'Name'</span><span class="p">,</span><span class="s1">'Code'</span><span class="p">,</span><span class="s1">'Year'</span><span class="p">],</span> <span class="n">inplace</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span> 
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d291b8cc">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [48]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[48]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
<th>Source</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>0</td>
<td>0</td>
<td>0.398</td>
<td>0.073</td>
<td>0.47</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>0</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c971f716">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [49]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">shape</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[49]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>(22092, 11)</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=1b2d26da">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Define-features-and-target">Define features and target<a class="anchor-link" href="#Define-features-and-target">¶</a></h5>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=186d33df">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [50]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[50]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Index(['Substance', 'Unit', 'Supply Chain Emission Factors without Margins',
       'Margins of Supply Chain Emission Factors',
       'Supply Chain Emission Factors with Margins',
       'DQ ReliabilityScore of Factors without Margins',
       'DQ TemporalCorrelation of Factors without Margins',
       'DQ GeographicalCorrelation of Factors without Margins',
       'DQ TechnologicalCorrelation of Factors without Margins',
       'DQ DataCollection of Factors without Margins', 'Source'],
      dtype='object')</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs" id="cell-id=b617536e">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [51]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">X</span> <span class="o">=</span> <span class="n">df</span><span class="o">.</span><span class="n">drop</span><span class="p">(</span><span class="n">columns</span><span class="o">=</span><span class="p">[</span><span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">])</span> <span class="c1"># Feature set excluding the target variable</span>
<span class="n">y</span> <span class="o">=</span> <span class="n">df</span><span class="p">[</span><span class="s1">'Supply Chain Emission Factors with Margins'</span><span class="p">]</span> <span class="c1"># Target variable </span>
</pre></div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=b4d5d358-18ed-4e1c-b205-4e3a42801fbe">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [52]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">X</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[52]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
<th>Source</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>0</td>
<td>0</td>
<td>0.398</td>
<td>0.073</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>0</td>
</tr>
<tr>
<th>1</th>
<td>1</td>
<td>0</td>
<td>0.001</td>
<td>0.001</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>1</td>
<td>1</td>
<td>0</td>
</tr>
<tr>
<th>2</th>
<td>2</td>
<td>0</td>
<td>0.002</td>
<td>0.000</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>0</td>
</tr>
<tr>
<th>3</th>
<td>3</td>
<td>1</td>
<td>0.002</td>
<td>0.000</td>
<td>3</td>
<td>3</td>
<td>1</td>
<td>3</td>
<td>1</td>
<td>0</td>
</tr>
<tr>
<th>4</th>
<td>0</td>
<td>0</td>
<td>0.659</td>
<td>0.081</td>
<td>4</td>
<td>3</td>
<td>1</td>
<td>4</td>
<td>1</td>
<td>0</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=582fb8e6-c355-49f2-86ca-4570666a01c3">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [53]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">y</span><span class="o">.</span><span class="n">head</span><span class="p">()</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[53]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>0    0.470
1    0.002
2    0.002
3    0.002
4    0.740
Name: Supply Chain Emission Factors with Margins, dtype: float64</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=ccf683ba">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Univariate-Analysis">Univariate Analysis<a class="anchor-link" href="#Univariate-Analysis">¶</a></h3>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c5d0741f">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [54]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Count plot for Substance</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="mi">3</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s2">"Substance"</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Count Plot: Substance"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xticks</span><span class="p">()</span>
<span class="n">plt</span><span class="o">.</span><span class="n">tight_layout</span><span class="p">()</span>
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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=c93c726a">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [55]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Count plot for Unit</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="mi">3</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s2">"Unit"</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Count Plot: Unit"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">tight_layout</span><span class="p">()</span>
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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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+HRoUo0bN5ajR4/a21dffWWfGzFihHz66aeydOlS2bBhgxw5ckT+8Y9/2OezsrJMYDp79qxs2rRJFi5caALRhAkT7DLJycmmTKdOnWT79u0yfPhwefjhh+Xzzz+/6vcKAAB8l893z5UsWVLCwsKyHU9LS5M33nhDFi9eLLfccos59tZbb0nDhg3lm2++kTZt2sjq1atlz5498sUXX0jVqlUlMjJSJk+eLGPHjjWtWAEBATJv3jypVauWTJs2zVxD36/BbMaMGRITE3PV7xcAAPgmn29p2r9/v1SrVk1q164t9913n+luU4mJiZKZmSnR0dF2We26q169uiQkJJh9fW3atKkJTBYNQunp6bJ79267jPs1rDLWNQAAAHy+pSkqKsp0p9WvX990zcXGxkq7du1k165dkpKSYlqKKlSo4PEeDUh6Tumre2Cyzlvnciujwer06dNSpkyZHOuWkZFhNouWBwAARZdPh6Zu3brZPzdr1syEqBo1asj7779/0TBztcTFxZkQBwAAigef755zp61K9erVk6SkJDPOSQd4nzhxwqOMzp6zxkDp64Wz6az9S5UJCgrKNZiNGzfOjKuytsOHD+fbfQIAAN9TqELTyZMn5cCBAxIeHi6tWrWSUqVKSXx8vH1+3759ZsxT27Ztzb6+fv/993Ls2DG7zJo1a0wgatSokV3G/RpWGesaF6PLE+h13DcAAFB0+XRoevLJJ81SAgcPHjRLBtxxxx3i7+8v9957rwQHB8uAAQNk5MiRsm7dOjMw/KGHHjJhR2fOqS5duphw9MADD8iOHTvMMgLjx483aztp6FGDBw+Wn376ScaMGSN79+6VV155xXT/6XIGAAAAhWJM0y+//GIC0u+//y5VqlSRm2++2SwnoD8rXRagRIkSZlFLHZSts9409Fg0YK1YsUKGDBliwlS5cuWkf//+MmnSJLuMLjewcuVKE5JmzZol1157rbz++ussNwAAADz4uVwul+ch5IXOntPWLx3fVJBddTxmAfDtxyxcCX6/Ae/8fjv9G+7T3XMAAAC+gtAEAADgAKEJAADAAUITAACAA4QmAAAABwhNAAAADhCaAAAAHCA0AQAAOEBoAgAAcIDQBAAA4AChCQAAwAFCEwAAgAOEJgAAAAcITQAAAA4QmgAAABwgNAEAADhAaAIAAHCA0AQAAOAAoQkAAKCwh6a4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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=93ea7160">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [56]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Count plot for Source</span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">6</span><span class="p">,</span> <span class="mi">4</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">countplot</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">df</span><span class="p">[</span><span class="s2">"Source"</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Count Plot: Source (Industry vs Commodity)"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">tight_layout</span><span class="p">()</span>
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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAk0AAAGGCAYAAABmPbWyAAAAOnRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjEwLjEsIGh0dHBzOi8vbWF0cGxvdGxpYi5vcmcvc2/+5QAAAAlwSFlzAAAPYQAAD2EBqD+naQAANulJREFUeJzt3Qm8zPX+x/HPsR6RfS9JqyVRh6SiLJfWm9ItpSjSRiVFSEopNyJEljYUN7lFpRKX0EXRkSwhlW5aLCVE2ef/eH8f/988ZuZs33Oc48w5Xs/HYxzzm+/85je/+c1v3vPdJiEUCoUMAAAA6SqQ/s0AAAAQQhMAAIAHQhMAAIAHQhMAAIAHQhMAAIAHQhMAAIAHQhMAAIAHQhMAAIAHQhMAAIAHQhOQQ04++WS79dZbc3szjlmDBw+2mjVr2uHDh3P0cS655BJ3AY7EhAkTLCEhwb7//vscPbbOP/9869WrV7au81hCaEKO+vbbb+3OO++0U045xRITE61kyZJ24YUX2ogRI+yvv/6yePDCCy+4E5YvndiCS4ECBaxq1arWqlUrmz9/frZsz88//2yPP/64rVix4ojX9d5779nFF19sFStWtOOOO869Dtdff73NmjXL8rNdu3bZM888Yw8//LB7jQJ6zbp162Z5ydNPP20zZsyw/EbH980332zVqlWzokWLWtmyZa1ly5b26quv2qFDh3J78+JSdpwb9J4YPXq0bd68OVu37VhBaEKOef/9961u3br25ptv2lVXXWXPP/+8DRo0yE466STr2bOn3X///ZYXQ5P87W9/s9dee80mTpxod911l61cudKaN29uH374YbacGAcMGHDEoenZZ5+1v//97y4o9OnTx5577jlr27atbdiwwd544w3Lz1555RU7ePCg3XjjjZbX5cfQ9NJLL1mDBg3s448/tvbt27v3YP/+/a1YsWLWuXNnF3hhNnv2bHfJznPD1Vdf7b68ap8j8wpl4T5AhjZu3Gjt2rWz6tWr27x586xKlSrh27p27WrffPONC1V51RlnnOG+JQeuueYaO/vss2348OF22WWXWW5TYHjyySdduIs86Qa2bt161Ldpz549Vrx48aPyWKqtUGBU7eax5Gju46z69NNP3ReNxo0b2wcffGDHH398+Lbu3bvb559/bqtXr87VbYwXRYoUyfZ1qub1uuuus0mT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8i/e48eOUunUMAUITRFUc9SxY0dr0KCBnXfeeTZ8+HDbs2ePG00HAACObYSmCDfccINt27bN+vfvb5s3b7b69evbrFmzUnQOBwAAxx5CUww1xaXWHAdEUtOsJkGNbaIFkD/wHkdqEkIZja8DAAAAk1sCAAD4IDQBAAB4IDQBAAB4IDQBWTB69Gg7+eSTLTEx0Ro1amRLly7N7U0CkA0WLlxoV111lZvkUBMVz5gxI7c3CXGE0ARk0tSpU92cXhpZs3z5cqtXr561bt3atm7dmtubBuAIaW4+vaf1xQiIxeg5IJNUs9SwYUMbNWpUeOZ4/dzCvffea717987tzQOQTVTTNH369PCvRADUNAGZsH//fktOTraWLVuGlxUoUMBdX7JkSa5uGwAgZxGagEz49ddf7dChQylmidd1zSIPAMi/CE0AAAAeCE1AJpQvX94KFixoW7ZsiVqu65UrV8617QIA5DxCE5AJRYoUsaSkJJs7d254mTqC63rjxo1zddsAADmLH+wFMknTDXTs2NEaNGhg5513ng0fPtwNU77ttttye9MAHKHdu3fbN998E76+ceNGW7FihZUtW9ZOOumkXN025D6mHACyQNMNDBkyxHX+rl+/vo0cOdJNRQAgb5s/f741a9YsxXJ9UZowYUKubBPiB6EJAADAA32aAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAAAAPBCaAOQ727Zts7vvvtv9VljRokWtcuXK1rp1a1u0aFFubxqAPIwf7AWQ77Rt29b2799vEydOtFNOOcW2bNlic+fOtd9++y3HHlOPV6RIkRxbP4DcR00TgHxlx44d9sknn9gzzzzjfni1evXqdt5551mfPn3s73//uyvzww8/2NVXX20lSpSwkiVL2vXXX++CVeDWW2+1Nm3aRK23e/fudskll4Sv6//dunVzy8uXL+9qsmTNmjV25ZVXuvUef/zx1qRJE/v222/D93vppZesVq1alpiYaDVr1rQXXnjhKOwVANmB0AQgX1EQ0mXGjBm2b9++FLcfPnzYBabt27fbggULbM6cOfbdd9/ZDTfckOnHUk2WapfU7Dd27Fj76aefrGnTpq5JcN68eZacnGydOnWygwcPuvKTJ0+2/v3721NPPWVr1661p59+2h599FG3HgDxj+Y5APlKoUKFbMKECdalSxcXZM4991y7+OKLrV27dnb22We7ZrpVq1bZxo0brVq1au4+kyZNsjp16tiyZcusYcOG3o91+umn2+DBg8PX+/bta6VKlbI33njDChcu7JadccYZ4dsfe+wxGzp0qF177bXueo0aNeyrr76ycePGWceOHbNxLwDICdQ0AciXfZp+/vlne/fdd+3SSy+1+fPnu/CkMKUaHoWlIDBJ7dq1rXTp0u62zEhKSoq6vmLFCtccFwSmSHv27HHNdJ07dw7XhukycODAqOY7APGLmiYA+ZL6DP3tb39zFzWB3X777a6m58EHH8zwvgUKFLBQKBS17MCBAynKFS9ePOp6sWLF0lzn7t273d8XX3zRGjVqFHVbwYIFM9wmALmPmiYAxwTVJqm2R52wN23a5C4BNZGpA7nKSIUKFeyXX35JUYuUETX/qRN6agGrUqVKVrVqVdd/6rTTTou6qJkOQPwjNAHIVzStQPPmze3111+3lStXur5L06ZNc32P1AG8ZcuWVrduXWvfvr0tX77cli5dah06dHD9nho0aODWoft//vnnrq/Thg0bXA3V6tWrM3xsjabbtWuX6z+l++u+r732mq1fv97dPmDAABs0aJCNHDnSvv76a9e36tVXX7Vhw4bl+H4BcOQITQDyFfUTUvPXc88950aynXXWWa55Th3DR40aZQkJCfbOO+9YmTJl3O0KUZrLaerUqeF1aPoA3adXr16uY/gff/zhglVGypUr50bNqSlOIUx9ntQcF/RxUhOhphxQUFJwUxn1s6KmCcgbEkKxDfcAAABIgZomAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAD4QmAAAAy9j/AV70rLZr2WGTAAAAAElFTkSuQmCC"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=d10c7c37">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [57]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">columns</span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[57]:</div>
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>Index(['Substance', 'Unit', 'Supply Chain Emission Factors without Margins',
       'Margins of Supply Chain Emission Factors',
       'Supply Chain Emission Factors with Margins',
       'DQ ReliabilityScore of Factors without Margins',
       'DQ TemporalCorrelation of Factors without Margins',
       'DQ GeographicalCorrelation of Factors without Margins',
       'DQ TechnologicalCorrelation of Factors without Margins',
       'DQ DataCollection of Factors without Margins', 'Source'],
      dtype='object')</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=6b253a95">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="Multivariate-Anslysis">Multivariate Anslysis<a class="anchor-link" href="#Multivariate-Anslysis">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell" id="cell-id=50f3c914">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h5 id="Correlation-heatmap">Correlation heatmap<a class="anchor-link" href="#Correlation-heatmap">¶</a></h5>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=12ee4cb4">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [58]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">number</span><span class="p">)</span><span class="o">.</span><span class="n">corr</span><span class="p">()</span> <span class="c1"># Checking correlation between numerical features </span>
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
<div class="jp-OutputPrompt jp-OutputArea-prompt">Out[58]:</div>
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Substance</th>
<th>Unit</th>
<th>Supply Chain Emission Factors without Margins</th>
<th>Margins of Supply Chain Emission Factors</th>
<th>Supply Chain Emission Factors with Margins</th>
<th>DQ ReliabilityScore of Factors without Margins</th>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<th>DQ DataCollection of Factors without Margins</th>
<th>Source</th>
</tr>
</thead>
<tbody>
<tr>
<th>Substance</th>
<td>1.000000e+00</td>
<td>7.745967e-01</td>
<td>-0.391851</td>
<td>-0.218400</td>
<td>-0.421603</td>
<td>0.095092</td>
<td>-3.666436e-15</td>
<td>NaN</td>
<td>0.198415</td>
<td>NaN</td>
<td>4.286684e-16</td>
</tr>
<tr>
<th>Unit</th>
<td>7.745967e-01</td>
<td>1.000000e+00</td>
<td>-0.155859</td>
<td>-0.094300</td>
<td>-0.169741</td>
<td>-0.025159</td>
<td>-3.151462e-17</td>
<td>NaN</td>
<td>0.286990</td>
<td>NaN</td>
<td>-1.600623e-17</td>
</tr>
<tr>
<th>Supply Chain Emission Factors without Margins</th>
<td>-3.918505e-01</td>
<td>-1.558594e-01</td>
<td>1.000000</td>
<td>0.143005</td>
<td>0.962971</td>
<td>-0.098000</td>
<td>9.283870e-03</td>
<td>NaN</td>
<td>0.148410</td>
<td>NaN</td>
<td>2.713112e-02</td>
</tr>
<tr>
<th>Margins of Supply Chain Emission Factors</th>
<td>-2.184002e-01</td>
<td>-9.429989e-02</td>
<td>0.143005</td>
<td>1.000000</td>
<td>0.404541</td>
<td>-0.069598</td>
<td>7.953109e-03</td>
<td>NaN</td>
<td>0.086335</td>
<td>NaN</td>
<td>-6.750426e-02</td>
</tr>
<tr>
<th>Supply Chain Emission Factors with Margins</th>
<td>-4.216032e-01</td>
<td>-1.697410e-01</td>
<td>0.962971</td>
<td>0.404541</td>
<td>1.000000</td>
<td>-0.109494</td>
<td>1.074848e-02</td>
<td>NaN</td>
<td>0.160574</td>
<td>NaN</td>
<td>6.687828e-03</td>
</tr>
<tr>
<th>DQ ReliabilityScore of Factors without Margins</th>
<td>9.509190e-02</td>
<td>-2.515938e-02</td>
<td>-0.098000</td>
<td>-0.069598</td>
<td>-0.109494</td>
<td>1.000000</td>
<td>-2.170715e-02</td>
<td>NaN</td>
<td>0.073583</td>
<td>NaN</td>
<td>-1.228726e-02</td>
</tr>
<tr>
<th>DQ TemporalCorrelation of Factors without Margins</th>
<td>-3.666436e-15</td>
<td>-3.151462e-17</td>
<td>0.009284</td>
<td>0.007953</td>
<td>0.010748</td>
<td>-0.021707</td>
<td>1.000000e+00</td>
<td>NaN</td>
<td>-0.030607</td>
<td>NaN</td>
<td>-2.898842e-15</td>
</tr>
<tr>
<th>DQ GeographicalCorrelation of Factors without Margins</th>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
</tr>
<tr>
<th>DQ TechnologicalCorrelation of Factors without Margins</th>
<td>1.984154e-01</td>
<td>2.869901e-01</td>
<td>0.148410</td>
<td>0.086335</td>
<td>0.160574</td>
<td>0.073583</td>
<td>-3.060675e-02</td>
<td>NaN</td>
<td>1.000000</td>
<td>NaN</td>
<td>2.827202e-02</td>
</tr>
<tr>
<th>DQ DataCollection of Factors without Margins</th>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
<td>NaN</td>
</tr>
<tr>
<th>Source</th>
<td>4.286684e-16</td>
<td>-1.600623e-17</td>
<td>0.027131</td>
<td>-0.067504</td>
<td>0.006688</td>
<td>-0.012287</td>
<td>-2.898842e-15</td>
<td>NaN</td>
<td>0.028272</td>
<td>NaN</td>
<td>1.000000e+00</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=cca48055">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [59]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="n">df</span><span class="o">.</span><span class="n">info</span><span class="p">()</span> <span class="c1"># Checking data types and non-null counts after mapping </span>
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
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 22092 entries, 0 to 22091
Data columns (total 11 columns):
 #   Column                                                  Non-Null Count  Dtype  
---  ------                                                  --------------  -----  
 0   Substance                                               22092 non-null  int64  
 1   Unit                                                    22092 non-null  int64  
 2   Supply Chain Emission Factors without Margins           22092 non-null  float64
 3   Margins of Supply Chain Emission Factors                22092 non-null  float64
 4   Supply Chain Emission Factors with Margins              22092 non-null  float64
 5   DQ ReliabilityScore of Factors without Margins          22092 non-null  int64  
 6   DQ TemporalCorrelation of Factors without Margins       22092 non-null  int64  
 7   DQ GeographicalCorrelation of Factors without Margins   22092 non-null  int64  
 8   DQ TechnologicalCorrelation of Factors without Margins  22092 non-null  int64  
 9   DQ DataCollection of Factors without Margins            22092 non-null  int64  
 10  Source                                                  22092 non-null  int64  
dtypes: float64(3), int64(8)
memory usage: 1.9 MB
</pre>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell" id="cell-id=a1fb07f5">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In [60]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
<div class="cm-editor cm-s-jupyter">
<div class="highlight hl-ipython3"><pre><span></span><span class="c1"># Correlation matrix </span>
<span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">(</span><span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">12</span><span class="p">,</span> <span class="mi">8</span><span class="p">))</span>
<span class="n">sns</span><span class="o">.</span><span class="n">heatmap</span><span class="p">(</span><span class="n">df</span><span class="o">.</span><span class="n">select_dtypes</span><span class="p">(</span><span class="n">include</span><span class="o">=</span><span class="n">np</span><span class="o">.</span><span class="n">number</span><span class="p">)</span><span class="o">.</span><span class="n">corr</span><span class="p">(),</span> <span class="n">annot</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">cmap</span><span class="o">=</span><span class="s2">"coolwarm"</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">"Correlation Heatmap"</span><span class="p">)</span>
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
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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bBo3bqyCNalElOlSXSeDbEhYJk17Zf8GDx6sAlUJC319fdXgJTmPy8SJE1VffNKHo8yjHyzkQUgYLMFwhw4d1MAt0v/ghAkT1HMcOnTojvnl3JMBYeR1lApBfXg7evToB94WIiKi+8Xgj4iIiIgKLemDTUIYCbqkukoCIAldZATb77//HoMGDcqaV8K54OBgTJ8+HQsXLlSDLXzwwQdqAIkH1aJFC1Xx9dlnn+Hnn39WQZWsX0aQleDKHG9vbzWAhIwuLAN8SAj44osvqqawOUcVfvXVV9UgE1L1Jv3cSZNec8GfNDletWqV2rdRo0apvukk7Pz6669zHbjkYZOQVCrmZPtnzJihXgdpCiuvy+uvv64Gw9APTDJv3jx1TN5++211LIcMGaKazPbv399onbJ/MqDJN998owZ7kf3Mj+BP1jFlyhR89dVXeOONN9Rxk+MnVX+mgj95XglaJei7dOkSqlSpos41OReJiIgKikab3z32EhERERERPUakUnPo0KEq9CUiIrIk7OOPiIiIiIiIiIioCGLwR0REREREREREVAQx+CMiIiIiIiIiIiqCGPwRERERERE9AOk2nf37ERE9fjZt2qQG2ipZsqTq71UGsLqbDRs2oFatWmowMhkpXgaCepgY/BEREREREREREd2jhIQE1KhRAxMmTMjT/OfPn0fnzp3RsmVLHDhwQI0aP3DgQKxevRoPC0f1JSIiIiIiIiIiegBS8bdw4UI8/fTTZud57733sHz5chw5ciRr2gsvvIDo6GisWrUKDwMr/oiIiIiIiIiI6LGXkpKC2NhYo5tMyy/bt29HmzZtjKa1b99eTX9YbB7amomI6LGy3LZiQW+CRak5rFZBb4LF6HX1jYLeBItSsXaFgt4Ei3Jky6GC3gSL8eHoRgW9CRblerRtQW+CxejfqqC3wLLsORlV0JtgUepU9CzoTbAYU/8r6C2wLIX12lGQ3yt2f9QDo0ePNpr2ySef4NNPP82X9V+/fh1+fn5G0+S+BIxJSUlwdHREfmPwR0REREREREREj70PPvgAb731ltE0GYSjMGPwR0REREREREREFkFjqymw57a3t3+oQV/x4sVx48YNo2ly383N7aFU+wn28UdERERERERERPSQNWzYEOvWrTOatnbtWjX9YWHwR0REREREREREdI/i4+Nx4MABdRPnz59X/790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Ls42OHwsBiM+OWxUoedf3FFVcuZVxbIuqHp7VOB/Jhn3+9ZtwA51rhS0mg07Ij42Cqvm/awG6PAPqITB7/+qmvSKqIgwaAx+pAmqUBO9h32NFf+Mx/I5P6FY8QD0HzEOJUpnN0+UQTwWz/xG12TYsxjqNH0S7Z7J7stOvqCeOrwDG1fOVCGjh3dxVK/XFu265t7ENr9IdU7kjXNY9PtCJCVEwdHZA8UDqqHXiFkoVjJ7P6JuXlahoKELJ7apvvqqNzIeREvID3Hdhv2OzYvHYsWMD9SXeGc3H1XN4+xqvpIxPiYc07/QBa1i179T1a10+Xro+Zbu71Rc1HUsnfqWGh3Y0cULpcrWRu93/4GTa94GI6FHo2HTtoiLica8vyYhJuoWAoLL471Pf4S7p66p762b141Ggf535QI1uvZPXxl/dnrmhQF4tuegR7799GD9ABpeK6W/z7V/j0Zc9HXY2DrAq3gwuvT7FpXrdMqaRwbs2bZiItbP/0oF+k4uHigZFIpyuYR+wvB6Ic2QpbrPzcsfQz7/T01z8yqB7q9Nwbq5X2Lq/55UgWSdln1Qv33RPqesrDm4R37SaA07rCIiIrpPy20ffmVHYVJzWK2C3gSL0evqGwW9CRalYm3jSoPH3ZEthwp6EyzGh6MbFfQmWJTr0ZY7kvaj1r9VQW+BZdlz0nK6XrAEdSp6FvQmWIypuryMCvm1Y0f9egX23A127kJRw4bTRERERERERERERRCb+hIRERERERERkUXQWLGpb35ixR8REREREREREVERxIo/IiIiIiIiIiKyCBzcI3+x4o+IiIiIiIiIiKgIYvBHRERERERERERUBLGpLxERERERERERWQQNm/rmK1b8ERERERERERERFUGs+CMiIiIiIiIiIougsWKNWn7i0SQiIiIiIiIiIiqCWPFHREREREREREQWQWPFPv7yEyv+iIiIiIiIiIiIiiAGf0REREREREREREUQm/oSEREREREREZFFsLJmU9/8xIo/IiIiIiIiIiKiIogVf0REREREREREZBE4uEf+YsUfERERERERERFREcTgj4iIiIiIiIiIqAhiU18iIiIiIiIiIrIIGivWqOUnHk0iIiIiIiIiIqIiiBV/RERERERERERkETi4R/5ixR8REREREREREVERxIo/IiIiIiIiIiKyCFbWrPjLTwz+iIgo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klGF38iRI1U/svKvjPYtAwBJ6Pd5jj5D8xODPyIiIiIiIiIiovswbNgwdTM3mIchGxsbNViI3B4V9vFHRERERERERERUBLHij4iIiIiIiIiILILGqvA09S0MWPFHRERERERERERUBLHij4iIiIiIiIiILILGYDAMenA8mkREREREREREREUQgz8iIiIiIiIiIqIiiE19iYiIiIiIiIjIInBwj/zFij8iIiIiIiIiIqIiiBV/RERERERERERkETi4R/7i0SQiIiIiIiIiIiqCWPFHREREREREREQWgX385S9W/BERERERERERERVBDP6IiIiIiIiIiIiKIDb1JSIiIiIiIiIii8CmvvmLFX9ERERERERERERFECv+iIiIiIiIiIjIMlixRi0/8WgSEREREREREREVQQz+iIiIiIiIiIiIiiA29SUiIiIiIiIiIoug0XBwj/zE4I+IiPJFr6tvFPQmWJR6E6oX9CZYjGZDQwt6EyyK8/4DBb0JFiWzS4OC3gSLsePr/QW9CRalpJ91QW8CWagrScULehMsStmC3gALYmerLehNsDAM0IjBHxERERERERERWQgNB/fIVzyaRERERERERERERRCDPyIiIiIiIiIioiKITX2JiIiIiIiIiMgiaKzYN2F+YsUfERERERERERFREcSKPyIiIiIiIiIisgwc3CNf8WgSEREREREREREVQaz4IyIiIiIiIiIii8A+/vIXK/6IiIiIiIiIiIiKIAZ/RERERERERERERRCb+hIRERERERERkUXQaFijlp94NImIiIiIiIiIiIogVvwREREREREREZFl4OAe+YoVf0REREREREREREUQgz8iIiIiIiIiIqIiiE19iYiIiIiIiIjIImisWKOWn3g0iYiIiIiIiIiIiiBW/BERERERERERkUXQcHCPfMWKPyIiIiIiIiIioiKIFX9ERERERERERGQZNKxRy088mhbs008/RWho6EN/ng0bNkCj0SA6OvqB1hMYGIixY8fCEr300kt4+umnC81rQsD06dPh4eFx1/nk3F20aNEj2abC5MKFC+rYHDhwoKA3hYiIiIiIiAoIK/5yuHnzJkaNGoXly5fjxo0b8PT0RI0aNdS0xo0bozDav38/vvjiC2zatAkxMTEoXbo0WrRogXfeeQcVKlTIt+fZvXs3nJ2dH2gdsl0bN268Y/rg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TTcTelw13v1bQW+CxZhyQdc3GOl4exTtQPZevMRCHyNL9+be3cfj5onarOfR+34R4w1DI54unNfR5BUFV0Xu0Kno9aPIKwTdQTr3l0ESmjdvrpr7/fzzz6rJpFSYUf6RyrLDhw+r/uYY+hERERERERFRfmPwRyabn0oFmzQrlIJQaSosfYPlNkgF3Ttptrtr1y7Vf5uMOExERERERET02DPTJRjdHwZ/dAfpMy7niKCPM+kX7W4t4qWfPrndaxNiIiIiIiIiIqKHhTEqERERERERERFREcSKPyIiIiIiIiIisgyawjkoiaVixR8REREREREREVERxIo/IiIiIiIiIiKyDBrWqOUnHk0iIiIiIiIiIqIiiBV/RERERERERERkGdjHX75ixR8REREREREREVERxOCPiIiIiIiIiIioCGJTXyIiIiIiIiIisgxWrFHLTzyaRERERERERERERRAr/oiIiIiIiIiIyCJoObhHvmLFHxERERERERERURHE4I+IiIiIiIiIiKgIYlNfIiIiIiIiIiKyDBrWqOUnHk0iIiIiIiIiIqIiiBV/RERERERERERkGVjxl694NImIiIiIiIiIiIogVvwREREREREREZFF0Go0Bb0JRQor/oiIiIiIiIiIiIogBn//Z+8+wJuq+jCAvy2lzJY9C5RN2XujgIAgS5ClICDDgRMnoijip+JWlrhBFGUv2UP2kL333lBmyyzQfM976k2TkJSWtjQt7+958mjSm+TecwfJm/85R0REREREREREJAVSV18REUkQW5dtTupV8CoZA6sm9Sp4jcjmNZJ6FbxK7TU/JPUqeJXlVZ9N6lXwGldGbUvqVfAq2TLrq4q4lyXd9aReBS+jc8WSLbO6iKYImtwjQak1RUREREREREREUiD9NCAiIiIiIiIiIt5Bk3skKFX8iYiIiIiIiIiIpEAK/kRERERERERERFIgdfUVERERERERERHv4KsatYSk1hQREREREREREUmBVPEnIiIiIiIiIiJewabJPRKUKv5ERERERERERERSIFX8iYiIiIiIiIiId/BRjVpCUmuKiIiIiIiIiIikQAr+REREREREREREUiB19RUREREREREREa9gU1ffBKXWFBERERERERERSYFU8SciIiIiIiIiIt7Bxyep1yBFUcWfiIiIiIiIiIhICqTgT0RERERERERE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iX8MxbRxPyFHzrx4vPsbqFG3aRJsodzL60SNxk+b8HDWH+/j2pUw5C9a2bymX+roH80favsWfFP54e9f38LNG9fMrL8dX/sN6TI4D8mxaflEFK/YCGnTR/37fb+wpdBJNpKKjy2uszRIkmKXRYYT7N7rKVBgkMCZVuPS3dbC0JEVaneaUVdEvAuHDGDYyvCV53FSqNNicZK8r7eq0TR6gqX7XdPP7n4c05So0pSoKkSJsryq+x/A7kfrR21L6lXwKvnzqEbB8lTMv5fed5ZtjxoqSaLUKZUwY0GnBCM9D1N/X0qu144LG/5JsvfOXPGhOD+H47pzfHz2LuQkj+zRFVNvSwuLLFhww6KqKVOieq0kBv1rKgYryzgWGcebU+gn4v1YnckKUv6DwvPX6p5vDR0gIiIiIiKSLCWjir+xY8eaXm/ff/+96eXJ3n/sVcihvTgkkyfsZcVedOxlldiST2tKomJYwC7F7DrIGYdFxPuxWzB/UeLYiaz4W7p0qel+LSIiIiIiIomPQzBxCLdu3bqZYaYYAHLoNQ7j5gknluzUqZOZEJQTNyY2VfwlMxy77E69szk2WVzHJ2MXYhFJPjhZyrp165J6NURERERERFKM69evm9udJjakiIgI852M46Q7zp3AwoyVK6NndnbF3lqsBuQQTSzeSGyq+BMREREREREREa9g8/FJstvAgQORKVMmpxsfc+fMmTOmei9XrlxOj/M+x/tzZ9myZWbiVddJRxOTKv5EREREREREROS+17dvXzNmnyN31X53Izw8HJ07dzah370coknBn4iIiIiIiIiIeAVbEk7ukcZDt153GN6lSpUKp06dcnqc93Pnzn3b8vv27TOTerRo0cL+WGRkpPmvn5+fmRCkSJEiSGjq6isiIiIiIiIiIhIH/v7+qFy5MhYsWOAU5PF+zZo1b1s+JCQEW7ZswcaNG+23li1bon79+ub/8+fPj8Sgij8REREREREREZE4Yrfgrl27okqVKqhWrRq+/fZbXL582czyS126dEFQUJAZJzBt2rQoU6aM0/MzZ85s/uv6eEJS8CciIiIiIiIiIt7BxwfJRYcOHRAaGor333/fTOhRoUIFzJ492z7hx+HDh81Mv0lJwZ+IiIiIiIiIiMhdePHFF83NnUWLFsX43JEjRyKxKfgTERERERERERHc75N7pERqTRERERERERERkRRIwZ+IiIiIiIiIiEgKpK6+IiIiIiIiIiLiFWxIPpN7JAeq+BMREREREREREUmBVPEnIiIiIiIiIiJeQZN7JCy1poiIiIiIiIiISAqkij8REREREREREfEOPhrjLyGp4k9ERERERERERCQFUvAnIiIiIiIiIiKSAqmrr4iIiIiIiIiIeAWbatQSlFpTREREREREREQkBVLFn4iIiIiIiIiIeAWbJvdIUAr+REQkQbwzoFZSr4JXORyaOqlXwWus+mxDUq+CV9lwUB0uHF0ZtS2pV8FrVOpSOqlXwascnbErqVdBvNSZy2mTehXES924mdRrIOJ99MlTREREREREREQkBVLFn4iIiIiIiIiIeAWbj2rUEpJaU0REREREREREJAVSxZ+IiIiIiIiIiHgFGzS5R0JSxZ+IiIiIiIiIiEgKpIo/ERERERERERHxChrjL2GpNUVERERERERERFIgBX8iIiIiIiIiIiIpkLr6ioiIiIiIiIiIV7D5aHKPhKSKPxERERERERERkRRIFX8iIiIiIiIiIuIVbFDFX0JSxZ+IiIiIiIiIiEgKpOBPREREREREREQkBVJXXxERERERERER8Qo2H9WoJSS1poiIiIiIiIiISAqkij8REREREREREfEKmtwjYaniT0REREREREREJAVSxZ+IiIiIiIiIiHgFjfGXsNSaIiIiIiIiIiIiKZCCPxERERERERERkRRIwV8KtGjRIvj4+ODChQvm/siRI5E5c+Y4vUbBggXx7bffxrgM32PKlCnm/w8ePGjub9y40e06SJQrV66gTZs2CAwMVPskwDH4wQcfoEKFCvdsnZKTp556Cq1atUrq1RAREREREYnz5B5JdUuJNMZfHL5E//bbb+b//fz8kDVrVpQrVw5PPPGE+Zuvr3OGumLFCnz00UdYuXIlrl69imLFiqFbt2545ZVXkCpVqli/T758+dCuXTt8+OGHSJs27V2te4cOHdC0aVMktBMnTiBLlixu/1arVi3z90yZMtnDx969e8c56GJQ9r///Q/jxo3DsWPHEBAQgFKlSuG1117Do48+iuSG+3bp0qXm+MiePbu9fRyxrXisuPrpp5/Qs2fPeL0/gzKGtVZA683WrFmDDBky2O8zKJ08eXKShFmxbTcuN2DAADRu3BizZ892+tsXX3yBt956C3Xr1jXBeGIbNGgQ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+0+3dfXdtXYiMgTmRr5i0WOmerMVO2xI7WczY//xeDkcasOfi245HS9ZMvr8d7xE7e+8WX3QpUH0D3sPV4r6/037IzHt36gnFg/ywaM1opdpUzvq/xdvicSSrYkzFuW9kqlyGdRc8Lv9fqkvoz5LHRk1CZt79EVyVfW/6+i8v6Kuo0G8jj7v5jrqcF6UqNwUVy6dw4oZg815kSOopHmO03X0YNR19NcPna+jPT6Iuo7u3jjHXIs57iBvlsCsQeg5IOYxeSXxla/xCC6HncPciUPMMCGszuv+1g/2rr4XXD5zFCxeEU88/znmjB+M2eO+Rfbcwejy6hDkdvjMQZtWzTQl4eVrNrvn2yQJq1qjqGvH3D//u3YUqYw2LzhfOy64XDtCeO0IP4fl06OvHW1fiL520MZlY7ByZtTEnTTmm07mv02eHIgyNR/DoR3LcSH0kLn98O6DTuv0xrBdibzVklL52GKahUISBL+Yc9IHdqVkl1THCRIkaiIUhn8M7hg6iEjcccxEdttnBWFSmbnei6Y49QKHQ2MeM+9+cu6CJltwlCaNuuw4unJVx4elUhfP44/ej47O0Jdcy7MPJ/UaeJcpa3TdcNSqavyHFUopfpqf1GvgXZ6OLlBMVvbuO5Bk7120yO3j1Sd3qvi7B9KmTWsqqlgZxQopazxAgekayio2dqHu1q1bUq+OSLLA6tfvv//eVMSy2/lff/1ln5RDREREREQkObNpOooEpeDvHoZ/ruOxCczYcOxuzHHrYjNmm4hEjTvCLuwcToAVxez2PXHiRDNeo4iIiIiIiIhFwZ8kKfU0F4k7TrrBCj8REREREZGUxgZN7pGQVD8pIiIiIiIiIiKSAin4ExERERERERERSYHU1VdERERERERERLyCuvomLFX8iYiIiIiIiIiIpECq+BMREREREREREa+gir+EpYo/ERERERERERGRFEgVfyIiIiIiIiIi4hVU8ZewVPEnIiIiIiIiIiKSAin4ExERERERERERSYHU1VdERERERERERLyCzaauvglJFX8iIiIiIiIiIiIpkCr+RERERERERETEK2hyj4Slij8REREREREREZEUSMGfiIiIiIiIiIhICqSuviIiIiIiIiIi4hXU1TdhqeJPREREREREREQkBVLFn4iIiIiIiIiIeAVV/CUsVfyJiIiIiIiIiIikQKr4ExER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VRo8bcLsBWOjzpW8hSuj9XPO58qFsy7nSqWm5jhfOXOwCe2y5yuJVs9FnyupUvvj+L612LjoNxPMsDI+qEgVM76f46Qg88b0w7G9q+33//wi6t+abu9HnU+S+Pjj5t7NUdemER87j3X+xKujzPjL7j6DcVKNJVO+RviFk0ibPjNKVHwYDz76qtPQB/w8xh/TFk781PyIlD5jZhPYFb3DD2WOn8E4ZiB/5OU1tNfHUevJf59nj37P/HuXNn0m08PjyTfH2INBEU98bLH99ppMcZB8BlqcLINd7hgyeQuGKqwqYggiIhIfDOsY1HOsRf6gkBR+TX7f6+QeiWNBuMh967p6AjrJ1yxqSA4Bmt3YldSr4FWGz07qNfAuvZznkbiv6fOos+4PIVlavO1Kkr133dJxH3Pe26X4j+Ksfpk6daqpoGE3PRGRlIBjnHLsUla0slKXXZDZHdmxulNERERERETub8mmq298w7+33347qVdDRCTBcGxAdoln13d2uWZXaI6d6DrDsYiIiIiIiNy/7ovgz1uNHDkyqVdBRJIpjnPJm4iIiIiISEpis939hIVyH3b1FRERERERERERuR+p4k9ERERERERERLxCyp6C9t5TxZ+IiIiIiIiIiEgKpIo/ERERERERERHxCpHQGH8JSRV/IiIiIiIiIiIiKZCCPxERERERERERkRRIXX1FRERERERERMQr2Gzq6puQVPEnIiIiIiIiIiKSAqniT0REREREREREvILNltRrkLKo4k9ERERERERERCQFUvAnIiIiIiIiIiKSAqmrr4iIiIiIiIiIeAUbNLlHQlLFn4iIiIiIiIiISAqkij8REREREREREfEKkZrcI0Gp4k9ERERERERERCQFUsWfiIiIiIiIiIh4BZtNY/wlJFX8iYiIiIiIiIiIpEAK/kRERERERERERFIgdfUVERERERERERGvYNPkHglKFX8iIiIiIiIiIiIpkI/NpixVRERERERERESS3vT1N5PsvZtXSnkdY1XxJyIiIiIiIiIikgIp+BMREREREREREUmBUl4No4iIiIiIiIiIJEsakC5hqeJPREREREREREQkBVLFn4iIiIiIiIiIeAWbzSepVyFFUcWfiIiIiIiIiIhICqSKPxERERERERER8QqRGuMvQaniT0REREREREREJAVS8CciIiIiIiIiIpICqauviIiIiIiIiIh4BZu6+iYoVfyJiIiIiIiIiIikQKr4ExERERERERERr2CDT1KvQoqiij8REREREREREZEUSMGfiIiIiIiIiIhICqSuviIiIiIiIiIi4hUiNblHglLFn4iIiIiIiIiISAqkij8REREREREREfEKNlX8JShV/ImIiIiIiIiIiKRAqvgTERERERERERGvoIq/hKWKPxERERERERERkRRIwZ+XKFiwIL799luPfz948CB8fHywcePGBHtPvt6UKVPgzUaOHInMmTN7zeskBLZ50aJFkSpVKvTu3TupV8drxXafJYfjOCkkxjVDREREREREUnjw99RTT5kvk7ylTp0auXLlQqNGjfDrr78iMjLytuVXrFiBpk2bIkuWLEibNi3Kli2Lr7/+Grdu3brje508eRKvvPKKCUn4XL5X7dq1MXz4cFy5cgX3k/z58+PEiRMoU6ZMor7PwoULzf7Kli0b0qdPj1KlSuH111/HsWPHkJxD1A4dOmD37t3wBs8++yzatm2LI0eO4H//+5/HbbDOM+uWL1++BHn/5BKUue6zDz74ABUqVEiy9Yltu1n7a9WqVU6PX79+3ZxX/NuiRYuQUq4ZIiIiIiIiCSnS5pNkt5Torir+mjRpYr5QsqJk1qxZqF+/vgnomjdvjps3b9qXmzx5MurWrWsCCwZKO3fuNMt99NFHePzxx2GLoeP2/v37UbFiRcydOxeffPIJNmzYgJUrV+Ktt97C9OnTMX/+fCS1Gzdu3LP3YnVY7ty54eeXeMMy/vDDD2jYsKF5n4kTJ2L79u34/vvvcfHiRXz11Vd3/boRERG3Pcbg111QnFjSpUuHnDlzIqldunQJp0+fRuPGjZE3b14EBAR4XPbDDz8055l14zngTRL7+PeWfXa3oduIESOcHuP1MGPGjPF+bXfnU1JdM0RERERERCQFBn9p0qQxXyiDgoJQqVIlvPPOO5g6daoJAdk9jy5fvoynn34aLVu2xI8//mgqdVjF1LNnT/z222+YMGECxo0b5/E9nn/+efOFde3atWjfvj1KliyJwoUL49FHH8WMGTPQokUL+7IXLlwwr5sjRw4EBgbioYcewqZNm5xej1WCRYoUgb+/P0qUKIHff//d6e8MJevUqWMqC1nlxmDRscLH6jY3duxYE2ZyudGjR+Ps2bN44oknTFuwQo4VjX/99ZfTa9erVw8vvviiuWXKlAnZs2fHe++9d1vwySrG7t27mzCoQIECpt1i6ra3bds2E7Zym/mcBx54APv27TN/W7NmjanE5HvxPbnO69ev99jeR48excsvv2xurN7kOnN/Pfjgg/j555/x/vvv25dlKFi6dGlzHHAZ11CQj7GSrUuXLmbdnnnmGXu3zWnTppn25XMPHz5sqqDeeOMN034ZMmRA9erVY6yG4vbxGGD1J0OUqlWrOoXAXO9Dhw7h1VdftVdeeeo2eqdjgs/ltrdu3drs22LFipn1j8n58+fNdrPClc955JFHsGfPHvM3bpcV9PEYvVPlF5fleWbdeHwzMO3RowcKFSpkgjGu96BBg257LvehtY/y5Mljjj1r3xC3ie9v3Y9te3AZntPcVx9//LHZ3k6dOpl14/qwjVwDLwsDe+4Dq9qXxzJf8+2337Yvw/P4ySefvG2f8f8HDBhgzmtrv1rXGjpz5kyM+2nx4sWoVq2avT34no4/UrirEuU1i1WGd2o3d7p27YoxY8bg6tWrTvuEj7vq06cPihcvbtad1zheGxxDVavSkcci9zuvPXG5ZlnXDB5rvL9gwQJUqVLFvF+tWrWwa9cu+3uxfflDDo89nruVK1c212AREREREZF7hVFJUt1SogQb449BRvny5TFp0iRzn5V6DMUY6rhiaMcvuq4BmYXP4/NfeOEFEzC4YwU61K5dO1NFxeBx3bp1Joxs0KABzp07Z6+0YaUhu6xu3brVdLXs1q2bqUIkBhGtWrUyX4T//fdfE7i9++67bt+XgQFfa8eOHaZq69q1a+bLMcNIvjZDrs6dO2P16tVOz2PYySCTjzOoYXdnfpF3xACNX8hZ2cXgs1evXk5fyh2x6y1DOQYZ//zzj9luhoZWmBEeHm5ChmXLlpkuhwxD2IWXj7szfvx4U0nEikp3rACG78MglhWbW7ZsMaEEgwrHEIa+/PJLczxwW/h3K9j87LPPzHYztGQ1FwMpVnIyJNm8ebPZl6wotcIydxVz3A6GF3xtLsvjiSEi8fhjhaljtZw7dzomLAybuL1cN74vQy7ruPLUFZ5BCYMnbhfDXT6PQY5jyMLwlOvGx+KCVZLcPu4vVmQykGXw7hiiM5zjucNjkfuI68Lu8lYgTAzn+P7W/di2B/c3wy++Lo837luuB889nhN8b4bN7jCY5vFnVS4yjOOyjuEnH2N4667bL9eNYaa1X/lYbPYTzxU+xpCYwRbX8ZdffjGVx7Hlqd084TWB4SD3M/H4XLJkibk2uGLIxvOH7chrw08//YRvvvnGaZm9e/ea1+LxzSAvLtcsV1yO1xoep7wmcT9a2G48vrh9PNd5veOQDiIiIiIiIpJM2eKoa9eutkcffdTt3zp06GArWbKk+f9PP/2UWant/Pnzbpdt2bKlfVlXq1atMs+dNGmS0+PZsmWzZciQwdzeeust89jSpUttgYGBtmvXrjktW6RIEdsPP/xg/r9WrVq2p59+2unv7dq1szVt2tT8/6xZs2x+fn62EydO2P8+b948sw6TJ0829w8cOGDuf/vtt3doIZutWbNmttdff91+v27dumZbIyMj7Y/16dPHafuDg4NtTz75pP0+l82ZM6dt+PDhTu+/YcMGc79v3762QoUK2SIiImyxcevWLVtAQIDt77//tj/muH29evUy7XgnHTt2tDVq1MjpsTfffNNWqlQpp21p1aqV0zIjRoww77dx40b7Y4cOHbKlSpXKduzYMadlGzRoYLbPel6mTJliXKfSpUvbhgwZ4vT+33zzzW3v7/g6dzomiOvbr18/+/1Lly6Zx3i8uLN7927z9+XLl9sfO3PmjC1dunS2cePGmfs8H7jMwoULY9wmboO/v7/9eOdt0KBBbpd94YUXbG3atLHfz5s3r+3dd9/1+NqO+z2u7dG7d2+nZVq0aGHr1q2bLbYqVapk++KLL8z/8xj5+OOPzXaGh4fbjh49at6D7ehun/Xv399Wvnx5t9sT03565513bCVKlHA6/4YNG2bLmDGjOS88HTN8L75nTO3mjrUcrxX169c3jw0YMMDWunXrWO1/tk/lypWdtjt16tS206dP2x+LyzXLumbwPXl//vz59ufMmDHDPHb16lVzn9eIkSNH3nEbRUREREREEsufyyKT7JYSJeisvvzO61iJZz3mCbsUxgWr5VjtwqofdhElVvCwCoyD5rPrp3U7cOCAvdsrK5E4KYgj3ufjxCosjsnF7pQWdgt0hxV5jlh5w26t7OKbNWtW895z5syxV6BZatSo4dQ2NWvWNFVtjpOclCtXzv7/XJbrw0pGd9gOrKDyVI1z6tQp09WalX7s6stue2wn1/WKad+546ktXbfFtZ2s/e24jawa43NY/em471j1Ze07V9wGVpGy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YuWxp/FMW7ZsaarrGLhx6AP+gGDNgh2T+FyzYnpNHk88H3kd5SzJ7J7s2p1XREREREREkg8fzvBxr96M41yx8onVN6wo8xTKeANWu9SpU8dUMrkGAHHFgINf6hnGiIh4+zVLREREREQkqfy+JOneu/ODSHESdHKPO2ElCqsCGYCxK6Y1HqA3YPc6TijBrnf84syKPM60qS/QIuKNdM0SERERERERrwr+rPCPXX29DScc6NOnj+mWzK557GLsbmISERFvoGuWiIiIiIikRPeuX+r94Z529RUREREREREREfFk1OKke+8unuebTLbuecWfiIiIiIiIiIiIO5EqT0v6WX1FRERERERERETud8OGDUPBggXN0HbVq1fH6tWrY1x+/PjxCAkJMcuXLVsWM2fOTNT1U/AnIiIiIiIiIiISR2PHjsVrr72G/v37Y/369ShfvjwaN26M06dPu11+xYoVeOKJJ9CjRw9s2LABrVq1MretW7cisWiMPxERERERERER8QojFibde3erH7flWeFXtWpVDB061NyPjIxE/vz58dJLL7md2LZDhw64fPkypk+fbn+sRo0aqFChAr7//nskBlX8iYiIiIiIiIjIfe/69esICwtzuvExdyIiIrBu3To0bNjQ/pivr6+5v3LlSrfP4eOOyxMrBD0tnxAU/ImIiIiIiIiIiFdgv9Skug0cOBCZMmVyuvExd86cOYNbt24hV65cTo/z/smTJ90+h4/HZfmEoFl9RURERERERETkvte3b18zZp+jNGnSIDlT8CciIiIiIiIiIve9NGnSxDroy549O1KlSoVTp045Pc77uXPndvscPh6X5ROCuvqKiIiIiIiIiIhXiLQl3S0u/P39UblyZSxYsMD+GCf34P2aNWu6fQ4fd1ye5s2b53H5hKCKPxERERERERERkThit+CuXbuiSpUqqFatGr799lsza2+3bt3M37t06YKgoCD7OIGvvPIK6tati6+++grNmjXDmDFjsHbtWvz4449ILAr+RERERERERETEK3CSjeSiQ4cOCA0Nxfvvv28m6KhQoQJmz55tn8Dj8OHDZqZfS61atfDnn3+iX79+eOedd1CsWDFMmTIFZcqUSbR19LHZklOTioiIiIiIiIhISvXT/KR776cbIsVRxZ+IiIiIiIiIiHiFyMikXoOURZN7iIiIiIiIiIiIpEAK/kRERERERERERFIgdfUVERERERERERGvoJkoEpYq/kRERERERERERFIgVfyJiIiIiIiIiIhXUMVfwlLFn4iIiIiIiIiISAqk4E9ERERERERERCQFUldfERFJEGt3nU/qVfAqWVKrPSxHr+ZO6lXwKmHX/JN6FbxKlnTXk3oVvMaZy2mTehW8yomzqZJ6FbxGryZJvQbeZUbqEkm9Cl6l2Y1dSb0KXuPPZeoj6qhjHR8kR5HajQlKFX8iIiIiIiIiIiIpkCr+RERERERERETEK9iSdHYPH6Q0qvgTERERERERERFJgVTxJyIiIiIiIiIiXiFJC/5SIFX8iYiIiIiIiIiIpEAK/kRERERERERERFIgdfUVERERERERERGvEBmZ1GuQsqjiT0REREREREREJAVSxZ+IiIiIiIiIiHgFTe6RsFTxJyIiIiIiIiIikgIp+BMREREREREREUmB1NVXRERERERERES8QqS6+iYoVfyJiIiIiIiIiIikQKr4ExERERERERERr6DJPRKWKv5ERERERERERERSIFX8iYiIiIiIiIiIV7Al6SB/PkhpVPEnIiIiIiIiIiKSAin4ExERERERERERSYHU1VdERERERERERLxCkvb0TYFU8SciIiIiIiIiIpIC3VfB3wcffIAKFSoky/dZtGgRfHx8cOHChQR5vYMHD5rX27hxI7xZQrXlvdr3sfHjjz8if/788PX1xbfffpvUq+O1YrPPkstxnBQS+pohIiIiIiJyL9hsSXfD/d7V96mnnsJvv/0W9UQ/P2TNmhXlypXDE088Yf7GIMPRihUr8NFHH2HlypW4evUqihUrhm7duuGVV15BqlSp3L4Hv6jGpH///iYQuN/UqlULJ06cQKZMmRL1fSZOnIghQ4Zgw4YNuHXrFgoXLoy2bdvixRdfNPs7OeAxNHnyZLRq1cr+2BtvvIGXXnoJSS0sLMy05ddff402bdp43J/uzoPatWtj2bJl8Xp/BmWFChUy+9dbglBPXPcZrzEMsaZMmXLP1yW27WYtx2vh4cOHERQUZP8bz18GvjyvDhw4gIIFC6aIa0ZSmDtjAmZM/gMXz59DgUJF0fWZ11GkeGm3y/4zZwqWLZyFI4f2m/uFipZAh869PC7v7f7++29MnDAB58+fR6HChdGrVy+UKFHC7bKzZ83CggULcOjQIXO/aNGi6PrU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iIiIiIjICzHwR0RERERERERE5IVY6ktERERERERERB6Bsz3eL2b8EREREREREREReSFm/BERERERERERkUfw43CP94oZf0RERERERERERB/InTt3pF69ehIlShSJFi2aNG3aVB4+fBjk57dq1UrSpk0r4cOHlyRJkkjr1q3l3r17b/29mfFHREREREREREQewdcLm/zVq1dPrl69KitXrpQXL15I48aNpUWLFjJt2jSXn3/lyhW9DRw4UDJkyCDnz5+Xr776SrfNnj37rb73J35+XriiREREREREREQU7LQaet9t33vEd1He+7959OhRDd7t3LlTcuXKpduWLVsm5cuXl0uXLkmCBAne6N+ZNWuWfPHFF/Lo0SMJFerN8/hY6ktERERERERERMZ79uyZ3L9/3+GGbf/F1q1btbzXCvpByZIlJUSIELJ9+/Y3/ndQ5otS4bcJ+gEDf0RERERERERE5DHDPdx169u3r0SNGtXhhm3/xbVr1yROnDgO2xC8ixEjhj72Jm7duiU///yzlge/LQb+iIiIiIiIiIjIeD/88INm1tnfsM2Vzp07yyeffBLk7dixY/95n5B1WKFCBS0X7tGjx1t/PYd7EBERERERERGRR0DmnbuEDRtWb2+iffv20qhRoyA/J0WKFBIvXjy5ceOGw/aXL1/q5F48FpQHDx5I2bJlJXLkyDJv3jwJHTq0vC0G/oiIiIiIiIiIiN5C7Nix9fY6+fPnFx8fH9m9e7fkzJlTt61Zs0Z8fX0lb968QWb6lSlTRgORCxculHDhwsm7YKkvERERERERERHRB5A+fXrN2mvevLns2LFDNm/eLN9++63Url3bNtH38uXLki5dOn3cCvqVLl1aJ/iOGzdOP0Y/QNz++eeft/r+DPzRR4c69/nz5+v9c+fO6cf79u37oN8T6bdVqlQRT4Ca/Lhx4zqsA73bz2zdunW6jnj3hBxNnDhRJ0cREREREREFJ6j0ddftQ5k6daoG9kqUKCHly5eXTz/9VP744w/b4y9evJDjx4/L48eP9eM9e/boxN+DBw9KqlSpJH78+LbbxYsX3+p7M/D3HwMTVsNG1FkjmFOqVCkZP368pmw627Jli/6Ao0ePrimamTNnlsGDB782Wvu23+dDBgPmzJkjRYsW1ck2kSJFkixZskivXr20Nt0TBBZIHDZsmD53dzt69Kj0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iMgj+HG4x3vFjD8iIiIiIiIiIiIvxMAfERERERERERGRF2KpLxEREREREREReQRfDvd4r5jxR0RERERERERE5IWY8UdERERERERERB7Bjxl/7xUz/oiIiIiIiIiIiLwQM/6IiIiIiIiIiMgj+Pkx4+99YsYfERERERERERGRF2Lgj4iIiIiIiIiIyAux1JeIiIiIiIiIiDyCn6+vu3fBqzDjj4iIiIiIiIiIyAsx44+IiIiIiIiIiDyCry+He7xPzPgjIiIiIiIiIiLyQsz4IyKi92L8GnfvAXmqMKH5rq2967fdvQeeJWa0T9y9Cx7jxUt374FnCckUBZsmxd29B55l2ib+XrFX91OeRy1LQqd19y54lAovjrt7F8gDMPBHREREREREREQewc+Pwf33ie+jEREREREREREReSFm/BERERERERERkUfw43CP94oZf0RERERERERERF6IGX9EREREREREROQRmPH3fjHjj4iIiIiIiIiIyAsx8EdEREREREREROSFWOpLREREREREREQewdfP19274FWY8UdEREREREREROSFmPFHREREREREREQegcM93i9m/BEREREREREREXkhBv6IiIiIiIiIiIi8EEt9iYiIiIiIiIjII7DU9/1ixh8REREREREREZEXYsYfERERERERERF5BD8/Zvy9T8z4IyIiIiIiIiIi8kIM/BEREREREREREXkhlvoSEREREREREZFH8PX1dfcueBVm/BEREREREREREXkhZvwREREREREREZFH8PPlcI/3iRl/REREREREREREXogZf0REH9HNmzelW7dusmTJErl+/bpEjx5dsmbNqtsKFiwoJtm2/A9ZP3+Q5CzWQErW/NHl5xzfu0K2LRstd29eEN9/Xkr0OEkld8nGkilvlf/0vR/euyFrZveTaxcOyd2b5yVn0fou9+Hp4/uyYcEQObFvpTx97CNRYiSUEjW6SMpMReR9wXPct3G6XLtwWJ4+8pFGXeZL3MTpX/t1H2LfXr54Jsunddd9uX3ttKTKXFSqffU/h89ZMqmzHNo2L8DXxoyfSpp1WyIfys41U2Xr8nHy8N4tiZs4nZSt85MkTJEl0M8/smuZrJs/THxuXZYYcZNKierfS+os/mvzz8sXsnb+MDl1cL343LwkYcNHkuQZCkiJ6u0kcrS4+jnnjm2XPwc2dPlv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Sbx/WwtQ8BY1ZybJv/pP28cZBnbR/1+cPFcONA26MoboQ/rEz7lZFBER0TsY7//3LlEAYULzTw171x3bRBkvZjTHsjeTvfBvu0n/CsmmRDZN3NNi1GNN28TfK/bqfsrzqGVJ6LTu3gWPUuHFh3vj5UMqXX+v2773ij/frs1FcMBfp0RERERERERERF6Ipb5EREREREREROQR7AfY0X/HjD8iIiIiIiIiIiIvxMAfERERERERERGRF2KpLxEREREREREReQQ/Xw7weZ+Y8UdEREREREREROSFmPFHREREREREREQewc+Pwz3eJ2b8EREREREREREReSEG/oiIiIiIiIiIiLwQA39EREREREREROQRfH393Hb7UO7cuSP16tWTKFGiSLRo0aRp06by8OHDN/paPz8/KVeunHzyyScyf/78t/7eDPwRERERERERERF9IAj6HT58WFauXCmLFy+WDRs2SIsWLd7oa4cOHapBv3fF4R5EREREREREROQR/Hy9a7jH0aNHZdmyZbJz507JlSuXbhsxYoSUL19eBg4cKAkSJAj0a/ft2yeDBg2SXbt2Sfz48d/p+zPjj4iIiIiIiIiI6APYunWrlvdaQT8oWbKkhAgRQrZv3x7o1z1+/Fjq1q0ro0aNknjx4r3z92fGHxEREREREREReQS/D9hr73WePXumN3thw4bV27u6du2axIkTx2FbqFChJEaMGPpYYNq2bSsFChSQypUry3/BjD8iIiIiIiIiIjJe3759JWrUqA43bHOlc+fO2nsvqNuxY8feaT8WLlwoa9as0f5+/xUz/oiIiIiIiIiIyHg//PCDtGvXzmFbYNl+7du3l0aNGgX576VIkULLdG/cuOGw/eXLlzrpN7ASXgT9Tp8+rSXC9qpXry6FChWSdevWveEzYuCPiIiIiIiIiIg8hJ+f+4Z7hH2Lst7YsWPr7XXy588vPj4+snv3bsmZM6ctsOfr6yt58+YNNJuwWbNmDtsyZ84sQ4YMkc8++0zeBgN/REREREREREREH0D69OmlbNmy0rx5cxk9erS8ePFCvv32W6ldu7Ztou/ly5elRIkSMnnyZMmTJ49mArrKBkySJIkkT578rb4/A39ERERERERERCSmD/f4UKZOnarBPgT3MM0XJbvDhw+3PY5g4PHjx3WS7/vGwB8REREREREREdEHggm+06ZNC/TxZMmSiZ9f0AHP1z0eGE71JSIiIiIiIiIi8kLM+CMiIiIiIiIiIo/g5+u+4R7eiBl/REREREREREREXugTv3ctEiYiIvIwz549k759+8oPP/wgYcOGFZNxLRxxPRxxPV7hWjjiejjierzCtXDE9XDE9XiFa0GehoE/IiLyGvfv35eoUaPKvXv3JEqUKGIyroUjrocjrscrXAtHXA9HXI9XuBaOuB6OuB6vcC3I07DUl4iIiIiIiIiIyAsx8EdEREREREREROSFGPgjIiIiIiIiIiLyQgz8ERGR10AD5e7du7ORMtciAK6HI67HK1wLR1wPR1yPV7gWjrgejrger3AtyNNwuAcREREREREREZEXYsYfERERERERERGRF2Lgj4iIiIiIiIiIyAsx8EdEREREREREROSFGPgjIiIiIiIiIiLyQgz8ERERkdfZs2ePHDx40PbxggULpEqVKtKlSxd5/vy5W/eNyJP9888/sm/fPrl79667d4XcjOdRRxcvXpRLly7ZPt6xY4d899138scff4iJnjx5Io8fP7Z9fP78eRk6dKisWLHCrftFRAEx8EdERERe58svv5QTJ07o/TNnzkjt2rUlQoQIMmvWLOnYsaOYZtKkSbJkyRLbx1iDaNGiSYECBfRizSRcC0cIXIwbN84W9CtSpIjkyJFDEidOLOvWrRPTLFu2TDZt2mT7eNSoUZItWzapW7euccFQnkcd4RhYu3at3r927ZqUKlVKg38//vij9OrVS0xTuXJlmTx5st738fGRvHnzyqBBg3T7b7/95u7dIyI7DPwREVGwt3HjRvniiy8kf/78cvnyZd32559/Oly8mSJFihRy+/btANvxRzkeMwUuVnGxDrhILVy4sEybNk0mTpwoc+bMEdP06dNHwocPr/e3bt2qwYz+/ftLrFixpG3btmISroWj2bNnS9asWfX+okWL5OzZs3Ls2DFdCwQ0TNOhQwe5f/++3ke2W/v27aV8+fK6Lu3atROT8Dzq6NChQ5InTx69P3PmTMmUKZNs2bJFpk6dqmtiYkZooUKFbOeRuHHj6psnCAYOHz5cTIS/PQsWLCgJEiSwvZGELEhkyxK5EwN/REQUrOHio0yZMnohv3fvXnn27Jluv3fvnl7gm+bcuXOateMM62IFRU3g5+cnvr6+en/VqlV64Q7IYrp165aYWKKWKlUq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IbiCP4V9sWpHbUfXsS5dunhlrCpkFyxYYFdeeWWyTxkIHsEfAACInKFDh3rL3jPPPOMLG2KLPrp168a2xUCpXVM3ok2bNk07Nm7cOJ/b9ssvv1jz5s3tqaeeSlt2gTDddtttvsBBrdCx18Kvv/5qDz/8sD8XqliTmCr9QqaAL/SZh0888YTNnj3bZsyYke79VHRMVX/ahD127Fhr37590s4TwP/Q6gsAACLn+OOP93ZeDerPnv2PzzljjzNuLd2xY0eSzhJ/JbVu1qlTx+699960Fr1q1apZx44drXz58h4W33TTTT7LDeFSddKcOXM89KtSpYofW758uf32229Wt27d4DYev/jii/b444/b+vXr/fvSpUvbnXfe6bNSQ6RtvcOHD0/bFn/WWWf5rEMFXaFQm7NeA9dff32WrxlV/TVo0MDeeOONICplgVRHxR8AAIgc3ZgB8ZYtW+aVXDGa43b++efb888/n9Yeruo/gr+waQv4VVddle6YXhsh6tevnz322GNePR2/6KR79+729ddf24ABAywk7777rs/404KgWrVq+TFtjh85cqS9+eabVr9+fQuBQuB69epl+XzsOUI/IHVQ8QcAAIDI0/IO3bDGQpwLL7zQqwD79Onj32/cuNE3l/70008WEgb0IytaeqMtv5rnFk+vF4WB27Zts5BoWZR+L7TFN16vXr1s1qxZtmTJEgtBoUKF7J///GfagpOMVE190UUX2c6dO//ycwOQWLYsjgMAABzVtMjj1Vdf9Sovfb322mve7oswFSlSJG1xgdo2dZOuLZwxCvxy5MhhodCA/jZt2vjXmjVrrFSpUlayZEkf0N+kSRPr2rWr/5zmIr7++uvJPl0kgRYkxWakxjvnnHOCfC9Ve2/nzp0zHVfLq36HQqHqTy3vyIpm68YqRAGkBlp9AQBA5Kxevdpbsr7//nsrW7asHxs8eLBXsKglq2LFisk+RfzFFGapMkevg+nTp1vevHmtdu3aac+vWLEiqDldDOhPTEGnWlznzZtnP/zwgwekoc4E1YZaBTxq9403atQoa9u2rYVG/35oZIDmHMbTsZNOOslCoSppzUvV78o999zjW33VRKhg9NFHH/UWX/3+AEgdtPoCAIDIUbWBbtJeeuklX/QhajvSIocff/zRFi1alOxTxF9MbYktWrSwhQsXWv78+f21oUUOMVrc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"/>
</div>
</div>
</div>
</div>
</div>
</main>
</body>
</html>


