## The idea is to bring in people to write collaboratively

How about writing in markdown and then using my pandoc and git to create an html file and then uploading that html file to Authorea.

So, this workflow means:

1. Start writing in markdown
2. Add citation from bibtex file directly in the Atom editor
3. Use pandoc to convert this section to html
4. upload through git bridge to Authorea
5. Add the html file to the layout.md
6. Update

It should show up where we want to show up. Will it?

The dicey thing is the citation bit. Let's see. If I want to add a citation by Carolina Menezes [@menezes2013improvement] (by the way I need to set the correct file for Pandoc to work) and write:

```pandoc -f markdown -t html --filter pandoc-citeproc --bibliography bibliography/biblio.bib -o one.html
```
Then modify the layout.md file to include one.html and upload everything.

Will it work?
