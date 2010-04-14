pydep
=====

**pydep** generates simple dependency listings and graphs for Python modules.

Usage::

    pydep dir [options] [extramodules]
    -q = Quiet mode
    -n = Don't generate the graph
    -u = Disable grouping
    -g = Group character(by default _ is used to split module names)

Examples::

    pydep ~/projects/foo os time sys
    pydep ~/projects/bar -g -

| **Examples of rendered graphs:**
| Atarashii_
| Python2.6_ (Warning 1.8MiB PNG!)
| Tweepy_

.. _Atarashii: http://github.com/BonsaiDen/pydep/blob/master/atarashii.png
.. _Python2.6: http://github.com/BonsaiDen/pydep/blob/master/python26.png
.. _Tweepy: http://github.com/BonsaiDen/pydep/blob/master/tweepy.png


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

