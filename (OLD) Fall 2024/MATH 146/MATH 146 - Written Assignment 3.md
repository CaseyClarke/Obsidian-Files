1. $$\int_4^5\frac{dx}{(x-3)\sqrt{x^2-6x+8}}$$
	$$\int_4^5\frac{dx}{(x-3)\sqrt{(x-3)^2-1}}$$
	$Let \; u = x-3, \; dx= du$
	$$\int_1^2\frac{du}{u\sqrt{u^2-1}}$$
	$Let \; u = sec(\theta), \; du = sec(\theta)tan(\theta)d\theta$
	$$\int_{sec(1)}^{sec(2)}\frac{sec(\theta)tan(\theta)d\theta}{sec(\theta)\sqrt{(sec(\theta))^2-1}}$$
	$$\int_{sec(1)}^{sec(2)}\frac{sec(\theta)tan(\theta)d\theta}{sec(\theta)tan(\theta)}$$
	$$\theta \bigg\rvert^{sec(2)}_{sec(1)}$$
	Using the Triangle method to back-substitute $u$ into the equation:
	$u = sec(\theta)$ which means that the Hypotenuse is $1$ and Adjacent is $u$. Using Pythagorean theorem the Opposite side is $\sqrt{u^2-1}$. Solving for $\theta$ gives $\theta = tan^{-1}(\sqrt{u^2-1})$ 
	$$tan^{-1}(\sqrt{u^2-1}) \bigg\rvert^{2}_{1}$$
	$$tan^{-1}\left( \sqrt{(x-3)^2-1}\right) \bigg\rvert^{5}_{4}$$
	$$tan^{-1}\left( \sqrt{(5-3)^2-1}\right) - tan^{-1}\left( \sqrt{(4-3)^2-1}\right)$$
	$$tan^{-1}( \sqrt{3}) - tan^{-1}\left(0\right)$$
	$$\frac\pi3$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
2. $$\int\frac{xdx}{x^2+8x+20}$$
	$$\int\frac{xdx}{(x+4)^2+4}$$
	$Let \; u = x+4, \; du = dx$
	$$\int\frac{u-4}{u^2+4}dx$$
	$$\int\frac{u}{u^2+4}du - \int\frac{4}{u^2+4}du$$
	For the first integral:
	$$\int\frac{u}{u^2+4}du$$
	$Let \; v = u^2+4, \; du = \frac{dv}{2u}$
	$$\int\frac{u}{v}\frac{1}{2u}dv$$
	$$\frac12ln(|v|)+C_1$$
	$$\frac12ln(|u^2+4|)+C_1$$
	For the second integral:
	$$\int\frac{4}{u^2+4}du$$
	$$4\int\frac{1}{4(\frac{u^2}{4}+1)}du$$
	$$\int\frac{1}{(\frac{u}{2})^2+1}du$$
	$Let\; v = \frac u2, \; dv = 2du$
	$$2\int\frac{1}{v^2+1}du$$
	$$2tan^{-1}\left(v\right) + C_2$$
	$$2tan^{-1}\left(\frac{u}{2}\right) + C_2$$
	Combining them back together
	$Let \; C = C_1 + C_2$
	$$2ln(|u^2+4|) - \frac12tan^{-1}\left(\frac{u}{2}\right) + C$$
	$$2ln(|(x+4)^2+4|) - \frac12tan^{-1}\left(\frac{x+4}{2}\right) + C$$
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
3. $$\int\frac{x^3dx}{x^2-2x+4}$$
	Using Polynomial division the equation becomes
	$$\int (x-2) - \frac{8}{x^2-2x+4}dx$$
	$$ \frac{x^2}{2} -2x - 8\int\frac{1}{x^2-2x+4}dx$$
	$$ \frac{x^2}{2} -2x - 8\int\frac{1}{(x-1)^2+3}dx$$
	Taking out the integral 
	$$\int\frac{1}{(x-1)^2+3}dx$$
	$Let \; u = x-1, \; du = dx$
	$$\int\frac{1}{u^2+3}du$$
	$$\int\frac{1}{3(\frac{u^2}{3}+1)}du$$
	$$\frac{\sqrt{3}}{3}\int\frac{1}{(\frac{u}{\sqrt{3}})^2+1}du$$
	$$\frac{1}{\sqrt{3}} tan^{-1}\left(\frac{u}{\sqrt{3}}\right) +C$$
	$$\frac{1}{\sqrt{3}} tan^{-1}\left(\frac{x-1}{\sqrt{3}}\right) +C$$
	Combining the answers
	$$\frac{x^2}{2} -2x - 8\left(\frac{1}{\sqrt{3}} tan^{-1}\left(\frac{x-1}{\sqrt{3}}\right)\right) + C$$