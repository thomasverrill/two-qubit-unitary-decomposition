# two-qubit-unitary-decomposition
This code implements both B-gate and SQiSW-based methods of 2-Qubit quantum gate decomposition. The decomposition methods are from these two papers: Quantum Instruction Set Design for Performance (https://arxiv.org/pdf/2105.06074.pdf) and Minimum construction of two-qubit quantum operations (https://arxiv.org/pdf/quant-ph/0312193.pdf). This was created for the final project in the Princeton ECE396 "Introduction to Quantum Computing Class). 

Due to bugs in the algorithm given in the SQiSW paper, cases where three SQiSW gates are needed do not work as intended. Additionally, in the case where a CNOT is given as the unitary to decompose with SQiSW gates, it does not work as intended. These issues have been resolved in the Qiskit-Terra GitHub repository, where the SQiSW method has been modified to work for all cases.

As of 1/25/23, the working methods implemented with this code have been contributed to the Qiskit-Terra GitHub repository. The SQiSW and B gates have also been contributed to the Qiskit gate library. See https://github.com/Qiskit/qiskit-terra/issues/9333 for the current progress on this implementation. 
