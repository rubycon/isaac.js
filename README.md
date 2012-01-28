# isaac.js
*isaac.js* is a javascript implementation of [ISAAC](http://www.burtleburtle.net/bob/rand/isaac.html).

ISAAC is a [CSPRNG](http://en.wikipedia.org/wiki/CSPRNG) designed by [Robert J. Jenkins Jr.](http://burtleburtle.net/bob/) in 1996 and based on RC4. It is designed to be fast and secure.

*isaac.js* is fully compatible with other *32-bit integer arithmetic* implementations of ISAAC and can be used as a good alternative to the default javascript `Math.random()` function.

##Usage
Include isaac.js into your html file: `<script src="isaac.js"></script>`.
Then just call `isaac.random()` to get a random real number between 0 and 1 :

`var random_number = isaac.random();`

If you want a little more control over the PRNG you can reset isaac (all internals to zero) using `isaac.reset()` or use a new seed using `isaac.seed(s)` (*s* can be a string, a number or an array of number). You can also run the prng an arbitrary number of time before querying a new random output using `isaac.prng()`.

##Licence
###isaac.js is released under the [MIT Licence](http://www.opensource.org/licenses/MIT):
Copyright (c) 2012 Yves-Marie K. Rinquin

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
