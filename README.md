# I founds a boooog

## Statement of bug

When creating a nested markdown file using GitHub's in-browser editor,
the editor preview resolves relative paths from the project root whereas
they /should/ be relative to the nested directory.

## Steps to reproduce

1. Create `dir/DOC.md` in browser editor
2. Add image tag with source 'image.png'
3. Preview in browser editor (looks good)
4. Save
5. View file (looks bad)

## Suggested behavior

Paths in editor preview should be expressed relative to nested directory.
