This week we mainly covered an intro to Quantum Computing, a good deal of Linear Algebra and some Quantum Mechanics as well.

I first read about what quantum computation actually is - just a brief introduction. We discussed qubits and different logical gates that could change the state of a qubit. The gates are just unitary transformations on the state space of the qubit in question. We then looked at multiple qubits and how qubits in Bell states were entangled with each other - measuring one qubit enables you to predict the result of a following measurement of the other qubit with 100% accuracy - the reason being very simple - both of |i j1 > and |i j2 > for any i & j1 != j2 are not present in any Bell state - so in a Bell state, knowing i, we can exactly tell what j is (of course, we must know which Bell state the qubits were in).

We then looked at a controlled gate - the CNOT gate, and saw how three of these could allow us to swap the states of two qubits.
We saw an interesting example of quantum teleportation - where using just a bit of classical communication to convey the result of measurement, a quantum state (some information) could be "teleported" to someone else arbitrarily far away using a pair of qubits in a Bell state.

We also saw the Toffoli gate that can, among other things, simulate a NAND gate and FANOUT, and so we can simulate an arbitrary classical circuit with a quantum circuit. Finally, we looked at Quantum Parallelism and the Deutsch-Josza algorithm - that can confirm with one unitary matrix application - whether a function on n bits is balanced or not.

Linear Algebra:

We shine new light on Linear Algebra - we study it from the perspective of co-ordinate independent vectors in a vector space, and linear operators. The linear operators can be represented as matrices given an input basis and an output basis. The most wow thing for me in the start of this section is that the identity transform needn't look like the identity matrix when the input and output bases are different.

We then covered usual linear algebra - Bases, Inner products & Gram-Schmidt, Outer products and the very useful completeness relation.
Outer products are hands-down one of the coolest things I've seen so far - they are a really neat way to represent linear operators, it's amazing.

We then see some definitions - the adjoint of an operator, Hermitian, Unitary and Normal operators.
We meet the Spectral Theorem - normal operators are the same as unitarily diagonalizable operators! - and simultaneous diagonalizability for commuting operators - they have a common eigenbasis!

We move to tensor products - the Kronecker Product is a really neat way to explain the effect of an operator on a tensor product space V tensor W, I thoroughly enjoyed proving that the Kronecker Product is indded the representation of a linear operator on V tensor W for pre-specified bases of V and W. (I didn't quite get how the inner product for a tensor space is defined, though).

Then we explored what is one of my favourites in Linear Algebra now - operator functions. It truly is a wonderful and neat definition. I had a lot of fun connecting this definition to the definitions of square roots and exponentials for matrices that I had seen before.
We also looked at the commutator and anti-commutator of a pair of matrices.

Finally, we looked at two decompositions of general matrices - the Polar Decomposition, and the SVD. I understood these from a proof standpoint, but I guess I'll need to think and learn more on these to gain the understanding of the decompositions from a geometric point of view.

Quantum Mechanics:

We formalized the axioms of QM in the language of linear operators - similar to PH107, but more formally. The measurement axiom was particularly striking - it was more general than the usual axiom about orthonormal eigenstates, but I didn't get why the more general axiom was required. Perhaps I'll see an example after a bit :)

I also learnt that the Schrodinger Equation for discrete times could be elegantly rephrased as: the state vector evolves according to a Unitary time-dependent transformation - this was really cool.

That's all for week 1, Thank you! :)
