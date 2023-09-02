---
share: true
---
The Exponential Function is a continuation of the constant we know that's refered to as Euler's number. To summarise, Euler's number has everything to do with exponential growth and compounding interest (Which is the reason e^x's derivative is e^x).
$$e=\lim_{n \to \infty}{(1+\frac{1}{n})^n}$$
As mathematicions enevitably do, they extended e. The reason being? It has uses outside exponential growth. Now, we usually determine e to be an infinite sum.
$$e=\sum\limits_{n=0}^{\infty} \frac{1}{n!}$$
Now the exponential function is very similar to this sum.
$$\exp(x)=\sum\limits_{n=0}^{\infty} \frac{x^{n}}{n!}$$
There are a few things to note about this function.
## 1) It acts like indices
The exponential function acts the same way indices do, as in:
$$\exp(x)\times\exp(y)=\exp(x+y)$$
$$\exp(x)\div\exp(y)=\exp(x-y)$$
Now you can see where people got the notation of:
$$\exp(x)=e^x$$
Which is how the NSW syllabus refers to it, but it should be known that this is referring to the summation.

## 2) It is it's own derivative
The derivative of exp(x) is itself, here's the proof.
$$\exp(x) = \frac{x^0}{0!} + \frac{x^1}{1!} + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \ ...$$
$$f(x) = 1 + x + \frac{x^2}{2} + \frac{x^3}{6} + \frac{x^4}{24} + \ ...$$
$$f'(x) = x^0 + 2\frac{x^1}{2} + 3\frac{x^2}{6} + 4\frac{x^3}{24} + \ ...$$
$$f'(x) = 1 + x + \frac{x^2}{2} + \frac{x^3}{6} + \ ...$$
## 3) Sine and Cosine
The exponential function has something to do with sine and cosine, we know this because the Polar Form and Exponential Form ([Exploring Forms of Complex Numbers](Exploring%20Forms%20of%20Complex%20Numbers.md)) both exist. So let's go through this proof.

First we need to define a few things, sine and cosine (just like the exponential function) are shorthand for an infinite series:
$$\sin(x)=\sum_{n=0}^{\infty}{\frac{(-1)^n}{(2n+1)!}x^{2n+1}}$$
$$\therefore sin(x)=x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \ ...$$
$$\cos(x)=\sum_{n=0}^{\infty}{\frac{(-1)^n}{(2n)!}x^{2n}}$$
$$\therefore sin(x)=1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \ ...$$
This is the proof:
$$\exp(i\theta) = \frac{(i\theta)^0}{0!} + \frac{(i\theta)^1}{1!} + \frac{(i\theta)^2}{2!} + \frac{(i\theta)^3}{3!} + \frac{(i\theta)^4}{4!} + \frac{(i\theta)^5}{5!} + \ ...$$
$$\exp(i\theta) = 1 + i\theta + \frac{(-1)\theta^2}{2!} + \frac{(-i)\theta^3}{3!} + \frac{(1)\theta^4}{4!} + \frac{(i)\theta^5}{5!} + \ ...$$
$$\exp(i\theta) = 1 + i\theta - \frac{\theta^2}{2!} - \frac{i\theta^3}{3!} + \frac{\theta^4}{4!} + \frac{i\theta^5}{5!} + \ ...$$
Collect real and imaginary terms:
$$\exp(i\theta) = (1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} + \ ...) + (i\theta - \frac{i\theta^3}{3!} + \frac{i\theta^5}{5!} + \ ...)$$
$$\exp(i\theta) = (1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} + \ ...) + i(\theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} + \ ...)$$
$$where: \ \ 1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} + \ ... \ = \cos(\theta), \  \ \theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} + \ ... \ =\sin(\theta)$$
$$\therefore \exp(i\theta)=\cos{\theta}+i\sin{\theta}$$
That's the basics of the exponential function.