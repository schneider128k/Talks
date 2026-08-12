# Talks and posters

Newest first. Each entry gives the occasion and date, names the people the work was done with,
and links to the slides or the poster and the sources they were built from.

Entries are being added one at a time. The recovery itself is finished; the publishing is not,
and the talks I gave after 2020 are not yet reconstructed.

---

## University of Central Florida

- **Efficient Quantum Algorithm for Identifying Hidden Polynomial Function Graphs** —
  *Seminar*, May 2007  
  Institute for Quantum Information (IQI), California Institute of Technology, Pasadena. The
  visit was arranged with Ann Harvey; I sent her the title and abstract on 11 May and flew
  into Los Angeles on the evening of Monday 21 May. The day of the seminar itself is not
  recorded anywhere I have.  
  Joint work with Thomas Decker and Jan Draisma.  
  The Hidden Polynomial Function Graph Problem: an abelian hidden subgroup problem is the
  case where the hidden object is the graph of a *linear* function over a finite field, and
  the generalization lets the function be a polynomial of higher degree. Classically the
  black-box query complexity stays polynomial in the field size; quantum mechanically the
  problem reduces to identifying a quantum state, and the query complexity stops depending on
  the field size altogether. For univariate polynomials the talk builds the von Neumann
  measurement that distinguishes those states, and gets the efficient algorithm by bounding
  its success probability below by a constant — the bound coming from algebraic geometry, via
  properties of generic morphisms between affine spaces.  
  The talk predates the paper: it was given in May 2007, and
  [arXiv:0706.1219](https://arxiv.org/abs/0706.1219) went up the following month.  
  I gave versions of this talk repeatedly through 2007 — in Sydney in May, in Warsaw at the
  end of July, and in Princeton in October.  
  These are the slides as I finished them in Pasadena, sent to myself under the subject
  *Final talk* on 22 May. They are one revision later than the copy that survives in my own
  files, which stops at 21 May and carries a wrong normalization in three of the
  density-matrix expressions.  
  [presentation](documents/2007-05_hidden_polynomial_graphs_caltech/hidden_polynomial_graphs_caltech_presentation.pdf) ·
  [abstract](documents/2007-05_hidden_polynomial_graphs_caltech/hidden_polynomial_graphs_caltech_abstract.txt) ·
  [sources](documents/2007-05_hidden_polynomial_graphs_caltech/)

- **Weak Fourier-Schur Sampling, the Hidden Subgroup Problem and the Quantum Collision
  Problem** — *Conference talk*, February 2007  
  STACS 2007, the 24th International Symposium on Theoretical Aspects of Computer Science,
  RWTH Aachen. I travelled to Aachen on 21 February and came back on the evening of the 24th.  
  Joint work with Andrew Childs and Aram Harrow.  
  Weak Fourier sampling measures only the name of the irreducible representation and throws
  the rest away; weak Schur sampling does the same for the partition under Schur duality. The
  talk shows what that costs. The distribution produced by weak Schur sampling depends only
  on the spectrum of the state, which lets the question be turned into a quantum collision
  problem and answered with a careful analysis of the Schur distribution and the typical
  shape of partitions under Plancherel measure. The conclusion is negative and sharp: weak
  Fourier-Schur sampling cannot distinguish a hidden reflection in the dihedral group, nor an
  order-two subgroup of the symmetric group, without exponentially many copies.  
  Along the way it gives the first results on estimating the spectrum of a quantum state in
  the regime where the number of copies is much smaller than the square of the dimension.  
  The talk is built on
  [quant-ph/0609110](https://arxiv.org/abs/quant-ph/0609110).  
  [presentation](documents/2007-02_weak_fourier_schur_sampling_stacs/weak_fourier_schur_sampling_stacs_presentation.pdf) ·
  [sources](documents/2007-02_weak_fourier_schur_sampling_stacs/)

## Institute for Quantum Information, Caltech — and the move to Florida

- **The Jones Polynomial: Quantum Algorithms and Applications in Quantum Complexity
  Theory** — *Invited talk*, November 2006  
  Seminar Combinatorial Theory at the Euler Institute for Discrete Mathematics and its
  Applications, Technische Universiteit Eindhoven, at the invitation of Prof. Arjeh Cohen.  
  Joint work with Jon Yard.  
  An earlier version of the same talk was given in February 2006 to the Topology Seminar of
  the Department of Mathematics at the University of California, Santa Barbara, at the
  invitation of Stephen Bigelow, under the title *Quantum algorithms, quantum complexity
  theory and their connection to the Jones polynomial*. The slides here are the Eindhoven
  ones; the abstract beside them is the one written for Santa Barbara.  
  Links as closures of braids, the Jones polynomial at roots of unity, and the unitary
  Jones-Wenzl representations of the braid group, with the Birman moves and the
  representation-theoretic formula that follows from them; then quantum computation read as
  the approximate evaluation of the Jones polynomial. The contribution is a direct proof
  that approximating the Jones polynomial of plat closures at roots of unity is
  BQP-complete — encoding a qubit in four strands rather than going through topological
  quantum computation — together with a braid problem complete for Quantum-NP.  
  The talk is built on [quant-ph/0603069](https://arxiv.org/abs/quant-ph/0603069).  
  [presentation](documents/2006-11_jones_polynomial_eindhoven/jones_polynomial_eindhoven_presentation.pdf) ·
  [abstract](documents/2006-11_jones_polynomial_eindhoven/jones_polynomial_abstract_santa_barbara.txt) ·
  [sources](documents/2006-11_jones_polynomial_eindhoven/)

- **On the Quantum Hardness of Solving Isomorphism Problems as Nonabelian Hidden Shift
  Problems** — *Seminar*, October 2005  
  Institute for Quantum Information (IQI), California Institute of Technology, Pasadena.  
  Joint work with Andrew Childs.  
  Graph isomorphism, and isomorphism of rigid graphs, recast as hidden shift problems over
  nonabelian groups — and the evidence that the recasting does not make them easy. Measuring
  a single register does not suffice: the distribution it produces with the shift and the
  one without it are exponentially close in total variation, so any algorithm along these
  lines has to make entangled measurements across many copies.  
  The talk is built on [quant-ph/0510185](https://arxiv.org/abs/quant-ph/0510185).  
  No mail from the Caltech years survives, so the month is that of the finished slides
  rather than of the seminar itself.  
  [presentation](documents/2005-10_nonabelian_hidden_shift_caltech/nonabelian_hidden_shift_caltech_presentation.pdf) ·
  [sources](documents/2005-10_nonabelian_hidden_shift_caltech/)

## Promotion — Universität Karlsruhe (TH), doctoral work at the IAKS

- **Estimating mixing properties of local Hamiltonian dynamics and continuous quantum random
  walks is PSPACE-hard** — *Invited talk*, 3 February 2004  
  Universität Innsbruck, at the invitation of Prof. Dr. Hans Briegel.  
  The results of the dissertation, turned around to give hardness rather than efficiency: a
  hypothetical apparatus measuring arbitrary 4-local observables on *n* qubits would solve
  PSPACE problems probabilistically, and estimating the entropy of the time-average of
  computational basis states under 4-local Hamiltonians and quantum random walks is
  PSPACE-hard.  
  I gave the same talk twice more the following month, on a trip through England: at the
  University of Bristol on 17 March 2004, at Richard Jozsa's invitation, under the title
  *Measuring 4-local n-qubit observables could probabilistically solve PSPACE*; and at
  Imperial College London, arranged with Martin Plenio for the same trip.  
  The talk is built on [quant-ph/0308011](https://arxiv.org/abs/quant-ph/0308011).  
  [presentation](documents/2004-02_mixing_properties_pspace/mixing_properties_pspace_presentation.pdf) ·
  [abstract](documents/2004-02_mixing_properties_pspace/mixing_properties_pspace_abstract.pdf) ·
  [sources](documents/2004-02_mixing_properties_pspace/)

- **Computational Power of Hamiltonians in Quantum Computing** — *Invited talk*, September 2003  
  Fondazione Istituto per l'Interscambio Scientifico (ISI), Turin, at the invitation of
  Prof. Mario Rasetti. I was in Turin from 22 to 25 September.  
  The main results of the dissertation, shown to Rasetti shortly before he examined them: he was
  the Korreferent, the second reviewer, and the oral examination followed on 17 November 2003
  under this same title.  
  The control-theoretic model and the definition of mutual simulation of Hamiltonians; lower
  bounds from the majorization and rank criteria; the complexity of time reversal; selective
  decoupling by chromatic index; the construction of planar orthogonal Hamiltonians whose ground
  states encode maximum independent sets; and the new complete problems for QMA and QCMA.  
  [presentation](documents/2003-09_computational_power_turin/computational_power_turin_presentation.pdf) ·
  [abstract](documents/2003-09_computational_power_turin/computational_power_turin_abstract.txt) ·
  [sources](documents/2003-09_computational_power_turin/)

- **Mutual simulation of Hamiltonian dynamics on interacting quantum systems** — *Seminar*, 1 April 2003  
  Institute for Quantum Information (IQI), California Institute of Technology, Pasadena, at
  the invitation of Prof. John Preskill. I stayed three weeks.  
  Joint work with Dominik Janzing, Martin Rötteler and Thomas Beth.  
  The Karlsruhe Hamiltonian-simulation work in its settled form: the control-theoretic model,
  simulation as a convex sum of local conjugates, decoupling schemes, and the bounds read off
  the interaction graph — with the harder direction added, that determining the ground-state
  energy for cubic planar interaction graphs is NP-complete.  
  [presentation](documents/2003-04_mutual_simulation_caltech/mutual_simulation_caltech_presentation.pdf) ·
  [abstract](documents/2003-04_mutual_simulation_caltech/mutual_simulation_caltech_abstract.txt) ·
  [sources](documents/2003-04_mutual_simulation_caltech/)

- **Computational Power of Hamiltonians in Quantum Computing** — *Professorenrunde*, February 2003  
  Universität Karlsruhe (TH), Fakultät für Informatik. Before the doctoral procedure was formally
  opened I wrote to the professors of the faculty, offering to discuss the results of the thesis;
  these are the slides I prepared for that round. The examination itself followed on
  17 November 2003, under this same title.  
  The Karlsruhe Hamiltonian-simulation work put to a general audience: average Hamiltonian
  theory and the fast control limit, simulation as a convex sum of local conjugates, decoupling
  by error bases and orthogonal arrays, and the bounds on the time overhead read off the
  interaction graph — with time reversal and the separability problem as the applications.  
  [presentation](documents/2003-02_computational_power_karlsruhe/computational_power_karlsruhe_presentation.pdf) ·
  [sources](documents/2003-02_computational_power_karlsruhe/)

- **Complexity of Mutual Simulation of Hamiltonian Dynamics** — *Invited talk*, 12 July 2002  
  Ludwig-Maximilians-Universität München, at the invitation of Robert Raussendorf.  
  Joint work with Dominik Janzing, Martin Rötteler and Thomas Beth.  
  Much the same talk as the one in Bad Honnef six months earlier, but with new material on
  the mathematics it rests on: vector and operator majorization, and Uhlmann's theorem.
  Those two slides are the earliest record I have of my working with majorization, which
  came back many years later in my work on spectral graph theory, so they are also set
  here on their own.  
  The abstract was written in German, under the title *Simulation hamiltonscher Dynamiken
  auf wechselwirkenden Quantensystemen*.  
  [presentation](documents/2002-07_complexity_of_mutual_simulation/complexity_of_mutual_simulation_presentation.pdf) ·
  [abstract](documents/2002-07_complexity_of_mutual_simulation/complexity_of_mutual_simulation_abstract.pdf) ·
  [sources](documents/2002-07_complexity_of_mutual_simulation/)

- **Mutual Simulation of Hamiltonian Dynamics on Interacting Quantum Systems** — *Colloquium*, January 2002  
  Colloquium *Quantum Information Processing* of the Deutsche Forschungsgemeinschaft, at the
  [Physikzentrum Bad Honnef](https://www.dpg-physik.de/ueber-uns/physikzentrum-bad-honnef).  
  Joint work with Dominik Janzing, Martin Rötteler and Thomas Beth.  
  Simulating one Hamiltonian with another on *n* interacting quantum systems: the
  control-theoretic model and average Hamiltonian theory, decoupling schemes built from
  orthogonal arrays and error bases, and bounds on the time overhead read off the
  interaction graph — its chromatic index, and the spectrum of its adjacency matrix.  
  [presentation](documents/2002-01_mutual_simulation_of_hamiltonians/mutual_simulation_of_hamiltonians_presentation.pdf) ·
  [sources](documents/2002-01_mutual_simulation_of_hamiltonians/)

- **Simulating Hamiltonians in Quantum Networks: Efficient Schemes and Complexity Bounds** — *Poster*, January 2002  
  QIP 2002, the Fifth Workshop on Quantum Information Processing, IBM T.J. Watson Research
  Center, Yorktown Heights, 14–17 January 2002.  
  Joint work with Martin Rötteler, Dominik Janzing and Thomas Beth.  
  The same poster as the one for the Turin project meeting below, listed here under the title of
  the paper it was built around.  
  [poster](documents/2001-10_multiparticle_hamiltonians/multiparticle_hamiltonians_poster.pdf)

- **Universal Simulation of Multiparticle Hamiltonians: Efficient Schemes and Complexity Bounds** — *Poster*, October 2001  
  Project meeting in Turin, under the European project Q-ACTA
  ([IST-1999-10596](https://cordis.europa.eu/project/id/IST-1999-10596)). The project had two
  partners: Karlsruhe, which coordinated it, and the Fondazione Istituto per l'Interscambio
  Scientifico in Turin.  
  Joint work with Martin Rötteler, Dominik Janzing and Thomas Beth.  
  The Karlsruhe Hamiltonian-simulation work on a single A1 sheet: decoupling and time
  reversal in quantum networks, schemes built from orthogonal arrays and error bases, and
  bounds on the simulation overhead taken from the spectrum and the chromatic index of the
  interaction graph.  
  What I have is the PostScript it was printed from.  
  [poster](documents/2001-10_multiparticle_hamiltonians/multiparticle_hamiltonians_poster.pdf) ·
  [sources](documents/2001-10_multiparticle_hamiltonians/)

- **Simulating Arbitrary Pair-Interactions by a Given Hamiltonian: Graph-Theoretical Bounds
  on the Time Complexity** — *Poster*, July 2001  
  Quantum Information: Theory, Experiment and Perspectives, Gdańsk, 10–18 July 2001.  
  Joint work with Dominik Janzing and Thomas Beth.  
  An earlier state of the poster above, listed here under the title of the paper it was built
  around. The October version is the one I have.  
  [poster](documents/2001-10_multiparticle_hamiltonians/multiparticle_hamiltonians_poster.pdf)

- **Performances of Binary Block Codes Used on Classical-Quantum Channels** — *Poster*, July 2000  
  QCMC 5, the Fifth International Conference on Quantum Communication, Measurement and
  Computing, Capri, 3–8 July 2000.  
  Joint work with Dejan E. Lazić and Thomas Beth. The seven sheets carry no title page, so
  the authorship is recorded only here.  
  Lower bounds on the error exponent of binary block codes used on classical-quantum
  channels: rescaled binomial multiplicity enumerators, Holevo's suboptimal decision rule,
  and the expurgated and cutoff rate bounds. The accompanying paper is in the conference
  proceedings, pp. 43–46.  
  [poster](documents/2000-07_binary_block_codes/binary_block_codes_poster.pdf) ·
  [sources](documents/2000-07_binary_block_codes/)

