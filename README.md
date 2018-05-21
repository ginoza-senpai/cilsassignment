<h1>Iterated Local Search: Quadratic Assignment Problem</h1>
<hr noshade size="1">
<p>
Implementation of iterative local search for the <a href="http://en.wikipedia.org/wiki/Quadratic_assignment_problem">quadratic assignment problem</a>. The QAP is a
strongly NP-hard problem, and solving instances with more than 20 variables is considered intractable.
The implementation uses a population of individuals and performs local improvement on them.
Local improvement accepts worse solutions with a probability of 0.0. The parameters of the algorithm
can be adjusted by changing the global variables. The algorithm can be used to find approximate solutions
for large QAP instances for which exact methods are not suitable. (The code finds optimal solutions to all <i>nugXX</i> instances in a few seconds)
</p>
Instances are available at <a href="http://www.opt.math.tu-graz.ac.at/qaplib/">QAPLIB</a>. (The code includes a parser for the QAPLIB format).
