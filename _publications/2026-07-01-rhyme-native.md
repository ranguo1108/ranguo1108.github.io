---
title: "Rhyme Native: Efficient Code Generation for Structured and Semi-Structured Workloads"
collection: publications
category: conferences
permalink: /publication/2026-07-01-rhyme-native
excerpt: 'A single declarative query language, Rhyme, that compiles both relational (SQL) and nested JSON queries to efficient native C code, matching state-of-the-art compiled engines on TPC-H and outperforming JSON-capable databases on JSONBench.'
date: 2026-07-01
venue: 'Proceedings of the VLDB Endowment (PVLDB), Vol. 19, No. 11'
paperurl: 'https://www.vldb.org/pvldb/vol19/p3676-guo.pdf'
citation: '<b>Ran Guo</b> and Tiark Rompf. (2026). &quot;Rhyme Native: Efficient Code Generation for Structured and Semi-Structured Workloads.&quot; <i>Proceedings of the VLDB Endowment</i>, 19(11), 3676&ndash;3688. <a href="https://doi.org/10.14778/3836663.3836717">doi:10.14778/3836663.3836717</a>'
---

**Abstract.** Modern data processing spans two worlds: flat relational tables, served by decades of database research producing highly optimized query engines, and nested semi-structured data such as JSON, for which expressive query languages exist but compilation and optimization techniques have been applied far less comprehensively. We ask whether a single query language can express both regimes naturally while compiling to efficient native code. We build on Rhyme, a declarative language whose object-notation syntax mirrors the structure of query results, and contribute on three fronts. We refine Rhyme's semantics for generator binding and missing values, allowing co-iteration, inner/outer joins, and nested-loop traversals to be expressed under different uses of generator symbols. We show that Rhyme's prior dependency-driven loop scheduler can generate incorrect code on hierarchical queries, and present a new scheduler based on finer-grained per-statement constraints that ensures correctness. We introduce a gradual type system and a C code generation backend that emits tag-less, statically typed code and specializes data loading and internal data structures for idiomatic SQL patterns. Our system matches state-of-the-art compiled engines on SQL workloads such as TPC-H and outperforms modern JSON-capable databases and DSLs on JSONBench and other hierarchical queries.

[Paper (PDF)](https://www.vldb.org/pvldb/vol19/p3676-guo.pdf) · [ACM Digital Library](https://dl.acm.org/doi/10.14778/3836663.3836717)
