# I founds a boooog

## Statement of bug

When creating a nested markdown file using GitHub's in-browser editor,
the editor preview resolves relative paths from the project root whereas
they /should/ be relative to the nested directory.

## Steps to reproduce

1. **Create** `dir/DOC2.md` in browser editor
2. Add image tag with source 'image.png'
3. Preview in browser editor (incorrect, see trollface)
4. Save
5. View file in source browser (looks good, see kitteh)
6. Click edit, preview in browser editor (looks good, see kitteh) 

> **NOTE:** editing an existing file resolves relative paths correctly.  This bug is only expressed during file creation.

## Desierd behavior

Resolve relative paths consistently in create+editor, edit+editor, and source browser.  That is, resolve relative to current directory.
