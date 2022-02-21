# bench-sets

This resource provides a list of optimisation problem benchmarking sets for evolutionary computation. The list is attached to the paper "Benchmarking in Optimization: Best Practice and Open Issues", see https://arxiv.org/abs/2007.03488. 

1. *Artificial discrete optimization problems*.

    Subjectively, this area is among those with the largest number of benchmark sets. Here, many are inspired by problems encountered in the real world, which then have given rise to many fundamental problems in computer science. Noteworthy subareas of discrete optimization are combinatorial optimization, integer and constraint programming - and for many of them large sets of historically grown sets of benchmarks exist. Examples include the Boolean satisfiability and maximum satisfiability competitions (http://www.satcompetition.org/, https://maxsat-evaluations.github.io/), travelling salesperson problem library (http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/ and http://www.math.uwaterloo.ca/tsp/index.html) and the mixed integer programming library (https://miplib.zib.de/). 
    
    In contrast to these, instance-driven sets are the more abstract models that define variable interactions at the lowest level (i.e., independent of a particular problem) and then construct an instance based on fundamental characteristics. Noteworthy examples here are (for binary representations) the NK landscapes (Kauffman, 1993), which has the idea of tunable ruggedness at its core, the W-Model (Weise & Wu, 2018) with configurable features like length, neutrality, epistasis, multi-objectivity, objective values, and ruggedness, and the Pseudo-Boolean Optimization (PBO) suite of 23 binary benchmark functions by (Doerr *et al.*, 2020), which covers a wide range of landscape features and which extends the W-model in various ways (in particular, superposing its transformations to other base problems).

2. *Artificial real-parameter problems*.

    Benchmark suites have been defined for special sessions, workshops and competitions at both the Association for Computing Machinery (ACM) Genetic and Evolutionary Computation Conference (GECCO) and the Institute of Electrical and Electronics Engineers (IEEE) Congress on Evolutionary Computation (CEC). Documentation and code are available online - for GECCO Black-Box-Optimization-Benchmarking (BBOB) https://coco.gforge.inria.fr, and for CEC https://github.com/P-N-Suganthan/2020-Bound-Constrained-Opt-Benchmark.


## References
* Carola Doerr, Furong Ye, Naama Horesh, Hao Wang, Ofer M. Shir, and Thomas Back. Benchmarking Discrete Optimization Heuristics with IOHprofiler. *Applied Soft Computing*, 88:106027, 2020.
* Stuart A. Kauffman. *The Origins of Order: Self-Organization and Selection in Evolution*. Oxford University Press, USA, 1993.
* Thomas Weise and Zijun Wu. Difficult features of combinatorial optimization problems and the tunable W-model benchmark problem for simulating them. In *Proceedings of the Genetic and Evolutionary Computation Conference Companion*, GECCO '18, pages 1769-1776. ACM, 2018. ISBN 9781450357647.
