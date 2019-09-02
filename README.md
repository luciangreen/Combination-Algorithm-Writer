# Combination-Algorithm-Writer
Combination Algorithm Writer

(Please note: Deprecated. See updated https://github.com/luciangreen/Combination-Algorithm-Writer-with-Predicates (a different repository) instead).

Combination Algorithm Writer is a SWI-Prolog algorithm that finds combinations of given commands that satisfy the given input and output.

Installation
Load all files in the form:
['filename'].

Running

caw00(off,f,[[append,2,1],[delete,2,1],[head,1,1],[tail,1,1],[member,1,1]],50,7,[[a,1]],[[b,1]],[],Program).
Program = [f,[1,b]],[[f,[a,b],:-,[[=,[b,a]]]]],[[b,1]]
(Press ";" for more results).

Note:
Use (:-) instead of :-.
