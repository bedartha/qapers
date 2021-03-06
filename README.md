qapers
======
A simple bash script to manage your library of scientific papers

qapers is a simple bash script manages a library of PDF files by allowing
the user to quickly find a file, open it in the default PDF viewer, and
maintain a separate directory of annotations on each PDF file. You can use
it to:

* Find a PDF file in a directory where you dump all your PDFs
* Pipe the results from the 'find' option to open a PDF of your choice
* Open a YAML annotations file to store your notes on the PDF
* Tag your PDFs using the YAML annotations file
* Review your previously stored annotations
* Export the bibliographic info of each PDF in BibTex format
* Export parts or all of your notes on any PDF in any format you wish

Features
--------
Detailed feature description coming soon

Installation
------------
Simply copy the `qapers` file from the repo to `/usr/local/bin`
(typically requires `sudo`) and change user access rights to make it
user executable.

Dependencies
------------
You need to have the following two packages installed to get the core
functionality right
- `yq`
    - `yq` is a lightweight and portable command-line YAML processor
    - https://mikefarah.gitbook.io/yq/
- `jq`
    - `jq` is a powerful and versatile Command-line JSON processor
    - Should be available via the package managers of standard distros.
    - Installation on Ubuntu: `sudo apt install jq`

Optional:
- `gvim`
    - I also use `vim-gnome` (i.e., `gvim`) as my YAML editor for
      annotations, but GEdit (which is installed on most distros by
      default) should work just as fine.
    - The important thing is to have an editor **that can be called from
      a script and that can open right at a specified line number of the
      given file**.


Example Usage
-------------
Examples and different use-cases coming soon

TO DO
-----
- [ ] Add more detailed features to README
- [ ] Add examples to README
- [ ] Add version numbering
- [x] Add `nautilus-sendto` functionality
- [ ] Add `set` functionality to set environment variables
- [ ] Add bash completion
- [ ] Add Bibtex export

LICENSE
-------

Copyright (C) 2020  Bedartha Goswami <bedartha@gmail.com>
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published
by the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU Affero General Public License for more details.

You should have received a copy of the GNU Affero General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
