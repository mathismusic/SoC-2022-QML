# Week 2
This week, we explored quantum circuits - what we can do with them, and how to implement them using a small existing set of gates.

First, we looked at single-qubit gates. The rotation matrices $R_x(\theta), R_y(\theta), R_z(\theta)$ constructed in terms of the Pauli matrices $X$, $Y$ and $Z$ together with a $Z-Y$ decomposition of a general unitary help us prove my favorite result(its usage in controlled multiple qubit gate construction was just really nice) of this week of all this week - Any unitary can be written as $e^{\iota \alpha}AXBXC$ with $ABC = I$.

Onward to controlled multiple qubit gates. Using the controlled-$X$ gate and single qubit unitaries, we can implement a general controlled-$U$ gate. Here's my favourite result from this week: a controlled-$U$ gate may be implemented directly and simply if we know its decomposition into a phase times $AXBXC$ for unitaries $A$, $B$, $C$ whose product is $I$. This relies on the simple but crucial point that $A \cdot X \cdot B \cdot X \cdot C$ is $U$, but $A \cdot I \cdot B \cdot I \cdot C$ is $I$.

We then move on to 2-control 1-target gates or $C^2(U)$ gates. The $V^2 = U$(as I like to call it) or Sleator-Weinfurter construction specifies the exact circuit to build a general $C2(U)$ gate. It is an ingenious idea, utilizing $V \cdot V = U$, but $V^* \cdot V = I$. We also discuss the construction of the ubiquitous Toffoli( $C^2(X)$ ) gate.

Then we briefly discuss $C^n(U)$ gates - $n$-control 1-target gates. They are most simply implemented using ancilla qubits, but can be constructed using the $V^2 = U$ idea - this time, the $V$ gates are $C^{n-1}(V \text{ or } V^*)$ gates. Turns out(I am yet to show this) a $C^n(X)$ gate can be implemented exclusively using $O(n^2)$ Toffoli, controlled-$X$ and single qubit unitaries from which, using the ubiquitous $U = e^{\iota \alpha}AXBXC$ a general $C^n(U)$ gate is eaily constructed.

We then discuss measurement: Deferred measurement can be done, since "no information is lost" till measurement and so the measurement can be done at the end with the same results. We check this using the Quantum Teleportation circuit. Another principle called the Principle of Implicit Measurement says that all unmeasured qubits at the end of a circuit may be assumed to be measured.

Finally, we discuss univerality - a small set of gates can be used to approximate any gate to arbitrary precision.
Any unitary can be wriiten as a product of two-level gates, any two-level gate can be built from controlled-$X$ and single qubit gates. This construction requires a huge number of gates(exponential in the number of qubits) ans so we try to approximate gates to required accuracies instead. Here we make use of $\pi/8$ and Hadamard gates. The number of gates required when using these gates to approximate single qubit gates is much lower and can be implemented.

We then moved to the Coding exercises. I was first introducet to Jupyter Notebooks and the Qiskit Library. I then implemented the problems as required. It was real fun seeing the algos in action. I have some ideas for the optional ones, will do them as and when I get time.

That's it for Week 2, Thank you for reading!
