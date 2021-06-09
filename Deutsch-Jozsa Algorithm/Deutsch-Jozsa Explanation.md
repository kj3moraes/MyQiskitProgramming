## Deutsch-Jozsa Algorithm

### Background
Consider a blackbox function *f:{0,1} -> {0,1}* at takes in a single bit and outputs a single bit. Assume that this blackbox function is a very time consuming function that takes 24 hours to compute a result. We want to know if this function is constant or balanced (i.e is 0 = f(0) & 1 = f(1) or is 0 = f(1) and 1 = f(0)). Now to determine f(0) and f(1), we would need 48 hours. For a classical computation, 48 hours are mandatory. Can quantum computers do any better? This is called Deustch's problem. We will examine the solution and the classical vs. quantum strategies.

### Mathematics
We already saw that classical computation needs 48 hours for one to determine whether or not the function is constant or balanced. Deutsch came up with an ingenious solution to use superposition to determine this. Suppose that I define a unitary transformation on 2 qubits as follows :
<img src="https://render.githubusercontent.com/render/math?math=U_f |x\langle |y\langle\rightarrow \ket{x}\ket{y \oplus f(x)}">


### Implementation
