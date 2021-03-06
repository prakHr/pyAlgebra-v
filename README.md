# pyAlgebra-v
performs integral and differentiable operations on string expressions using sympy

## Motivation
The motivation behind it came from the purpose and realisation to **help** others understand it in a much better.
**In other words,** to push others and become a better version of ourselves.

## Tech/framework used
Ex. - latest version of sympy(or 1.8), matplotlib(or 3.1.3)

<b>Built with</b>
- [idle-python3](http://echorand.me/site/notes/articles/idle/article.html)

## Code Example
```python3
#For example :-
import matplotlib.pyplot as plt
from sympy import sympify
from sympy import Poly,Symbol,summation,pprint,solve,Integral,Derivative
from sympy import solve_poly_inequality,solve_rational_inequalities,solve_univariate_inequality,sin
    
expr='-x**2 + 4 < 0'
pprint(inequality_solver(expr))
    
expr='((x-1)/(x+2)) > 0'
pprint(inequality_solver(expr))

expr='sin(x)-0.6>0'
pprint(inequality_solver(expr))

r1,r2=roots(1,1,1)
print(r1,r2)

x_values=list(range(-1000,1000))
expr='x*x*x*x+5*x*x*x+10*x*x+12*x+1'
plot_general_equation(expr,x_values)

x=Symbol('x')
y=Symbol('y')
z=Symbol('z')
expr1=2*x+2*y+2*z
expr2=4*x+4*y+4*z
expr3=3*x+3*y+3*z
expressions=(expr1,expr2,expr3)
print(solve_n_equations(expressions))

expr = 'a*n+d'
upto = 10000
s=seriesSummation(expr,upto)
pprint(s)
    
St='5*u*t**2+2*t+8'
Stt=find_derivative(St,'t')
pprint(Stt)
Sttt=find_derivative(Stt,'t')
pprint(Sttt)

```