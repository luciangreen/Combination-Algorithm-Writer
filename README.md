# Combination-Algorithm-Writer
Combination Algorithm Writer

(Please note: Deprecated. See updated https://github.com/luciangreen/Combination-Algorithm-Writer-with-Predicates (a different repository) instead).

Combination Algorithm Writer is a SWI-Prolog algorithm that finds combinations of given commands that satisfy the given input and output.


# Installation from List Prolog Package Manager (LPPM)

* Optionally, you can install from LPPM by installing <a href="https://www.swi-prolog.org/build/">SWI-Prolog</a> for your machine, downloading the <a href="https://github.com/luciangreen/List-Prolog-Package-Manager">LPPM Repository</a>,
```
git clone https://github.com/luciangreen/List-Prolog-Package-Manager.git
```
loading LPPM with `['lppm'].` then installing the package by running `lppm_install("luciangreen","Combination-Algorithm-Writer").`.

Installation
Load all files in the form:
```
['listprologinterpreter1listrecursion4 copy 52'].
['listprologinterpreter3preds5 copy 52'].
['caw5 copy 11'].
```
Running

```
caw00(off,f,[[append,2,1],[delete,2,1],[head,1,1],[tail,1,1],[member,1,1]],50,7,[[a,1]],[[b,1]],[],Program).
Program = [f,[1,b]],[[f,[a,b],:-,[[=,[b,a]]]]],[[b,1]]
(Press ";" for more results).
```

```
caw00(off,f,[[+,2,1]],4,8,[[a,1],[b,1],[c,2]],[[e,4]],[],P),writeln(P).
[[f,[a,b,c,e],:-,[[+,[c,c,h]],[=,[e,h]]]]]
```

```
caw00(off,f,[[+,2,1]],4,8,[[a,1],[b,1],[c,2],[d,1]],[[e,5]],[],P),writeln(P). 
[[f,[a,b,c,d,e],:-,[[+,[a,c,g]],[+,[c,g,h]],[=,[e,h]]]]]
.
.
.
```

Note:
Use (:-) instead of :-.
