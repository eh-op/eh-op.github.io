---
title: NII Shonan Seminar no. 146
layout: default
---

## Programming and Reasoning with Algebraic Effects and Effect Handlers

Jump to [Schedule](#schedule) -- [Organisers](#organisers) -- [Participants](#participants).

### Overview

Algebraic effects and effect handlers are becoming an increasingly
popular approach for expressing and composing computational
effects. There are implementations of algebraic effects and effect
handlers in Clojure, F#, Haskell, Idris, Javascript, OCaml,
PureScript, Racket, Scala, Scheme, Standard ML, and even C. There are
full-fledged languages built around effects such as Eff, Frank, Links,
Koka, and Multicore OCaml. Moreover, there is growing interest from
industry in effect handlers. For instance, Facebook’s React library
for JavaScript UI programming is directly inspired by effect handlers,
and Uber’s recently released Pyro tool for probabilistic programming
and deep learning relies on effect handlers. Such interest arises from
the ease of combining in the same program independently developed
components using algebraic effects and effect handlers.

<details><summary class="collapsible">[Read more]</summary>
<p>
The increased adoption and use of algebraic effects and effect
handlers reveal and make pressing three main problems: reasoning,
performance, and typing. These problems may appear disparate, but we
believe there are in fact deep connections that bring them together.
</p>

<p>
<strong>Reasoning</strong>&nbsp;&nbsp; Algebraic effects are defined by a signature of operations
and an equational theory that describes how the operations interact,
providing direct support for reasoning. Effect handlers are modular
interpreters for algebraic effects, giving meaning to such
operations. Existing implementations of effect handlers dispense with
equations, largely because many open questions remain about how to
incorporate them into a programming language. A key question that this
meeting will seek to address is how to reintroduce equations and other
forms of reasoning back into the effect handlers picture. An important
consideration here is how to combine equational theories for several
interacting effects.
</p>

<p>
<strong>Performance</strong>&nbsp;&nbsp; The dominant implementation method, the free monad, is
notably slower than the direct execution of side-effects where
available. A range of approaches for improving performance are under
active investigation. These include direct stack manipulation, in the
case that continuations are used linearly, selective CPS translations,
and fusion transformations. The jury is still out on which techniques
work best in which situations.
</p>

<p>
<strong>Typing</strong>&nbsp;&nbsp; Programming in the large involves working with complex and
interacting systems. Effect type systems are a powerful means of
taming this complexity, in a way that is amenable for practical
programming. Several different effect type systems have been
introduced for algebraic effects and effect handlers. It is not clear
yet precisely what the tradeoffs are between the different
approaches. Many open questions remain over how best to support
features such as generative effects, and how to leverage effect type
systems to support reasoning and to improve performance.
</p>

<p>
Given the complexity of these problems and their importance, we
believe the face-to-face meeting of main community representatives
will promote their solution. We identify five specific application
areas to be discussed at the meeting in the context of the three main
problem areas:

<ul>
  <li>Effect handlers for concurrent and distributed programming;</li>
  <li>Effect handlers for generative effects (ML references, renaming effects, scoped effects, modularity, runST, existentials);</li>
  <li>Effect handlers with behavioral types (parameterized monads, graded monads, type state, session types, answer type modification, dependent types);</li>
  <li>Effect handlers and resource management;</li>
  <li>Effect handlers for probabilistic programming.</li>
</ul>

To promote mutual understanding, we plan for the workshop to have
substantial time available for discussion. Our hope is to emphasize
tutorials, brainstorming, and working-group sessions, rather than mere
conference-like presentations.
</p>

<p>
The field of effect handlers is thriving, and we believe that Shonan
would be an ideal setting to bring researchers interested in the topic
together. A previous meeting held at <a href="https://www.dagstuhl.de/en/program/calendar/semhp/?semnr=18172">Dagstuhl in March 2016, entitled
"<i>From Theory to Practice of Algebraic Effects and Handlers</i>"</a> had more
people willing to participate than it was possible to
accommodate. Since then, the field has grown, and so we anticipate
that there will be an abundance of interest in attending this meeting.
</p>
</details>

### Organisers

- [Oleg Kiselyov](http://okmij.org/ftp/), Tohoku University, Japan
- [Sam Lindley](http://homepages.inf.ed.ac.uk/slindley), The University of Edinburgh, UK
- [Gordon Plotkin](http://homepages.inf.ed.ac.uk/gdp/), The University of Edinburgh, UK
- [Nicolas Wu](http://zenzike.com/), University of Bristol, UK


### Participants

- [Danel Ahman](https://danelahman.github.io/), University of Ljubljana, Slovenia
- [Nada Amin](http://namin.org/), University of Cambridge, UK
- [Robert Atkey](https://bentnib.org/), University of Strathclyde, UK
- [Oliver Bračevac](https://www.stg.tu-darmstadt.de/staff/oliver_bracevac_menu/oliver_bracevac.en.jsp), TU Darmstadt, Germany
- [Edwin Brady](https://edwinb.wordpress.com/), University of St Andrews, UK
- [Youyou Cong](https://sites.google.com/site/youyoucong212/), Ochanomizu University, Japan
- [Stephen Dolan](http://stedolan.net/), University of Cambridge, UK
- [Jeremy Gibbons](http://www.cs.ox.ac.uk/jeremy.gibbons/), University of Oxford, UK
- [Daniel Hillerström](https://dhil.net/research), The University of Edinburgh, UK
- [Atsushi Igarashi](https://www.fos.kuis.kyoto-u.ac.jp/~igarashi/index.html.en), Kyoto University, Japan
- [Mauro Jaskelioff](https://www.fceia.unr.edu.ar/~mauro/), Universidad Nacional de Rosario / CONICET, Argentina
- [Yukiyoshi Kameyama](http://www.cs.tsukuba.ac.jp/~kam/), University of Tsukuba, Japan
- [Ohad Kammar](http://www.denotational.co.uk/), The University of Edinburgh, UK
- [Shin-ya Katsumata](http://group-mmm.org/~s-katsumata/index-e.html), National Institute of Informatics, Japan
- [Daan Leijen](https://www.microsoft.com/en-us/research/people/daan/), Microsoft Research, USA
- [Conor McBride](https://personal.cis.strath.ac.uk/conor.mcbride/), University of Strathclyde, UK
- [James McKinna](http://homepages.inf.ed.ac.uk/jmckinna/), The University of Edinburgh, UK
- [Craig McLaughlin](http://homepages.inf.ed.ac.uk/s1544843/), The University of Edinburgh, UK
- [Shin-Cheng Mu](https://www.iis.sinica.edu.tw/pages/scm/), Academia Sinica, Taiwan
- [Max New](https://maxsnew.github.io/), Northeastern University, USA
- [Maciej Pirog](http://www.ii.uni.wroc.pl/~mpirog/), University of Wroclaw, Poland
- [Andreas Rossberg](https://people.mpi-sws.org/~rossberg/), Dfinity Foundation, Germany
- [Tom Schrijvers](https://people.cs.kuleuven.be/~tom.schrijvers/), KU Leuven, Belgium
- [Philipp Schuster](http://ps.informatik.uni-tuebingen.de/team/schuster/), Universität Tübingen, Germany
- [KC Sivaramakrishnan](http://kcsrk.info/), IIT Madras, India
- [Leo White](http://www.lpw25.net/), Jane Street, UK
- [Jeremy Yallop](https://www.cl.cam.ac.uk/~jdy22/), University of Cambridge, UK
- [Yizhou Zhang](http://www.cs.cornell.edu/~yizhou/), Cornell University, USA


### Schedule

The full schedule is to be announced.

#### Sunday, March 24, 2019

- 15:00 -- : Check-in
- 19:00 -- 21:00: Welcome banquet

#### Monday, March 25, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch
- 18:00 -- 19:30: Dinner

#### Tuesday, March 26, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch
- 18:00 -- 19:30: Dinner

#### Wednesday, March 27, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch
- 13:30 -- 20:45: Excursion and dinner (TBC)

#### Thursday, March 28, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch
- 18:00 -- 19:30: Dinner

#### Friday, March 29, 2019

- 07:30 -- 09:00: Checkout and breakfast
- 12:00 -- 13:30: Lunch
