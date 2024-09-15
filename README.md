# Pawprint Members and Tool Wiki

The contents in the `docs` directory automagically gets published to https://wiki.pawprint.space thanks to
[Material-mkdocs](https://squidfunk.github.io/mkdocs-material/).

## Editing Locally - Quick start

Prerequisites:
* git
* Python 3

TL;DR:
```bash
git clone https://github.com/PawprintPrototyping/pawprintprototyping.github.io.git wiki && cd wiki
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
mkdocs serve
```
Then visit http://localhost:8000 in your browser, open the `docs/` directory in your favourite editor,
and let the markdown flow.

## I have no idea what any of that means!

The longer version, for mere mortals:  The content for the Pawprint Wiki is stored and edited here in Github,
written using a formatting language called [Markdown](https://www.markdownguide.org/).  Using Markdown is different than a WYSIWYG editor, where you
see your changes immediately.  When you create a Markdown file (like this one!), you add characters that apply
various formatting - Markdown is meant to be easy to write, look decent when you're looking at the unrendered source
text, and compiles into HTML to be shown with a web browser.

It's easy to contribute to the wiki with just a Github account - click down into the docs folder, click on 
an existing article, and then click the "Edit" pencil icon in the top right - you can edit that right in your browser.
When you're done, click "Commit Changes", enter a message describing your changes, and if you're brave go ahead and commit
directly to the main branch.  After a few seconds, you should see your change show up on wiki.pawprint.space.  If you are
less brave and want someone to check over your work, use the "Create a new branch and start a pull request" radio button.
This will stage your changes for another member to review, before getting published.

If you'd like to edit multiple pages at once, upload files, or move pages around, you can open a more advanced IDE by pressing
the period/full-stop '.'
