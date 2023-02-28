# UND TKET Workshop, March 2023

On behalf of [Quantinuum](https://www.quantinuum.com/), welcome to the UND TKET Workshop. It consists of two 1 hour 30 minute lectures. This workshop will explore tools available in [TKET](https://www.quantinuum.com/developers/tket), providing a comprehensive, feature-focused tour of the platform.

[TKET](https://www.quantinuum.com/developers/tket) is the leading open-source developer toolkit designed to compile and optimize quantum programs. It is platform inclusive allowing it to target the world’s leading quantum hardware, simulators, and quantum computing SDKs like Qiskit. It also enhances the performance of every Quantinuum product, including cybersecurity key-generation platform Quantum Origin, quantum computational chemistry and materials science package InQuanto, and lambeq, Quantinuum's quantum natural language processing and computational linguistics toolkit. 

## Installation
First, make sure that a recent version of Python is installed on your machine. You can check this in a terminal:

`python --version`

I would recommend using either Python 3.10 or Python 3.11.

To run the Jupyter notebooks, refer to the following: https://jupyter.org/. In case you don't have access to Python or a Jupyter Notebook yet, I suggest you install Anaconda: https://www.anaconda.com/products/distribution

There is currently an implementation of TKET available in the form of the `pytket` python package that is installed by running 

`pip install pytket`

Additional extension modules are available for interfacing pytket with several quantum software packages, including: Qiskit, Cirq, PennyLane, pyQuil, and others. For this workshop, also install the Qiskit extension:

`pip install pytket-qiskit` 

Documentation and examples are available → https://github.com/CQCL/pytket-extensions.

## Useful Links

- [Pytket User manual](https://cqcl.github.io/pytket/manual/index.html)
- [Pytket API docs](https://cqcl.github.io/tket/pytket/api/)
- [Pytket Notebook Examples](https://github.com/CQCL/pytket/tree/main/examples)

## Workshop Contents

### Part 1 (1.5 hours): Quantum circuit construction and running on classical backends
A quantum circuit forms the unit of computation that we can send off to a quantum co-processor: there is the main program running on the classical host computer, which routinely sends off jobs to a quantum computer. We will use Quantinuum’s quantum software development kit called TKET to discuss basic quantum gates, build quantum circuits and perform measurements. Moreover, when working with quantum circuits, we may want access to the quantum state prepared by our circuit. This can be helpful if we want to check whether our circuit construction is correct. We will use different classical simulators, such as a statevector simulator and a simulator that mimics a perfect quantum computer. 

### Part 2 (1.5 hours): The Quantum compiler flow
In part 1, we have covered enough to be able to design the quantum circuits we want to run, submit them to a simulator backend, and interpret the results in a meaningful way. This is all we need to run a quantum computation and observe some basic results. If you want to run your circuit on a real quantum processor, we need to consider the necessary steps for circuit compilation. In this part of the workshop, we will explore the quantum compiler toolchain. The primary goals of compilation are two-fold: solving the backend constraints to get from the abstract model to something runnable, and optimizing/simplifying the circuit to make it faster, smaller, and less prone to noise.

In order to run a circuit on one of IBM's free superconducting devices, you will need to setup a free IBM Q account: 
https://quantum-computing.ibm.com/composer/docs/iqx/manage/account/


## Survey
Throughout the TKET workshop, you will be able to gain a lot of hands-on experience with TKET. It would be very helpful for us to know what you found particularly difficult. The installation, the interface, the documentation or did you even find a bug? How did you find the covered material (underwhelming, overwhelming, just right), and what suggestions do you have for improvement? Please let us know by filling out this short survey that will take about 5 minutes to complete:
https://forms.office.com/r/b8N2XK20xf

## Contact

If any questions arise, don't hesitate to contact me via email
[kathrin.spendier@quantinuum.com](mailto:kathrin.spendier@quantinuum.com). 

There is a public TKET slack channel for community discussion and support. Click [here](https://tketusers.slack.com/join/shared_invite/zt-18qmsamj9-UqQFVdkRzxnXCcKtcarLRA#/shared-invite/email) to join. 

You can also join our [mailing list](https://list.cambridgequantum.com/cgi-bin/mailman/listinfo/tket-users) for updates on new pytket releases and features. If you have TKET support questions please send them to [tket-support@cambridgequantum.com](mailto:tket-support@cambridgequantum.com).
