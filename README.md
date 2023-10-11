***Behavioral study of two board classes of QKD protocol in density matrix simulation.***

This project had been developed to study the effect of noise over quantum key distribution protocols. Two primary classes of protocol viz. 

***1.Prepare and Measure Class***
***2.Entanglement Class*** 

had been observed.Under the prepare and measure class BB84 had been observed and under the second class Ekert 91 had been studied.
The noise model had been taken from the given noise dictionary in ***dm_simulator*** which is avaible at *https://github.com/indian-institute-of-science-qc/qiskit-aakash.git*.

In our implementation there are two jupyter notebooks which can be run over local installation provided the above mentioned simulator had already been installed in the system.User can define their own noise model using the above mentioned dictionary by passing noise parameters in the notebook promt.User can also stimulate the protocols in both noiseless and noisy enviornment in both presence and absence of sniffing.All he need is to pass proper command as and when appear by running cells.

In the case of BB84 QKD Protocol user will get both the secret-key-rate(essential parameter in information reconcillation phase) and ensembled probility distribution, but in the second case of Ekert 91 protocol user can only get ensemble probility distribution because to calculate the secret-key-rate one need result of individual classical bits which is difficult to get from resulted density matrix due to multiqubit nature of the protocol.

The same can be obtained using statevector simulation where result of individual classical bits can be obtained using **get_counts()** method which is not avaible in prior simulation.
