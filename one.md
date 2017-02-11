The idea is to bring in people to write collaboratively
-------------------------------------------------------

<div>

How about writing in markdown and then using my pandoc and git to create
an html file and then uploading that html file to Authorea.

</div>

<div>

So, this workflow means:

</div>

1.  Start writing in markdown
2.  Add citation from bibtex file directly in the Atom editor
3.  Use pandoc to convert this section to html
4.  upload through git bridge to Authorea
5.  Add the html file to the layout.md
6.  Update

<div>

It should show up where we want to show up. Will it?

</div>

<div>

The dicey thing is the citation bit. Let's see. If I want to add a
citation by Carolina Menezes \\cite{menezes2013improvement} . To do
this, I need to set the correct file for Pandoc to work and write:

</div>

<div>

</div>

<div>

`pandoc -f markdown -t html --filter pandoc-citeproc --bibliography bibliography/biblio.bib -o one.html`
Another citation, by Barrett \\cite{barrett2012meditation}. Work?? Then
modify the layout.md file to include one.html and upload everything.

</div>

<div>

Will it work?

</div>

<div>

<div>

<div>

</div>

</div>

</div>

<div>

</div>
