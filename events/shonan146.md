---
title: NII Shonan Seminar No. 146
layout: default
---

## Programming and Reasoning with Algebraic Effects and Effect Handlers

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

The increased adoption and use of algebraic effects and effect
handlers reveal and make pressing three main problems: reasoning,
performance, and typing. These problems may appear disparate, but we
believe there are in fact deep connections that bring them together.

**Reasoning** Algebraic effects are defined by a signature of operations
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

**Performance** The dominant implementation method, the free monad, is
notably slower than the direct execution of side-effects where
available. A range of approaches for improving performance are under
active investigation. These include direct stack manipulation, in the
case that continuations are used linearly, selective CPS translations,
and fusion transformations. The jury is still out on which techniques
work best in which situations.

**Typing** Programming in the large involves working with complex and
interacting systems. Effect type systems are a powerful means of
taming this complexity, in a way that is amenable for practical
programming. Several different effect type systems have been
introduced for algebraic effects and effect handlers. It is not clear
yet precisely what the tradeoffs are between the different
approaches. Many open questions remain over how best to support
features such as generative effects, and how to leverage effect type
systems to support reasoning and to improve performance.

Given the complexity of these problems and their importance, we
believe the face-to-face meeting of main community representatives
will promote their solution. We identify five specific application
areas to be discussed at the meeting in the context of the three main
problem areas:

- Effect handlers for concurrent and distributed programming;
- Effect handlers for generative effects (ML references, renaming effects, scoped effects, modularity, runST, existentials);
- Effect handlers with behavioral types (parameterized monads, graded monads, type state, session types, answer type modification, dependent types);
- Effect handlers and resource management;
- Effect handlers for probabilistic programming.

To promote mutual understanding, we plan for the workshop to have
substantial time available for discussion. Our hope is to emphasize
tutorials, brainstorming, and working-group sessions, rather than mere
conference-like presentations.

The field of effect handlers is thriving, and we believe that Shonan
would be an ideal setting to bring researchers interested in the topic
together. A previous meeting held at Dagstuhl in March 2016, entitled
“From Theory to Practice of Algebraic Effects and Handlers” had more
people willing to participate than it was possible to
accommodate. Since then, the field has grown, and so we anticipate
that there will be an abundance of interest in attending this meeting.


### Organisers

- [Oleg Kiselyov](http://okmij.org/ftp/), Tohoku University, Japan
- [Sam Lindley](http://homepages.inf.ed.ac.uk/slindley), The University of Edinburgh, UK
- [Gordon Plotkin](http://homepages.inf.ed.ac.uk/gdp/), The University of Edinburgh, UK
- [Nicolas Wu](http://zenzike.com/), University of Bristol, UK


### Participants

- Danel Ahman, University of Ljubljana, Slovenia
- Nada Amin, University of Cambridge, UK
- Robert Atkey, University of Strathclyde, UK
- Oliver Bračevac, TU Darmstadt, Germany
- Edwin Brady, University of St Andrews, UK
- Youyou Cong, Ochanomizu University, Japan
- Stephen Dolan, University of Cambridge, UK
- Jeremy Gibbons, University of Oxford, UK
- Daniel Hillerström, The University of Edinburgh, UK
- Atsushi Igarashi, Kyoto University, Japan
- Mauro Jaskelioff, Universidad Nacional de Rosario / CONICET, Argentina
- Yukiyoshi Kameyama, University of Tsukuba, Japan
- Ohad Kammar, University of Oxford, UK
- Shin-ya Katsumata, National Institute of Informatics, Japan
- Daan Leijen, Microsoft Research, USA
- Conor McBride, University of Strathclyde, UK
- James McKinna	LFCS, The University of Edinburgh, UK
- Craig McLaughlin, The University of Edinburgh, UK
- Shin-Cheng Mu, Academia Sinica, Taiwan
- Maciej Pirog, University of Wroclaw, Poland
- Andreas Rossberg, Dfinity Foundation, Germany
- Tom Schrijvers, KU Leuven, Belgium
- KC Sivaramakrishnan, IIT Madras, India
- Leo White, Jane Street, UK
- Jeremy Yallop, University of Cambridge, UK
- Nick Benton, Facebook, UK
- Philipp Schuster, Universitat Tubingen, Germany
- Max New, Northeastern University, USA


### Schedule

The full schedule is to be announced.

#### Sunday, March 24, 2019

- 15:00 -- : Check-in
- 19:00 -- 21:00: Welcome banquet

#### Monday, March 25, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch

#### Tuesday, March 26, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch

#### Wednesday, March 27, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch

#### Thursday, March 28, 2019

- 07:30 -- 09:00: Breakfast
- 12:00 -- 13:30: Lunch

#### Friday, March 29, 2019

07:30 -- 09:00: Breakfast
12:00 -- 13:30: Lunch