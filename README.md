# Hard_OT

This is the code for Hard negative sampling via optimal transport.

Use python main.py to train the model.

Some hyper-parameters to tune: 

--tau_plus: Positive class priorx. To reproduce the result in table 1, 2, 3. The best value are 0.1, 0.05 and 0.05 for stl10, cifar10 and cifar100.

--estimator: We only have one choice of estimator in this demo: "entropy_ot"

--dataset_name: "stl10", "cifar10", "cifar100".

--reg: $\epsilon$ in our paper, when $reg \leq 0$, the method is SimCLR (baseline). To reproduce the result in table 1, 2, 3. The best value are 0.3, 0.7 and 0.7 for stl10, cifar10 and cifar100.

--new_cost: To reproduce the result in Figure 4. True or False. If true: using new cost function proposed in our paper. If False: using default cost function.

--kappa: $\kappa$ in our paper. To reproduce the result in Figure 4, set new_cost = True, for "cifar100": $\epsilon = 0.7, \kappa = 1$, for "stl10": $\epsilon = 0.7, \kappa = 1$.
