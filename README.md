# bench-sets

This resource provides a list of optimisation problem benchmarking sets for evolutionary computation. The list is attached to the paper "Benchmarking in Optimization: Best Practice and Open Issues", see https://arxiv.org/abs/2007.03488. 

1. *Artificial discrete optimization problems*.

    Subjectively, this area is among those with the largest number of benchmark sets. Here, many are inspired by problems encountered in the real world, which then have given rise to many fundamental problems in computer science. Noteworthy subareas of discrete optimization are combinatorial optimization, integer and constraint programming &ndash; and for many of them large sets of historically grown sets of benchmarks exist. Examples include the Boolean satisfiability and maximum satisfiability competitions (http://www.satcompetition.org/, https://maxsat-evaluations.github.io/), travelling salesperson problem library (http://comopt.ifi.uni-heidelberg.de/software/TSPLIB95/ and http://www.math.uwaterloo.ca/tsp/index.html) and the mixed integer programming library (https://miplib.zib.de/). 
    
    In contrast to these, instance-driven sets are the more abstract models that define variable interactions at the lowest level (i.e., independent of a particular problem) and then construct an instance based on fundamental characteristics. Noteworthy examples here are (for binary representations) the NK landscapes (Kauffman, 1993), which has the idea of tunable ruggedness at its core, the W-Model (Weise & Wu, 2018) with configurable features like length, neutrality, epistasis, multi-objectivity, objective values, and ruggedness, and the Pseudo-Boolean Optimization (PBO) suite of 23 binary benchmark functions by (Doerr *et al.*, 2020), which covers a wide range of landscape features and which extends the W-model in various ways (in particular, superposing its transformations to other base problems).

2. *Artificial real-parameter problems*.

    Benchmark suites have been defined for special sessions, workshops and competitions at both the Association for Computing Machinery (ACM) Genetic and Evolutionary Computation Conference (GECCO) and the Institute of Electrical and Electronics Engineers (IEEE) Congress on Evolutionary Computation (CEC). Documentation and code are available online &ndash; for GECCO Black-Box-Optimization-Benchmarking (BBOB) https://coco.gforge.inria.fr, and for CEC https://github.com/P-N-Suganthan/2020-Bound-Constrained-Opt-Benchmark.
    
3. *Artificial mixed representation problems*.

    Benchmark suites combining discrete and continuous variables include mixed-integer NK landscapes (Li *et al.*, 2006), mixed-binary and real encoded multi-objective problems (McClymont and Keedwell, 2011), mixed-integer problems based on the CEC functions (Liao *et al.*, 2014), and a mixed integer suite based on the BBOB functions (bbob-mixint) with a bi-objective formulation (bbobbiobj-mixint) (Tusar *et al.*, 2019).

4. *Black-box optimization problems*.

    For all benchmarks listed here, the problem formulation and the instances typically are publicly available, which inevitably leads to a specialization of algorithms to these. The Black-Box Optimization Competition (https://www.ini.rub.de/PEOPLE/glasmtbl/projects/bbcomp/) has attempted to address this with its single- and multi-objective, continuous optimization problems. Having said this, in 2019, the evaluation code has been made available.
    
5. *Constrained real-parameter problems*.

    Most real-parameter benchmark problems are unconstrained (except for basic bounds on variables) and there is a general lack of constrained benchmark sets for EC. Exceptions include a set of 18 artificial scalable problems for the CEC 2010 Competition on Constrained Real-Parameter Optimization (https://github.com/P-N-Suganthan/CEC2010-Constrained), six constrained real-parameter multi-objective real-world problems by Tanabe and Ishibuchi (2020) and the set of 57 real-world constrained problems (https://github.com/P-N-Suganthan/2020-RW-Constrained-Optimisation) for both the GECCO and CEC 2020 conferences.

6. *Dynamic single-objective optimization problems*.

    Benchmark problems for analysing algorithms in dynamic environments should ideally allow for the nature of the changes (such as severity and frequency) to be configurable. A useful resource on benchmarks for dynamic environments is the comprehensive review by Nguyen *et al.* (2012).
    
7. *Expensive optimization problems*.

    The GECCO 2020 Industrial Challenge provides a suite of discrete-valued electrostatic precipitator problems with expensive simulation-based evaluation (https://www.th-koeln.de/informatik-und-ingenieurwissenschaften/gecco-challenge-2020_72989.php). An alternative approach to benchmarking expensive optimization (used by CEC competitions) is to limit the number of allowed function evaluations for solving existing benchmark problems.
    
8. *Multimodal optimization (niching)*.

    Benchmark problem sets for niching include the GECCO and CEC competitions on niching methods for multimodal optimization problems (http://epitropakis.co.uk/gecco2020/) and the single-objective multi-niche competition problems (https://github.com/P-N-Suganthan/CEC2015-Niching).

9. *Noisy*.

    The original version of the Nevergrad platform (https://github.com/facebookresearch/nevergrad) had a strong focus on noisy problems, but the platform now also covers discrete, continuous, mixed-integer problems with and without constraints, with and without noise, explicitly modelled problems and true blackbox problems, etc. The electroencephalography (EEG) data optimization problem set of the CEC Optimization of Big Data 2015 Competition (http://www.husseinabbass.net/BigOpt.html) also includes noisy versions of the problem.

10. *Problems with interdependent components*.

    While much research tackles combinatorial optimization problems in isolation, many real-world problems are combinations of several sub-problems (Bonyadi *et al.*, 2019). The Travelling Thief Problem (Bonyadi *et al.*, 2013) has been created as an academic platform to systematically study the effect of the interdependence, and the 9 720 instances (https://cs.adelaide.edu.au/~optlog/research/combinatorial.php) vary in four dimensions. A number of single- and multi-objective as well as static and dynamic extensions of the Travelling Thief Problem have been proposed since then (Sachdeva *et al.*, 2020).

11. *Real-world discrete optimization*.

    The GECCO competition on the optimal camera placement problem (OCP) and the unicost set covering problem (USCP) include a set of discrete real-world problem instances (http://www.mage.fst.uha.fr/brevilliers/gecco-2020-ocp-uscp-competition/). Other real-world problems include the Mazda benchmark problem (http://ladse.eng.isas.jaxa.jp/benchmark/), which is a scalable, multi-objective, discrete-valued, constrained problem based on real-world car structure design, and a benchmark suite of combinatorial logic circuit design problems (de Souza *et al.*, 2020).

## References
* Mohammad Reza Bonyadi, Zbigniew Michalewicz, and Luigi Barone. The Travelling Thief Problem: The First Step in the Transition from Theoretical Problems to Realistic Problems. In 2013 *IEEE Congress on Evolutionary Computation*, pages 1037-1044. IEEE, 2013.
* Mohammad Reza Bonyadi, Zbigniew Michalewicz, Markus Wagner, and Frank Neumann. Evolutionary Computation for Multicomponent Problems: Opportunities and Future Directions. In *Optimization in Industry: Present Practices and Future Scopes*, pages 13-30. Springer, 2019. doi:10.1007/978-3-030-01641-8.
* Lucas Augusto Muller de Souza, Jose Eduardo Henriques da Silva, Luciano Jerez Chaves, and Heder Soares Bernardino. A benchmark suite for designing combinational logic circuits via metaheuristics. *Applied Soft Computing*, 91:106246, June 2020. doi:10.1016/j.asoc.2020.106246.  
* Carola Doerr, Furong Ye, Naama Horesh, Hao Wang, Ofer M. Shir, and Thomas Back. Benchmarking Discrete Optimization Heuristics with IOHprofiler. *Applied Soft Computing*, 88:106027, 2020.
* Stuart A. Kauffman. *The Origins of Order: Self-Organization and Selection in Evolution*. Oxford University Press, USA, 1993.
* Rui Li, Michael T. M. Emmerich, Jeroen Eggermont, Ernst G. P. Bovenkamp, Thomas Back, Jouke Dijkstra, and Johan H. C. Reiber. Mixed-Integer NK Landscapes. In *Proceedings of Parallel Problem Solving from Nature*, pages 42-51. Springer, 2006.
* Tianjun Liao, Krzysztof Socha, Marco A. Montes de Oca, Thomas Stutzle, and Marco Dorigo. Ant colony optimization for mixed-variable optimization problems. *IEEE Transactions on Evolutionary Computation*, 18(4):503-518, 2014.
* Kent McClymont and Ed Keedwell. Benchmark Multi-Objective Optimisation Test Problems with Mixed Encodings. In *Proceedings of the 2011 IEEE Congress on Evolutionary Computation*, pages 2131-2138. IEEE, 2011.
* Trung Thanh Nguyen, Shengxiang Yang, and Juergen Branke. Evolutionary dynamic optimization: A survey of the state of the art. *Swarm and Evolutionary Computation*, 6:1-24, October 2012. doi:10.1016/j.swevo.2012.05.001.
* Ragav Sachdeva, Frank Neumann, and Markus Wagner. The dynamic travelling thief problem: Benchmarks and performance of evolutionary algorithms, 2020.
* Ryoji Tanabe and Hisao Ishibuchi. An Easy-to-Use Real-World Multi-Objective Optimization Problem Suite. *Applied Soft Computing*, 89:106078, 2020.
* Tea Tusar, Dimo Brockhoff, and Nikolaus Hansen. Mixed-integer benchmark problems for single- and bi-objective optimization. In *Proceedings of the Genetic and Evolutionary Computation Conference*, pages 718-726. ACM, 2019.
* Thomas Weise and Zijun Wu. Difficult features of combinatorial optimization problems and the tunable W-model benchmark problem for simulating them. In *Proceedings of the Genetic and Evolutionary Computation Conference Companion*, GECCO '18, pages 1769-1776. ACM, 2018. ISBN 9781450357647.
