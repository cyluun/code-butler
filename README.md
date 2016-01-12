![alfe](https://cloud.githubusercontent.com/assets/13040597/12249698/0a2f7d84-b8ca-11e5-8b40-4b6b63ccb086.png)

**A tool that parses TODOs from your source code effectively.**

**Currently in beta.**

Alfe is a CLI productivity tool that saves you time by finding all the to-do's in your code. It tries its best not to bother with files which may not be yours by filtering out gitignore material when searching inside git repositories. The search is very flexible as you can specify either a file or a directory with a relative or absolute path. There are options for searching only one specific file extension or excluding one.

![alfe-snap](https://cloud.githubusercontent.com/assets/13040597/11715950/e3632f46-9f4e-11e5-9027-390a8427f3a3.png)

**With Alfe you can**
* search separate files or entire directories with ease
* specify language extension to search
* specify language extension to exclude from search
* search inside git repositories excluding gitignore material
* search by either relative or absolute path

## Supported file extensions

.cpp|.cs|.c|.h|.css|.cjsx|.coffee|.ejs|
.erl|.go|.html|.htm|.hbs|.handlebars|
.hs|.hng|.hogan|.jade|.js|.es|.es6|.jsx|
.less|.mustache|.php|.pl|.pm|.py|.rb|
.sass|.scss|.sh|.zsh|.bash|.styl|.twig|.ts


#### Installation

Currently you'll need to clone, cd, and pip3 install .

## Usage

#### How to use the CLI:

alfe | option | directory/file


Options are:
* **-o --only** searches only files of this extension
* **-x --exclude** searches all other files except this extension

#### Examples

To search all files in a directory:
```bash
alfe Projects/web-app/
```

To search only Python files in current directory:
```bash
alfe -o .py .
```

To search a single file:
```bash
alfe contact.html
```

##License

MIT
