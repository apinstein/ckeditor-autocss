The "autocss" plugin makes ckeditor a truly WYSIWYG even in complex css environments.

It does this by doing two things:

1.  Copies all css from the host page into the editor via editor.config.contentsCSS.
1.  Samples the background-color in effect at the parent of the host <textarea> control and applies that color to the editor so that you get appropriate background color for even better WYSIWYG.

This plugin has jQuery included inline; if your site already uses jQuery, you could save room by removing it. Or someone could optimize out the parts that we need (just a selector for all included css and a cross-browser getComputedStyle).
