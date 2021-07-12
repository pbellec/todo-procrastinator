This is the source code of the [todo-procratinator

This is the source code of the [to-do list for procrastinators](https://pbellec.github.io/todo-procrastinator).
Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by], except for images, see below.
 * file `images/shutterstock_1427368160.eps` and `todo-procrastinator/logo.png` was purchased with a limited license (unlimited web distribution) by P. Bellec from [shutterstock ID 1427368160](https://shutterstock.com/image-vector/procrastinating-woman-sitting-office-her-legs-1427368160)
 * file `todo-procrastinator/celeste.jpg` is a Fan-art by [GomiGomiPomi](https://gomigomipomi.tumblr.com) reproduced with permission from the author (_Usage of my drawings is allowed as long as proper credits are given and it's not for commercial purposes_).

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

This website presents a to-do list system for procrastinators.

## Usage

### Building the book

If you'd like to develop on and build the to-do list for procrastinators, you should:

- Clone this repository and run
- Run `pip install -r requirements.txt` (it is recommended you do this within a virtual environment)
- Run `jb build how_todo-procrastinators/`

A fully-rendered HTML version of the book will be built in `todo-procrastinators/_build/html/`.

### Hosting the book

The html version of the book is hosted on the `gh-pages` branch of this repo. Navigate to your local build and run,
- `ghp-import -n -p -f todo-procrastinators/_build/html`

This will automatically push your build to the `gh-pages` branch. More information on this hosting process can be found [here](https://jupyterbook.org/publish/gh-pages.html#manually-host-your-book-with-github-pages).

## Contributors

This text was put together by P. Bellec.

## Credits

This project is created using the excellent open source [Jupyter Book project](https://jupyterbook.org/) and the [executablebooks/cookiecutter-jupyter-book template](https://github.com/executablebooks/cookiecutter-jupyter-book).
