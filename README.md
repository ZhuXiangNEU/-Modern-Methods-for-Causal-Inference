# Effect of Treatments on Glottic Cancer


##### 1. Specify a Causal Model.

Endogenous nodes: $X = (W_1, W_2, W_3, W_4, Y)$
W1: denotes sex (male or female).
W2: denotes age in years
W3: denotes race (White/Black/Others)
W4: denotes American Joint Committee on Cancer staging classification system. It denotes a specific tumor stage of a patient.
A: indicates the radiation/surgery treatment status
Y: indicates surviving status at endpoint


Exogenous nodes: $U = (U_{W_1}, U_{W_2}, U_{W_3}, U_{W_4}, U_{A}, U_{Y}) ∼ P^*$
Structural equations F:
$$W_1 \gets f_{W_1}(U_{W_1})$$
$$W_2 \gets f_{W_2}(U_{W_2})$$
$$W_3 \gets f_{W_3}(U_{W_3})$$
$$W_4 \gets f_{W_4}(W_1, W_2, W_3, U_{W_3})$$
$$A \gets f_{A}(W_1, W_2, W_3, W_4, U_A)$$
$$Y \gets f_{Y}(W_1, W_2, W_3, W_4, A, U_Y)$$

##### 2. Translate your question into a formal target causal parameter, defined using counter-factuals.
The target causal parameter is the difference in the counterfactual probability of survival if all patients received both surgery and radiation and the counterfactual probability of survival if all patients received only surgery:

$$\theta^*=E^*(Y_1)-E^*(Y_0)=P^*(Y_1)-P^*(Y_0)$$

##### 3. Specify your observed data and its link to the causal model.



##### 4. Identify.


##### 5. Commit to a Statistical Model and Estimand (target parameter of the observed datadistribution).



