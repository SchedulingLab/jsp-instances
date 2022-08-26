# Job-shop instances

This repository is the merge of two other repositories:

- [tamy0612/JSPLIB](https://github.com/tamy0612/JSPLIB) (JSON file, classical instances)
- [strassl/jssp-instances](https://github.com/strassl/jssp-instances) (classical instances, gen instances)

and a paper:

- [Large-Scale Benchmarks for the Job Shop Scheduling Problem](https://arxiv.org/abs/2102.08778)


Data about the classical instances can be found on [jobshop.jjvh.nl](http://jobshop.jjvh.nl/)

WARNING! Data may not be accurate. If you find an error, please report an issue. Always refer to the original paper.


## Classical instances

Description in [classical.json](classical.json).

- `abz` (5 instances [1])
- `dmu` (80 instances [8])
- `ft` (3 instances [2])
- `la` (40 instances [3])
- `orb` (10 instances [4])
- `swv` (20 instances [5])
- `ta` (80 instances [7])
- `yn` (4 instances [6])

## Generated instances

Description in [generated.json](generated.json)

- `gen` (4225 instances, [9])

The (initial) bounds for these instances have been computed as follows:

- The lower bound has been computed as the maximum of the sums of operations time for a same job on the one hand, and for the same machine on the other hand.
- The upper bound has been computed as the makespan of a list scheduling where each operation number 1 of each job (in increasing index order) has been put in the schedule as earlier as possible, then operation number 2 of each job, and so on.

This has given 123 non-trivial instances (with more than 1 job and 1 machine) with lower bound equal to upper bound.

## Large instances

Description in [large.json](large.json)

- `ko` (24 instances, [10])
- `lta` (90 instances, [10])

The (initial) bounds for `lta` have been computed as before. This has given 11 instances with lower bound equal to upper bound. The optimum makespan for `ko` is 600000 by construction of the instances.

## References

1. J. Adams, E. Balas, D. Zawack. "The shifting bottleneck procedure for job shop scheduling.", Management Science, Vol. 34, Issue 3, pp. 391-401, 1988.
2. J.F. Muth, G.L. Thompson. "Industrial scheduling.", Englewood Cliffs, NJ, Prentice-Hall, 1963.
3. S. Lawrence. "Resource constrained project scheduling: an experimental investigation of heuristic scheduling techniques (Supplement).", Graduate School of Industrial Administration. Pittsburgh, Pennsylvania, Carnegie-Mellon University, 1984.
4. D. Applegate, W. Cook. "A computational study of job-shop scheduling.", ORSA Journal on Computer, Vol. 3, Isuue 2, pp. 149-156, 1991.
5. R.H. Storer, S.D. Wu, R. Vaccari. "New search spaces for sequencing problems with applications to job-shop scheduling.", Management Science Vol. 38, Issue 10, pp. 1495-1509, 1992.
6. T. Yamada, R. Nakano. "A genetic algorithm applicable to large-scale job-shop problems.", Proceedings of the Second international workshop on parallel problem solving from Nature (PPSN'2). Brussels (Belgium), pp. 281-290, 1992.
7. E. Taillard. "Benchmarks for basic scheduling problems", European Journal of Operational Research, Vol. 64, Issue 2, pp. 278-285, 1993.
8. E. Demirkol, S. Mehta, R. Uzsoy. "Benchmarks for shop scheduling problems", European Journal of Operational Research, Vol. 109, Issue 1, pp. 137--141, 1998.
9. S. Strassl and N. Musliu. "Instance space analysis and algorithm selection for the job shop scheduling problem", Computers & Operations Research, Vol. 141, 2022.
10. G. Da Col, E. Teppan. "Large-Scale Benchmarks for the Job Shop Scheduling Problem", 2021.
