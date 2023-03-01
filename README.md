# UND TKET Workshop, March 2023

On behalf of [Quantinuum](https://www.quantinuum.com/), welcome to the UND TKET Workshop. This workshop will explore tools available in [TKET](https://www.quantinuum.com/developers/tket), providing a comprehensive, feature-focused platform tour. It consists of two 1 hour 30-minute lectures.

[TKET](https://www.quantinuum.com/developers/tket) is one of the leading open-source quantum software development toolkits (SDKs) designed to compile and optimize quantum programs. It is platform inclusive, allowing it to target the world’s leading quantum hardware, simulators, and other quantum SDKs like Qiskit and PennyLane. It also enhances the performance of other Quantinuum products, such as the quantum computational chemistry and materials science package InQuanto and lambeq, Quantinuum's quantum natural language processing and computational linguistics toolkit. 

## Please complete prior to the workshop:

### 1) Installation
In this workshop we will use Jupyter notebooks. To run the Jupyter notebooks, refer to the following: https://jupyter.org/. You can follow options a), b), or c) below to run the notebooks:

#### a) If you don't want to install anything on your computer just click on "launch Binder" (Open in a new tab) to run all the notebooks in a browser: [launch Binder](https://mybinder.org/v2/gh/spendierk/UND-TKET-Workshop-2023/main)
 1. Wait for the Binder environment to launch (this may take a few minutes).
 2. Once the environment is ready, you should see a Jupyter notebook interface.
 3. Click on the script "TEST_Binder.ipynb" to open it in a new tab.
 4. Run each script cell by clicking on the "Run" button or using the keyboard shortcut "Shift + Enter".

Note that Binder links are temporary and will expire after a period of inactivity, so you'll need to generate a new link each time you want to launch the environment.

#### b) In case you want to run the Jupyter notebooks on your computer,
I suggest you install Anaconda: https://www.anaconda.com/products/distribution. Once installed, open and run the [TEST_your_environment.ipynb](https://github.com/spendierk/UND-TKET-Workshop-2023/blob/main/TEST_your_environment.ipynb) Jupyter notebook to make sure you are set for the workshop.

#### c) In case you have Python already installed on your machine,
You should check your current Python version in a terminal by typing
`python --version`
I would recommend using either Python 3.9 or Python 3.10. Run the [TEST_your_environment.ipynb](https://github.com/spendierk/UND-TKET-Workshop-2023/blob/main/TEST_your_environment.ipynb) Jupyter notebook to make sure you are set for the workshop.

### 2) Sign up for an IBM Quantum account
You can sign up to get free access to some of IBM's superconducting devices to run a quantum circuit on a real quantum computer. To do this, you will need to set up a free IBM Q account: 
https://quantum-computing.ibm.com/composer/docs/iqx/manage/account/

### 3) Read this [Short introduction to Quantum Computing](https://www.kattemolle.com/KattemolleShortIntroToQC.pdf)
These notes offer physicists a brief introduction to quantum computation. The reading time is about two hours if you also do the small exercises. This should give
you a good but basic understanding of the notation and the most important concepts.

### 4) If you have time:
Have a look at the [PyTKET User manual](https://cqcl.github.io/pytket/manual/index.html). Further references that may be useful after the workshop if you want to explore more about TKET:
- [Pytket API docs](https://cqcl.github.io/tket/pytket/api/)
- [Pytket Notebook Examples](https://github.com/CQCL/pytket/tree/main/examples)


## Workshop Contents (notebooks will be available the day of the workshop here)

### Part 1 (1.5 hours): Quantum circuit construction and running on classical backends
A quantum circuit forms the unit of computation that we can send off to a quantum co-processor: there is the main program running on the classical host computer, which routinely sends off jobs to a quantum computer. We will use Quantinuum’s quantum software development kit called TKET to discuss basic quantum gates, build quantum circuits and perform measurements. Moreover, when working with quantum circuits, we may want access to the quantum state prepared by our circuit. This can be helpful if we want to check whether our circuit construction is correct. We will use different classical simulators, such as a statevector simulator and a simulator that mimics a perfect quantum computer. 

### Part 2 (1.5 hours): The Quantum compiler flow
In part 1, we have covered enough to be able to design the quantum circuits we want to run, submit them to a simulator backend, and interpret the results in a meaningful way. This is all we need to run a quantum computation and observe some basic results. If you want to run your circuit on a real quantum processor, we need to consider the necessary steps for circuit compilation. In this part of the workshop, we will explore the quantum compiler toolchain. The primary goals of compilation are two-fold: solving the backend constraints to get from the abstract model to something runnable, and optimizing/simplifying the circuit to make it faster, smaller, and less prone to noise.


## Survey (after the workshop)
Throughout the TKET workshop, you will be able to gain a lot of hands-on experience with TKET. It would be very helpful for us to know what you found particularly difficult. The installation, the interface, the documentation or did you even find a bug? How did you find the covered material (underwhelming, overwhelming, just right), and what suggestions do you have for improvement? Please let us know by filling out this short survey that will take about 5 minutes to complete:
https://forms.office.com/r/b8N2XK20xf

## Contact
If any questions arise, don't hesitate to contact me via email
[kathrin.spendier@quantinuum.com](mailto:kathrin.spendier@quantinuum.com). 

There is a public TKET slack channel for community discussion and support. Click [here](https://tketusers.slack.com/join/shared_invite/zt-18qmsamj9-UqQFVdkRzxnXCcKtcarLRA#/shared-invite/email) to join. 

You can also join our [mailing list](https://list.cambridgequantum.com/cgi-bin/mailman/listinfo/tket-users) for updates on new pytket releases and features. If you have TKET support questions please send them to [tket-support@cambridgequantum.com](mailto:tket-support@cambridgequantum.com).
