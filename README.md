# Hard_OT

This is the code for Hard negative sampling via optimal transport.

Some hyper-parameters to tune: 

--tau_plus: Positive class priorx. To reproduce the result in table 1, 2, 3. The best value are 0.1, 0.05 and 0.05 for stl10, cifar10 and cifar100.

--estimator: We only have one choice of estimator in this demo: "entropy_ot"

--dataset_name: "stl10", "cifar10", "cifar100".

--reg: $\epsilon$ in our paper
