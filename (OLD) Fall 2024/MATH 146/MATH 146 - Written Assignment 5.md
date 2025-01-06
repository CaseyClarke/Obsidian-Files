1.  
	<br>Using hyperbolic trig identity for $cosh$
	$x = cosh(y)$
	$x' = sinh(y)$
	$$S = 2\pi\int^{ln(2)}_0x\sqrt{1+(x')^2}dy$$
	$$S = 2\pi\int^{ln(2)}_0cosh(y)\sqrt{1+sinh^2(y)}dy$$
	$$S = 2\pi\int^{ln(2)}_0cosh^2(y)dy$$
	$$S = 2\pi\int^{ln(2)}_0\frac{1+cosh(2y)}{2}dy$$
	$$S = \pi\int^{ln(2)}_01 dy +\pi\int^{ln(2)}_0cosh(2y)dy$$
	$$S = \pi \left( y \bigg\rvert^{ln(2)}_{0} + \frac12sinh(2y)\right) \bigg\rvert^{ln(2)}_{0}$$
	$$S = \pi \left( ln(2) + \frac12sinh(2ln(2)) - \frac12sinh(0) \right)$$
	$$S = \pi \left( ln(2) + \frac12\frac{e^{2ln(2)}-e^{-2ln(2)}}{2}\right)$$
	$$S = \pi \left( ln(2) + \frac{2^2-2^{-2}}{4}\right)$$
	$$S = \pi \left( ln(2) + \frac{15}{8}\right)$$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
2. 
	<br>The equation for the width of the water in any slice of the tank is given by $w(y) = \frac23y$
	which means that the area of a slice is given by $A(y) = w(y)dy$
	Using $F = PA$ and newtons pressure equation $P = pgd$ with our slices of the tank
	$$F = pgd \; A(y)$$
	$$dF = pgy\;w(y) \;dy$$	
	$$dF = \frac23 (1000)(9.81)y^2dy$$	
	Integrating both sides
	$$F = \frac23 (1000)(9.81)\frac{y^3}{3}$$	
	Setting this equal to the maximum allowed force
	$$2500 = \frac23 (1000)(9.81)\frac{y^3}{3}$$
	$$y = \sqrt[3]{\frac{25(9)}{2(9.81)}}$$
	$$y \approx 2.2551$$
	Now that we have the maximum height it can withstand we can find the total volume of the shape with that height
	$$V = \frac12 (bh) \;  w$$
	$$V = \frac12 10\; y\; w(y)$$
	$$V = \frac12 10\; y\; \frac23y$$
	$$V =10\frac13y^2$$
	$$V = 10\frac13(2.2551)^2$$
	$$v \approx 16.9516 \; m^3$$
	$$\therefore \text{ The container can hold roughly 17 }m^3 \text{ of water before exceeding it's limitation } $$