# Preferences
The preferences dialog  can be accessed with the menu item "*Edit*" -> "*Preferences*". The following options can be configured:

Interface
---------
**Add 'tearoff' strips to the menu** adds a 'tearoff' strip to all menus in the menubar. This means that menus can be opened as small windows and stay open while editing a page.

**Use <Ctrl><Space> to switch to the side pane** toggles the key binding for <Ctrl><Space>. Reason to toggle this binding off is usually that this binding is also used for input methods for non-western scripts.

**Remove links when deleting pages** toggles whether links to a page are removed when the page is deleted (the text of the link will remain, but it will no longer be a link). This is a preference because deletion does not use a dialog since we have support for the system trash.

**Always use last cursor position when opening a page** toggles whether pages are always opened on their last cursor position or not. When this is disabled pages only open with a cursor position when they are opened be a history reference (e.g. the "Back" button or a link from the pathbar).

**Use <Enter> to follow links** toggles the key binding to follow links inside a page. If disabled an <Enter> on a link will just be ignored. The <Alt><Enter> key binding can be used as an alternative.

**Show cursor also for pages that can not be edited** is used to toggle behavior of the cursor when a page can not be edited. By default the cursor is not visible when a page is read-only, but keyboard navigation is easier when the cursor is always visible.

**Use custom font** allows selecting a custom font for the editor window. This only applies to the page view itself, the font for all other interface elements is determined by the desktop theme.

Editing
-------
**Automatically turn "CamelCase" words into links** is used to enable or disable [auto-linking](./Auto_Formatting.markdown) CamelCase words.

**Automatically turn file paths into links** is used to enable or disable [auto-linking](./Auto_Formatting.markdown) for file paths.

**Automatically select the current word when you apply formatting **is used to enable or disable the feature where pressing e.g. <Ctrl><B> to toggle Bold formatting will automatically select the current word when the cursor is inside a word. The same option also controls whether toggling the format for a heading will select the whole line automatically.

**Unindent on <BackSpace>** toggles the key binding for the <BackSpace> key. If enabled the <BackSpace> key at the start of a indented line will unindent the line, if disabled the will delete the line break instead. The <Shift><Tab> key binding can be used as an alternative.

**Repeated clicking a checkbox cycles through the checkbox states** enables cycling the checkbox state. When turned off clicking a checkbox only toggles the checkbox between it's "checked" and "unchecked" states.

**(Un-)indenting a list item also changes any sub-items** toggles the behavior to make sub-items follow indenting of their parent list item

**Checking a checkbox also changes any sub-items** toggles the behavior to make toggling checkboxes recursive. This feature makes sense for example for todo-lists but not necessarily for other kinds of lists.

If the Reformat wiki markup on the fly option is enabled, zim tries to turn wiki syntax into formatting while you type. For example, typing "``**text**``" will turn into bold formatting when you type a <space> or <enter> after the last "*".

**Default format for copying text to the clipboard** allows you to set the preferred format when you copy some text from zim and paste it in an other application. Default is just plain text, but you can also choose to paste wiki formatted text. This option will only affect copy-pasting where the receiving application asks for text input (like a text editor), if it asks for example for HTML input zim will paste HTML formatted text automatically.
 
**Folder with templates for attachment files** is the folder to look for file templates, see [Attachments](./Attachments.markdown) for details.

Plugins
-------
This tab allows you to enable or disable the various [Plugins](../Plugins.markdown). Selecting a plugin will show a short description, select "More" to open the relevant manual page in this manual for a specific plugin or select "Configure" to set plugin specific preferences.

Applications
------------
**Set default text editor** allows to change the binding for the text editor that is used e.g. by the "Edit Source" menu option.

