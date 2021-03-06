
.. _app_code:

Code / Markdown
===============

The Code/Markdown application in CryptPad is an integration of
`CodeMirror <https://codemirror.net/>`__.

.. image:: /images/app-code-preview.png
   :class: screenshot

Toolbar
-------

|wrench| **Tools**: Show/hide the text editor toolbar.

|picture-o| **Insert**: Add an image to the document. The image can be
chosen in the CrpytDrive or uploaded. :badge_user:`Logged in users`

|cptools palette| **Theme**: Set colors for the editor, detailed
:ref:`below <app_code_theme>`.

|eye| **Preview**: Show/hide the Markdown preview pane.

.. _app_code_theme:

Theme
-----

|paint-brush| **Color by author**: Highlight the text written by each
user with their cursor color (picked in :ref:`user settings <user_settings_cursor>`). When active:

- |paint-brush| **Hide author colors** to turn off the display of colors in this window, the colors can be turned back on and remain active for other users.

- |paint-brush| **Color by author** > **Clear and disable** to turn off the colors for all users and delete the data.

**Theme**: Color scheme used in the code editor pane.

**Language**: Used for syntax highlighting.

Import/Export
-------------

| |file-o| **File** > |upload| **Import**.
| Suported formats: Any plain text file, the file extension is used to determine the language.

| |file-o| **File** > |download| **Export**.
| Supported formats: ``.md``, any other extension can be typed for the name of the exported file.

Markdown
--------

The Code application is particularly suited for writing documents in
Markdown: a lightweight syntax that offers basic formatting while
remaining readable. Markdown is readily converted to other formats such
as HTML.

`Markdown syntax
guide. <https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet>`__

.. localised link to markdown tutorial if possible. French here:
   https://blog.wax-o.com/2014/04/tutoriel-un-guide-pour-bien-commencer-avec-markdown/

Additionally to basic Markdown syntax, the following features are also
available:

-  ``[TOC]`` Inserts a table of contents.
-  Todo list

   -  ``- [ ] task`` for a task to do: |square-o| task.

   -  ``- [x] task`` for a completed task: |check-square| task.

-  Diagrams with `Mermaid <https://mermaid-js.github.io/mermaid/#/>`__.
-  Mindmaps with `Markmap <https://markmap.js.org/>`__.
-  Mathematical equations with `Mathjax <https://www.mathjax.org/>`__.

Images
------

It is strongly advised **not** to insert external images in documents.
The Markdown syntax ``![description](https://site.com/image.jpg)`` is
supported but presents security risks. Malicious code can be hidden in
images and result in data leakage.

For this reason, CryptPad makes use of ``media-tag`` to insert images
from the CryptDrive. This syntax is more complex but it is managed
automatically by the |picture-o| **Insert** menu.

Lightbox
--------

To browse through all images and diagrams in a document using the full
width of the window:

1. ``Double click`` on an image or diagram in the Markdown preview.
2. Navigate with the arrow keys.
3. Close the light box with |times| or ``Esc``.