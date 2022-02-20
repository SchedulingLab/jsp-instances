# Job-shop instances

This repository is the merge of two other repositories:

- [tamy0612/JSPLIB](https://github.com/tamy0612/JSPLIB) (JSON file, classical instances)
- [strassl/jssp-instances](https://github.com/strassl/jssp-instances) (classical instances, gen instances)

Data about the classical instances can be found on [jobshop.jjvh.nl](http://jobshop.jjvh.nl/)

WARNING! Data may not be accurate. If you find an error, please report an issue. Always refer to the original paper.


## Classical instances

Description in [classical.json](classical.json).

- `abz`
- `dmu`
- `ft`
- `la`
- `orb`
- `swv`
- `ta`
- `yn`

## Generated instances

Description in [generated.json](generated.json)

- `gen`

The (initial) bounds for these instances have been computed as follows:

- The lower bound has been computed as the maximum of the sums of operations time for a same job on the one hand, and for the same machine on the other hand.
- The upper bound has been computed as the makespan of a list scheduling where each operation number 1 of each job (in increasing index order) has been put in the schedule as earlier as possible, then operation number 2 of each job, and so on.

This has given 123 non-trivial instances (with more than 1 job and 1 machine) with lower bound equal to upper bound.
