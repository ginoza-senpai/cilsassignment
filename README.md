<h1>Iterated Local Search: Quadratic Assignment Problem</h1>

<i><h3>Shalin Shah</h3></i>
<a href="https://zenodo.org/badge/latestdoi/134310524"><img src="https://zenodo.org/badge/134310524.svg" alt="DOI"></a>

<p>
Implementation of iterative local search for the <a href="http://en.wikipedia.org/wiki/Quadratic_assignment_problem">quadratic assignment problem</a> (C++). The QAP is a
strongly NP-hard problem, and solving instances with more than 20 variables is considered intractable.
The implementation uses a population of individuals and performs local improvement on them.
Local improvement accepts worse solutions with a probability of 0.0. The parameters of the algorithm
can be adjusted by changing the global variables. The algorithm can be used to find approximate solutions
for large QAP instances for which exact methods are not suitable. (The code finds optimal solutions to <i>nug21</i>, <i>nug22</i> and <i>nug30</i> instances in a few seconds). The nug instances were first described in [1].
</p>
Instances are available at <a href="http://www.opt.math.tu-graz.ac.at/qaplib/">QAPLIB</a>. 
(The code includes a parser for the QAPLIB format).<br><br>
<p><b>Cite this code:</b>
<br>
<pre>
@misc{shah2014ilsqap,
  title={Implementation of iterative local search (ILS) for the quadratic assignment problem},
  author={Shah, Shalin},
  year={2014}
}
</pre>
<br>
<b>Usage:</b><br>
<pre>
- Compile the code using g++
- Run ./a.out filename iterations
- e.g. ./a.out instances/nug30.dat 10000
- Typical value for iterations is 10000
</pre>
<b>Results:</b><br>
Results on some instances (from the instances directory and at QAPLIB). The algorithm is quite fast and takes only a few seconds for 10000 iterations). The code is able to find optimum solutions for almost all instances (or at least a close to optimum solution)<br>
<table>
	<tr><td>Instance</td><td>Best Known Solution</td><td>This Algorithm's Solution</td></tr>
	<tr><td>nug12</td><td>578</td><td><b></b></td></tr>
  <tr><td>nug14</td><td>1014</td><td><b></b></td></tr>
  <tr><td>nug15</td><td>1150</td><td><b></b></td></tr>
  <tr><td>nug16a</td><td>1610</td><td><b></b></td></tr>
  <tr><td>nug16b</td><td>1240</td><td><b></b></td></tr>
  <tr><td>nug17</td><td>1732</td><td><b></b></td></tr>
  <tr><td>nug18</td><td>1930</td><td><b></b></td></tr>
  <tr><td>nug20</td><td>2570</td><td><b></b></td></tr>
  <tr><td>nug21</td><td>2438</td><td><b></b></td></tr>
  <tr><td>nug22</td><td>3596</td><td><b></b></td></tr>
  <tr><td>nug24</td><td>3488</td><td><b></b></td></tr>
  <tr><td>nug25</td><td>3744</td><td><b></b></td></tr>
  <tr><td>nug27</td><td>5234</td><td><b></b></td></tr>
  <tr><td>nug30</td><td>6124</td><td><b></b></td></tr>
</table><br>
<br><b>Cited By:</b><ul><li>Kanduc, T. “Optimisation of factory floor layout in a complex manufacturing process.” (2014).</li><li>Kanduc, T., and B. Rodic. "Optimisation of machine layout using a force generated graph algorithm and simulated annealing." International Journal of Simulation Modelling 15.2 (2016): 275-287.</li><li>Rodic, B., and T. Kanduc. "Optimisation of a complex manufacturing process using discrete event simulation and a novel heuristic algorithm." International Journal of Mathematical Models and Methods in Applied Sciences 9 (2015): 320-329.</li><li>Truetsch, Uwe. A semidefinite programming based branch-and-bound framework for the quadratic assignment problem. CentER, Tilburg University, 2014.</li><li>Manufacturing processes optimisation in a furniture factory (ITIS 2014)</ul></li><br>

<b>References</b>

[1] C.E. NUGENT, T.E. VOLLMAN, and J. RUML. An experimental comparison of techniques for the assignment of facilities to locations. Operations Research, 16:150-173, 1968.
