.. _section_new_feature:

=====================================================
New feature
=====================================================

.. contents::
   :depth: 2
   :local:

Rough notes
=====================================================
* Content about new feature.

equation :math:`x = x + 1`


Algebra
============================================================================
A set :math:`\mathcal{A}` formed from another set :math:`S`, according 3 rules:

   * :math:`S \in \mathcal{A}`
   * If :math:`X \in \mathcal{A}`, then :math:`X^c \in \mathcal{A}`
   * If :math:`X \in \mathcal{A}` and :math:`Y \in \mathcal{A}`, then :math:`X \cup Y \in \mathcal{A}`


Implications of rules:

   * Empty set is always in :math:`\mathcal{A}`, because the empty set is the complement of :math:`S`.
   * The union of all pairs of sets in :math:`S` must be in :math:`\mathcal{A}`.
   * The intersections of sets is included in :math:`\mathcal{A}`.
   * The relative differences of sets is also included in :math:`\mathcal{A}`.



Sigma Algebra
============================================================================
A sigma algebra is a type of algebra, the follows the first two rules of an algebra, but expands rule 3 require that the union of any sequence of sets in :math:`\mathcal{A}` must also be in :math:`\mathcal{A}`:

* If :math:`\{A_n: n \in N \}` is a sequence of sets in :math:`\mathcal{A}`, then :math:`\bigcup_{n} A_n \in \mathcal{A}`.

Given a domain :math:`S`, and a set :math:`C` of subsets of :math:`S` that you want to measure, you generate a sigma algebra :math:`\mathcal{A} = \sigma(C)`.

For example, if :math:`C = { A, B }`, you form a sigma algebra :math:`\mathcal{A} = \sigma( A, B)`. You get the sigma algebra with the fewest elements that also contains the set :math:`C`.


Probability space
============================================================================
A probability space is a formal model of a random process or experiment. A probability space is a measure space: :math:`(\Omega, \mathcal{F}, P)`, where the measure of :math:`\Omega = 1`:


#. **Sample space**: :math:`\Omega` is a set of all possible outcomes of the experiment.
#. **Event space**: Sigma algebra :math:`\mathcal(F)` is a set of events, where an event is a subset of events in :math:`\Omega`.
#. **Probability measure**: A set function that assigns each event in :math:`\mathcal{F}` a number between 0 and 1.

These three elements must satisfy the Andrey Kolmogorov's three axioms of probability.


Reference: `Probability space <https://en.wikipedia.org/wiki/Probability_space>`_
