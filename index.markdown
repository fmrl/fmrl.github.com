---
layout: front
title: fmrl
---

ramalloc
--------

[ramalloc][ramalloc] is a parallelized, amortized-constant time allocator for objects smaller than a hardware page. it exhibits deterministic performance characteristics, which is necessary for soft real-time applications. it also reduces memory fragmentation, which is important for long-running processes. *ramalloc* is designed for game and interpreter development but should be useful for other applications as well. *ramalloc* is also parallelized; there is no global resource that requires serialized access.

*ramalloc* source code is available under the [New BSD
License][ramalloc/license].

please read the [README][ramalloc/readme] file for details about project status and usage.

[ramalloc]: http://github.com/fmrl/ramalloc
[ramalloc/license]: http://github.com/fmrl/ramalloc/blob/master/LICENSE.markdown
[ramalloc/readme]: http://github.com/fmrl/ramalloc/blob/master/README.markdown

---

failure policies
----------------

[failure policies][nyan/fail_policy] abstract exception handlers in C++ from the places where they’re caught. 

[nyan/fail_policy]: http://github.com/fmrl/nyan/blob/master/doc/failure-policies.markdown 


