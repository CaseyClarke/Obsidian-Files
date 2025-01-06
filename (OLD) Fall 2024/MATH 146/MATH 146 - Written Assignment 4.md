1. 
	Using the shell method with the height being $sin(x^2-1)$ and the width being $x$ and bounds given by the question we get the equation 
	$$2\pi\int_1^{\sqrt{1+\pi}}xsin(x^2-1) \; dx$$
	$Let \; u = x^2 - 1$
	$dx = \frac{du}{2x}$
	$x = 1 \quad u = 0$
	$x = \sqrt{\pi + 1} \quad u = \pi$
	$$2\pi\int_0^\pi xsin(u)\frac{1}{2x} \; du$$
	$$\pi\int_0^\pi sin(u) \; du$$
	$$-\pi cos(u)\bigg\rvert^\pi_{0}$$
	$$\pi(-cos(\pi) + cos(0))$$
	$$2\pi$$
	$$\therefore \text{ The total volume of the cake is } 2\pi \text{ units cubed}$$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
	
2.  The equation of the circle is given by
	$$x^2+y^2=2^2$$
	Solving for $y$ gives
	$$y = \sqrt{4-x^2}$$
	The area of the square is then given by 
	$$S(x) = (2\sqrt{4-x^2})^2 = 4(4-x^2) = 16 - 4x^2$$
	The volume of this shape is given by the integral
	$$\int^2_{-2} S(x) dx$$
	$$\int^2_{-2}16dx - \int^2_{-2}4x^2 dx$$
	$$16x \bigg\rvert^2_{-2} - 4\frac{x^3}{3} \bigg\rvert^2_{-2}$$
	$$16(2) - 16(-2) - 4\left(\frac{2^3}{3} - \frac{(-2)^3}{3}\right)$$
	$$64 - \left(\frac{32}{3} + \frac{32}{3}\right)$$
	$$\frac{192}{3} - \frac{64}{3}$$
	$$\frac{128}{3}$$
	$$\therefore \text{ The volume of the solid is } \frac{128}{3} \text{ units cubed}$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
3. 
	To find the bounds we find the intersect of the two curves
	$$y^2 = 2- y^2$$
	$$y^2 = 1$$
	$$y = -1, 1$$
	Using the washers method given that we are rotating about $x=3$ the radii functions are subtracted from 3
	$$\pi\int^1_{-1} \left((3-y^2)^2 - (3-(2-y^2))^2\right)dy$$
	$$\pi\int^1_{-1} \left((3-y^2)^2 - (1+y^2)^2\right)dy$$
	$$\pi\int^1_{-1} \left((y^4-6y^2 + 9) - (y^4 + 2y^2 + 1)\right)dy$$
	$$\pi\int^1_{-1} \left( y^4 - 6y^2 + 9 - y^4 - 2y^2 - 1\right)dy$$
	$$\pi\int^1_{-1} \left(-8y^2 + 8\right)dy$$
	$$-8\pi\int^1_{-1} y^2 - 1 \; dy$$
	$$-8\pi\left(\frac{y^3}{3} - y\right) \bigg\rvert^1_{-1}$$
	$$-8\pi\left(\frac{1^3}{3} - 1 - \frac{(-1)^3}{3} -1\right)$$
	$$\frac{32\pi}{3}$$
	$$\therefore \text{ The volume of the solid is } \frac{32\pi}{3} \text{ units cubed }$$

	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

	There is a bonus question on the assignment pdf written in white text that I found by accident so here's my solution if that gets me any bonus marks
	Prove: $$\int_0^1(ln(x))^ndx = (-1)^nn!$$
	Using proof by induction
	Base Case $n= 0$	:
	$$\int_0^1(ln(x))^0dx = (-1)^00!$$
	$$1 = 1$$
	$$\therefore \text{The base case holds}$$
	Assume the formula works for n
	Inductive Step, $n = n+1$:
	Prove:
	 $$\int_0^1(ln(x))^{n+1}dx = (-1)^{n+1}(n+1)!$$
	$$\text{Using Integration by Parts}$$
	$$u = (ln(x))^{n+1}, \quad du = (n+1)(ln(x))^n\frac1x dx$$
	$$dv = dx, v = x$$
	$$\int_0^1(ln(x))^{n+1}dx = x(ln(x))^{n+1} \bigg\rvert^1_0 - \int_0^1x(n+1)(ln(x))^n\frac1x dx$$
	$$\int_0^1(ln(x))^{n+1}dx =  -(n+1) \int_0^1(ln(x))^ndx$$
	$$\text{Using the inductive hypothesis } \int_0^1(ln(x))^ndx = (-1)^nn!$$
	$$\int_0^1(ln(x))^{n+1}dx =  -(n+1)(-1)^nn!$$
	$$\int_0^1(ln(x))^{n+1}dx =  -1(-1)^n(n+1)n!$$
	$$\int_0^1(ln(x))^{n+1}dx =  (-1)^{n+1}(n+1)!$$
	Since $n=0$ is true and $n \implies n+1$ by induction the formula is true $\forall n \geq 0$
