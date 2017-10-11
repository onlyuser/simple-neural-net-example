[![Build Status](https://secure.travis-ci.org/onlyuser/simple-neural-net-example.png)](http://travis-ci.org/onlyuser/simple-neural-net-example)

simple-neural-net-example
=========================

Copyright (C) 2011-2017 <mailto:onlyuser@gmail.com>

About
-----

simple-neural-net-example is a simple neural net example.

Net Topology
------------

![picture alt](https://sites.google.com/site/onlyuser/files/bpnet_graph.jpg "simple-neural-net-example")

<pre>
layer0          layer1                 layer2

[v0]------w00---[out0|err0]------w20---[out2|err2|v2]
   \            /  |                   /  |
    \  *--w01--*  w02         *--w21--*  w22
     \/           /          /           /
     /\          /          /           /
    /  *--w10--*/          /           /
   /           /\         /           /
[v1]------w11---[out1|err1]          /
             /     |                /
       *----*     w12         *----*
      /           /          /
     /   *-------*          /
    /   /                  /
   /   /                  /
[b0]--*                [b1]

bias==1                bias==1
</pre>

Training Data (XOR)
-------------------

<table>
    <tr><th> input0 </th><th> input1 </th><th> output </th></tr>
    <tr><td> 0 </td><td> 0 </td><td> 0 </td></tr>
    <tr><td> 0 </td><td> 1 </td><td> 1 </td></tr>
    <tr><td> 1 </td><td> 0 </td><td> 1 </td></tr>
    <tr><td> 1 </td><td> 1 </td><td> 0 </td></tr>
</table>

Make Targets
------------

<table>
    <tr><th> target </th><th> action                        </th></tr>
    <tr><td> all    </td><td> make binaries                 </td></tr>
    <tr><td> test   </td><td> all + run tests               </td></tr>
    <tr><td> clean  </td><td> remove all intermediate files </td></tr>
</table>

Requirements
------------

Unix tools and 3rd party components (accessible from $PATH):

    gcc

Installation
------------

git clone https://github.com/onlyuser/simple-neural-net-example.git

References
----------

<dl>
    <dt>"Backpropagation"</dt>
    <dd>https://en.wikipedia.org/wiki/Backpropagation</dd>
</dl>

Keywords
--------

    backpropagation neural net
