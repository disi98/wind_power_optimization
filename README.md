# portfolio_website

# Newton-Raphson Method

Here is the Python function for the Newton-Raphson method:

```python
def newton_raphson_method(func, deriv_func, initial_guess, epsilon=1e-6):
    a = initial_guess
    while True:
        a_new = a - func(a) / deriv_func(a)
        if abs(a_new - a) < epsilon:
            break
        a = a_new
    return a