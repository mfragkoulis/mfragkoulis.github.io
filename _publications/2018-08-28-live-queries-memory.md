---
title: "Live interactive queries to a software application's memory profile"
collection: publications
permalink: /publication/2018-08-28-live-queries-memory.md
excerpt: "Memory operations are critical to an application's reliability and performance. To reason about their correctness and track opportunities for optimisations, sophisticated instrumentation frameworks, such as Valgrind and Pin, have been developed. Both provide only limited facilities for analysing the collected data. This work presents a Valgrind's extension for examining a software applications' dynamic memory profile through live interactive analysis with SQL. The Pico COllections Query Library (PiCO QL) module maps Valgrind's data structures that contain the instrumented application's memory operations metadata to a relational interface. Queries are type-safe and the module imposes only a trivial overhead when idle. We evaluate our approach on ten applications and through a qualitative study. We find 900KB of undefined bytes in bzip2 that account for 12% of its total memory use and a performance-critical code execution path in the Unix commands sort and uniq. The referenced functions are part of glibc and have been independently modified to boost the library's performance. The qualitative study has users rate the usefulness, usability, effort, correctness, and expressiveness of PiCO QL queries compared to Python scripts. The findings indicate that querying with PiCO QL incurs lower user effort."

date: 2018-08-28
venue: 'IET Software'
paperurl: 'http://ietdl.org/t/uIR5q'
citation: "Marios Fragkoulis, Diomidis Spinellis, and Panos Louridas. (2018). &quot;Live interactive queries to a software application's memory profile.&quot; IET Software."
---

