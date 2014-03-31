---
layout: front
title: fmrl
---

about
=====

**michael lowell roberts** is a creative computer scientist that has produced breakthroughs within the domain of parallel and distributed programming. his distributed actor-based server platform, used to build [the mmorpg horizons][horizons], is the *first elastic, distributed compute engine used for a production multiplayer game server*, long before the word "cloud" became a staple of the computer science lexicon.

he is the sole inventor of *the first parallelized incremental garbage collector*, an algorithm that eliminates performance penalties normally associated with garbage collection in multi-threaded environments. His collector is also an excellent example of how actor systems can applied to parallelize algorithms with complex state requirements-- an important area of programming that is still poorly understood by the software development industry at large.

projects & patents
==================

orleans (microsoft research)
----------------------------

[orleans][orleans] is a distributed actor system framework for the .NET framework developed by *microsoft research* that simplifies development of distributed systems for those already comfortable with object-oriented programming.

the nom garbage collector
-------------------------

**the nom garbage collector** is *the first parallelized, incremental garbage collection algorithm* and *was independently developed and patented by michael*. it is also *the first garbage collection algorithm capable of delivering real-time performance within a parallelized environment*.

please see [USPTO patent 8,200,718][nom/patent] for more details on the *nom* collector.

the **ramalloc** cached memory allocator
----------------------------------------

[ramalloc][ramalloc] is a parallelized, amortized-constant time memory allocator for objects smaller than a hardware page. it exhibits deterministic performance characteristics, which is necessary for soft real-time applications. it also reduces memory fragmentation, which is important for long-running processes. *ramalloc* is designed for game and interpreter development but should be useful for other applications as well. *ramalloc* is also parallelized; there is no global resource that requires serialized access.

the *ramalloc* source code is available under the [new BSD
license][ramalloc/license].

please read the [README][ramalloc/readme] file for details about project status and usage.

failure policies for C++
------------------------

[failure policies][nyan/fail_policy] are an experiment in abstracting exception handlers in C++ from the places where they're caught. 


[nom/patent]: http://patft.uspto.gov/netacgi/nph-Parser?Sect1=PTO1&Sect2=HITOFF&d=PALL&p=1&u=%2Fnetahtml%2FPTO%2Fsrchnum.htm&r=1&f=G&l=50&s1=8200718.PN.&OS=PN/8200718&RS=PN/8200718 
[nyan/fail_policy]: http://github.com/fmrl/nyan/blob/master/doc/failure-policies.markdown 
[orleans]: https://research.microsoft.com/en-us/projects/orleans
[ramalloc/license]: http://github.com/fmrl/ramalloc/blob/master/LICENSE.markdown
[ramalloc/readme]: http://github.com/fmrl/ramalloc/blob/master/README.markdown
[ramalloc]: http://github.com/fmrl/ramalloc
[horizons]: http://en.wikipedia.org/wiki/Horizons:_Empire_of_Istaria
