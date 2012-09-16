This is an Awk script copied from http://code.google.com/p/line-counting/ originally written to compute C code metrics and modified to calculate nested comments as in Scala. It looks at code and comments via regular expressions and computes:

* Lines of code (non-blank)
* Number of comments (multiline and single-line accounted for)
* Raw lines of text
* Total code
* Total comments
* Comment percentage 

Usage
-----

Run it like so::

	awk -f lc.awk $(find /project/dir -name "*.scala")

