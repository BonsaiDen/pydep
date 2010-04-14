pydep
=====

**pydep** generates simple dependency listings and graphs for Python modules.

Usage::

    pydep dir [options] [extramodules]
    -q = Quiet mode
    -n = Don't generate the graph
    -u = Disable grouping
    -g = Group character(by default _ is used to split module names)
    -d = Density of the graph(10=very dense, 0=very loose, default=9)

Examples::

    pydep ~/projects/foo os time sys
    pydep ~/projects/bar -g -

| **Examples of rendered graphs(Right click and "Save as..."):**
| Atarashii_
| Python2.6_ (Warning 11000x6000 Pixels!)
| Tweepy_

.. _Atarashii: http://github.com/BonsaiDen/pydep/blob/master/atarashii.svg
.. _Python2.6: http://github.com/BonsaiDen/pydep/blob/master/python2.6.svg
.. _Tweepy: http://github.com/BonsaiDen/pydep/blob/master/tweepy.svg


Graph information
-----------------
**Nodes can have 3 types of information**

- [number] which show the number of modules the node depends on.
- (number) which show how many modules depend on this node.
- \* indicates that this node imports itself.

**Edges can have 3 types of arrows**

- Arrow, indicates a direct import via "import foo"
- Dot, indicates a partly import via "from foo import bar"
- Empty box, it seems that this import isn't used.

**Note:** Due to the dynamic nature of Python some of the edge information might 
be incorrect.


Contributing
------------

The source is available on GitHub_, to
contribute to the project, fork it on GitHub and send a pull request.
Everyone is welcome to make improvements to **pydep**!

.. _GitHub: http://github.com/BonsaiDen/pydep

License
=======

Copyright (c) 2010 Ivo Wetzel

**pydep** is free software: you can redistribute it and/or 
modify it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

**pydep** is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with
**pydep**. If not, see <http://www.gnu.org/licenses/>.

