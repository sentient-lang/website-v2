---
title: "Command-line interface: --optimise"
header: /cli
layout: default
---
# \-\-optimise

The 'optimise' option instructs Sentient to optimise machine code:

```bash
$ sentient --optimise program.json > program.min.json
```

Optimisation attempts to simplify the SAT problem contained in the machine code
so that it can solved more quickly. It does this by looking for tautologies and
contradictions within the SAT problem and propogating that information to other
clauses.

Optimisation is **strongly recommended** for programs that are going to be run
more than once or for programs that are going to be packaged for the web.
Optimisation depends on [Riss's Coprocessor](../solvers/riss). Please note that
it is **your responsibility** to ensure you comply with Riss's license if you
intend to use Sentient's optimisation feature.
