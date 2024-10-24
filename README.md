# Prattle: A Pratt Parser & Parser Generator in Rust

This is an illustration of a flexible and dynamically extensible Pratt parser design. [Here is an article about it.](https://www.robertjacobson.dev/designing-a-pratt-parser-generator)

## What is a Pratt parser?

A parser reads in text and recognizes it, transforming it into an internal format the computer can understand. The Pratt
parsing algorithm is one of the most useful and elegant of the parsing algorithms yet has suffered obscurity for
decades. It is especially adept at parsing expression grammars. To read more about it, check out these resources:

* [Parsing Expressions by Recursive Descent](http://www.engr.mun.ca/~theo/Misc/exp_parsing.htm)
* [From Precedence Climbing to Pratt Parsing](http://www.engr.mun.ca/~theo/Misc/pratt_parsing.htm)
* [Andy Chu’s coverage on his blog](https://www.oilshell.org/blog/2017/03/31.html)

## Which is it, a parser or a parser generator?

It is neither or both. Most Pratt parser designs hard-code the operator data into the source code for no real benefit.
But doing so severely limits the flexibility of the resulting parser. What makes one Pratt parser different from another
is often only the operator data. If you separate the operator data from the code, you get a *universal* expression
parser with all the same efficiency and ease of use of any other Pratt parser. You can even modify the operator data at
run time. For more information, [read this article.](https://www.robertjacobson.dev/designing-a-pratt-parser-generator)

## Authors and License

© Copyright 2019-2022 Robert Jacobson

 Released under the MIT license.

Permission is hereby granted, free of charge, to any person obtaining  a copy of this software and associated documentation files (the  "Software"), to deal in the Software without restriction, including  without limitation the rights to use, copy, modify, merge, publish,  distribute, sublicense, and/or sell copies of the Software, and to  permit persons to whom the Software is furnished to do so, subject to  the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,  EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF  MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY  CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,  TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE  SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
