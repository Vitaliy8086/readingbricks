# Snip & Ship

## What is it?

It is a structured collection of tagged notes about machine learning theory and practice (now, in Russian only). Each note is independent of the others, but some of them require familiarity with core concepts and definitions.

Two key parts of the repository are as follows:
* The notes itself, all of them are written specially for this project;
* Search system.

Currently, there are a small number of notes and so there is no need in complicated search system. However, an outline of its evolution is created. Planned features of the search system are as follows:
- [x] Search by tags
- [ ] Logical operators
- [ ] Support of tags hierarchy
- [ ] Full-text search
- [ ] Ranking based on flexible parameters

## How to use it?

As always, this repository can be cloned to your local machine. Just run `git clone https://github.com/Nikolay-Lysenko/snip_and_ship` from your terminal.

When repository is cloned, look through the file named `list_of_tags.txt` and choose the tags you are interested in. Suppose that they are 'tag1', 'tag2', and 'tag3'. To make a notebook with notes that are associated with at least one of these tags, run:

```
python search.py -t tag1 tag2 tag3
```

Go to `notes` directory and look at the freshly created file named `notes_for_the_last_query.ipynb`. Enjoy reading!

## How to contribute?

Everyone can create a pull request.

Note that it is strongly recommended to update list of tags automatically. This is easy — just copy and rename files from `hooks` directory according to instructions that are placed inside of them right below shebang. If it is done correctly, Git hooks will refresh list of tags for you.


