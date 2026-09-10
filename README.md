# CBA01-Michaelis-Menten-Case
This is Computational Biology Assignment which we have to model Michaelis Menten Reaction 

## Reaction Network Michaelis Menten
$S + E \underset{v_{-1}}{\overset{v_1}{\rightleftharpoons}} C \xrightarrow{v_2} P + E$

$$v_1 = k_1 [S][E]$$
$$v_{-1} = k_{-1} [C]$$
$$v_2 = k_2 [C]$$

The total enzyme concentration: $e_T = e + c$.

$$\frac{d}{dt} s(t) = -v_1 + v_1 = -k_1 s(t) e(t) + k_{-1} c(t)$$
$$\frac{d}{dt} e(t) = -v_1 + v_{-1} = -k_1 s(t) e(t) + k_{-1} c(t)$$
$$\frac{d}{dt} c(t) = v_1 - v_{-1} - v_2 = k_1 s(t) e(t) - k_{-1} c(t) - k_2 c(t)$$
$$\frac{d}{dt} p(t) = v_2 = k_2 c(t)$$

Since enzyme is not consumed in the reaction, therefore enzyme is constant which can re-write as below
e(t) = e_T - c(t)

Therefore the equation for this case.
$$\frac{d}{dt} s(t) = -k_1 s(t) (e_T - c(t)) - k_{-1} c(t)$$
$$\frac{d}{dt} c(t) = k_1 s(t) (e_T - c(t)) - k_{-1} c(t) - k_2 c(t)$$
$$\frac{d}{dt} p(t) = k_2 c(t)$$
