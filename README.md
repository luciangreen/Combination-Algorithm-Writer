# Combination-Algorithm-Writer
Combination Algorithm Writer

(Please note: Deprecated. See updated https://github.com/luciangreen/Combination-Algorithm-Writer-with-Predicates (a different repository) instead).

Combination Algorithm Writer is a SWI-Prolog algorithm that finds combinations of given commands that satisfy the given input and output.

# Prerequisites

* Use a search engine to find the Homebrew (or other) Terminal install command for your platform and install it, and search for the Terminal command to install swipl using Homebrew and install it or download and install SWI-Prolog for your machine at <a href="https://www.swi-prolog.org/build/">SWI-Prolog</a>.

# Mac, Linux and Windows (with Linux commands installed): Prepare to run swipl

* In Terminal settings (Mac), make Bash the default shell:

```
/bin/bash
```

* In Terminal, edit the text file `~/.bashrc` using the text editor Nano:

```
nano ~/.bashrc
```

* Add the following to the file `~/.bashrc`:

```
export PATH="$PATH:/opt/homebrew/bin/"
```

* Link to swipl in Terminal:

```
sudo ln -s /opt/homebrew/bin/swipl /usr/local/bin/swipl
```

# 1. Install manually

Download <a href="http://github.com/luciangreen/Combination-Algorithm-Writer/">this repository</a>.

# 2. Or Install from List Prolog Package Manager (LPPM)

* Download the <a href="https://github.com/luciangreen/List-Prolog-Package-Manager">LPPM Repository</a>:

```
mkdir GitHub
cd GitHub/
git clone https://github.com/luciangreen/List-Prolog-Package-Manager.git
cd List-Prolog-Package-Manager
swipl
['lppm'].
lppm_install("luciangreen","Combination-Algorithm-Writer").
../
halt.
```

# Running

* In Shell:
`cd Combination-Algorithm-Writer`
`swipl`
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
