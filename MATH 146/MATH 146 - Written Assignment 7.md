1. 
	<br>$$\frac{\partial}{\partial x}f(x,y) = \frac{\partial}{\partial x}x(x^2+y^2)^{-3/2}e^{sin(x^ay)}$$
	$$\frac{\partial f}{\partial x} = ax^ay(x^2 + y^2)^{-3/2}e^{sin(x^ay)}cos(x^ay) +  e^{sin(x^ay)}\left(\frac{\partial}{\partial x}(x(x^2+y^2)^{-3/2})\right)$$
	$$\frac{\partial f}{\partial x} = ax^ay(x^2 + y^2)^{-3/2}e^{sin(x^ay)}cos(x^ay) +  e^{sin(x^ay)}(-3x^2(x^2 + y^2)^{-5/2} + (x^2 + y^2)^{-5/2})$$
	$$\frac{\partial f}{\partial x} = ax^ay(x^2 + y^2)^{-3/2}e^{sin(x^ay)}cos(x^ay) - 3x^2(x^2 + y^2)^{-5/2}e^{sin(x^ay)} + (x^2 + y^2)^{-5/2}e^{sin(x^ay)}$$
	$$\begin{eqnarray} 
	\frac{\partial f}{\partial x}\bigg\rvert_{(1,0)}    \\
	&=&a(1)^a(0)((1)^2 +(0)^2)^{-3/2}e^{sin((1)^a(0))}cos((1)^a(0))  \\
	&-& 3(1)^2((1)^2 + (0)^2)^{-5/2}e^{sin((1)^a(0))}  \\
	&+& ((1)^2 + (0)^2)^{-5/2}e^{sin((1)^a(0))}
	\end{eqnarray}$$

	$$\frac{\partial f}{\partial x}\bigg\rvert_{(1,0)} = 0 -3(1)^{-5/2} + (1)^{-5/2}$$
	$$\frac{\partial f}{\partial x}\bigg\rvert_{(1,0)} = -2$$
	
	Therefore at $(1,0)$ this is always equal to -2 $\forall a \in \mathbb{R}$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. 
	<br>$$f = x^3 -3x+y^2$$
	$$f_x = \frac{\partial}{\partial x}(x^3 - 3x +y^2) = 3x^2 - 3$$
	$$f_y = \frac{\partial}{\partial y}(x^3 -3x +y^2) = 2y$$
	$$\text{Setting Both Derivatives to 0 to find critical points}$$
	$$f_x = 0, \; f_y =0\Rightarrow 3x^2 -3 = 0, \;2y = 0$$
	$$y = 0, \; x = \pm 1 \Rightarrow (x,y) = (1,0), \; (x,y) = (-1,0) \text{ Are both critial points}$$
	$$f_{xx} = \frac{\partial}{\partial x}(3x^2 -3) = 6x$$
	$$f_{yy} = \frac{\partial}{\partial y}(2y) = 2$$
	$$f_{xy} = f_{yx} = 0$$
	$$D(a,b) = \begin{vmatrix}   f_{xx}& f_{xy}\\f_{yx} & f_{yy}\\ \end{vmatrix}(a,b) = f_{xx}(a,b)f_{yy}(a,b) = 12x$$
	$$D(1,0) = 12(1) > 0  \;\wedge \; f_{xx}(1,0) > 0 \;\Rightarrow (1,0)\text{ is a Local Minimum}$$
	$$D(-1,0) = 12(-1) < 0  \;\Rightarrow (-1,0)\text{ is a Saddle Point}$$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. 
	<br>	$$\frac{\partial x}{\partial \theta} = -rsin(\theta)$$
	$$\frac{\partial y}{\partial \theta} = rcos(\theta)$$
	$$\frac{\partial x}{\partial r} = cos(\theta)$$
	$$\frac{\partial y}{\partial r} = sin(\theta)$$
	
	$$\frac{\partial z}{\partial r} = \frac{\partial z}{\partial x} \frac{\partial x}{\partial r} + \frac{\partial z}{\partial y} \frac{\partial y}{\partial r}$$
	$$\frac{\partial z}{\partial r} = \frac{\partial z}{\partial x} cos(\theta) + \frac{\partial z}{\partial y} sin(\theta)$$
	$$\frac{\partial^2 z}{\partial r^2} = cos(\theta)\frac{\partial}{\partial r}\frac{\partial z}{\partial x}  + sin(\theta)\frac{\partial}{\partial r}\frac{\partial z}{\partial y} $$
	$$\frac{\partial^2 z}{\partial r^2} = cos(\theta)(\frac{\partial^2 z}{\partial x^2}\frac{\partial x}{\partial r} + \frac{\partial^2 z}{\partial x \partial y}\frac{\partial y}{\partial r})  + sin(\theta)(\frac{\partial^2 z}{\partial x^2}\frac{\partial x}{\partial r} + \frac{\partial^2 z}{\partial x \partial y}\frac{\partial y}{\partial r})$$
	$$\frac{\partial^2 z}{\partial r^2} = cos^2(\theta)\frac{\partial^2 z}{\partial x^2} + 2sin(\theta)cos(\theta)\frac{\partial^2 z}{\partial x \partial y} + sin^2(\theta)\frac{\partial^2 z}{\partial y^2}$$
	
	
	$$\frac{\partial z}{\partial\theta} = \frac{\partial z}{\partial x} \frac{\partial x}{\partial \theta} + \frac{\partial z}{\partial y} \frac{\partial y}{\partial \theta}$$
	$$\frac{\partial z}{\partial\theta} = -rsin(\theta)\frac{\partial z}{\partial x} + \frac{\partial z}{\partial y}rcos(\theta)$$
	$$\frac{\partial^2 z}{\partial\theta^2} = -rcos(\theta)\frac{\partial z}{\partial x} -rsin(\theta)\frac{\partial }{\partial \theta}\frac{\partial z}{\partial x} -rsin(\theta)\frac{\partial z}{\partial y} +rcos(\theta)\frac{\partial }{\partial \theta}\frac{\partial z}{\partial y} $$
	$$\begin{eqnarray} 
	\frac{\partial^2 z}{\partial\theta^2} 
	&=&-rcos(\theta)\frac{\partial z}{\partial x} - rsin(\theta)\frac{\partial z}{\partial y}\\
	&-& rsin(\theta)(\frac{\partial^2 z}{\partial x^2}\frac{\partial x }{\partial \theta} + \frac{\partial^2 z}{\partial x \partial y}\frac{\partial y }{\partial \theta}) \\
	&+& rcos(\theta)(\frac{\partial^2 z}{\partial x^2}\frac{\partial x }{\partial \theta} + \frac{\partial^2 z}{\partial x \partial y}\frac{\partial y }{\partial \theta})
	\end{eqnarray}$$
	$$\begin{eqnarray} 
	\frac{\partial^2 z}{\partial\theta^2} 
	&=&-rcos(\theta)\frac{\partial z}{\partial x} - rsin(\theta)\frac{\partial z}{\partial y}\\
	&-& rsin(\theta)(-rsin(\theta)\frac{\partial^2 z}{\partial x^2} + rcos(\theta)\frac{\partial^2 z}{\partial x \partial y}) \\
	&+& rcos(\theta)(-rsin(\theta)\frac{\partial^2 z}{\partial x^2} + rcos(\theta)\frac{\partial^2 z}{\partial x \partial y})
	\end{eqnarray}$$
	$$\frac{\partial^2 z}{\partial\theta^2} = -r(cos(\theta)\frac{\partial z}{\partial x} +sin(\theta)\frac{\partial z}{\partial y}) + r^2(cos^2(\theta)\frac{\partial^2 z}{\partial y^2} - 2sin(\theta)cos(\theta)\frac{\partial^2 z}{\partial x \partial y} + sin^2(\theta)\frac{\partial^2 z}{\partial x^2})$$
	$$\frac{1}{r^2}\frac{\partial^2 z}{\partial\theta^2} = \frac{-1}{r}\frac{\partial z}{\partial r} + cos^2(\theta)\frac{\partial^2 z}{\partial y^2} - 2sin(\theta)cos(\theta)\frac{\partial^2 z}{\partial x \partial y} + sin^2(\theta)\frac{\partial^2 z}{\partial x^2}$$
	$$\frac{1}{r^2}\frac{\partial^2 z}{\partial\theta^2} + \frac{1}{r}\frac{\partial z}{\partial r} + \frac{\partial^2 z}{\partial r^2} = \frac{\partial^2 z}{\partial r^2}+  cos^2(\theta)\frac{\partial^2 z}{\partial y^2} - 2sin(\theta)cos(\theta)\frac{\partial^2 z}{\partial x \partial y} + sin^2(\theta)\frac{\partial^2 z}{\partial x^2}$$
	$$\frac{1}{r^2}\frac{\partial^2 z}{\partial\theta^2} + \frac{1}{r}\frac{\partial z}{\partial r} + \frac{\partial^2 z}{\partial r^2} =   cos^2(\theta)\frac{\partial^2 z}{\partial y^2} + sin^2(\theta)\frac{\partial^2 z}{\partial x^2} + cos^2(\theta)\frac{\partial^2 z}{\partial x^2} + sin^2(\theta)\frac{\partial^2 z}{\partial y^2}$$
	$$\frac{1}{r^2}\frac{\partial^2 z}{\partial\theta^2} + \frac{1}{r}\frac{\partial z}{\partial r} + \frac{\partial^2 z}{\partial r^2} =   (cos^2(\theta) + sin^2(\theta))(\frac{\partial^2 z}{\partial x^2} + \frac{\partial^2 z}{\partial x^2})$$
	
	$$cos^2(\theta) + sin^2(\theta) = 1$$
	$$\frac{1}{r^2}\frac{\partial^2 z}{\partial\theta^2}  + \frac{1}{r}\frac{\partial z}{\partial r} + \frac{\partial^2 z}{\partial r^2}= \frac{\partial^2 z}{\partial x^2} + \frac{\partial^2 z}{\partial y^2}$$
	
<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

4. 
	<br>$$f = e^{-\frac{x^3}{3} + x - y^2}$$
	$$f_x = \frac{\partial}{\partial x}(e^{-\frac{x^3}{3} + x - y^2}) = e^{-\frac{x^3}{3} + x - y^2}(-x^2+1)$$
	$$f_y = \frac{\partial}{\partial y}(e^{-\frac{x^3}{3} + x - y^2}) = e^{-\frac{x^3}{3} + x - y^2}(-2y)$$
	$$\text{Setting Both Derivatives to 0 to find critical points}$$
	$$f_x = 0, \; f_y =0\Rightarrow e^{-\frac{x^3}{3} + x - y^2}(-x^2+1) = 0, \;e^{-\frac{x^3}{3} + x - y^2}(-2y) = 0$$
	$$y = 0, \; x = \pm 1 \Rightarrow (x,y) = (1,0), \; (x,y) = (-1,0) \text{ Are both critial points}$$
	$$f_{xx} = \frac{\partial}{\partial x}(e^{-\frac{x^3}{3} + x - y^2}(-x^2+1)) = e^{-\frac{x^3}{3} + x - y^2}(-2x) + e^{-\frac{x^3}{3} + x - y^2}(-x^2+1)^2$$
	$$f_{yy} = \frac{\partial}{\partial y}(e^{-\frac{x^3}{3} + x - y^2}(-2y)) = e^{-\frac{x^3}{3} + x - y^2}(-2) + e^{-\frac{x^3}{3} + x - y^2}(-2y)^2$$
	$$f_{xy} = f_{yx} = \frac{\partial}{\partial x}(e^{-\frac{x^3}{3} + x - y^2}(-2y)) = -2y(e^{-\frac{x^3}{3} + x - y^2}(-x^2+1))$$
	$$D(a,b) = \begin{vmatrix}   f_{xx}& f_{xy}\\f_{yx} & f_{yy}\\ \end{vmatrix}(a,b) = f_{xx}(a,b)f_{yy}(a,b) - (f_{xy}(a,b))^2$$
	$$\begin{eqnarray} 
	D(a,b)   \\
	&=& (e^{-\frac{x^3}{3} + x - y^2}(-2x) + e^{-\frac{x^3}{3} + x - y^2}(-x^2+1)^2)(e^{-\frac{x^3}{3} + x - y^2}(-2) + e^{-\frac{x^3}{3} + x - y^2}(-2y)^2)\\
	&-&  (-2y(e^{-\frac{x^3}{3} + x - y^2}(-x^2+1)))^2\\
	\end{eqnarray}$$
	$$\begin{eqnarray} 
	D(a,b)   \\
	&=& (e^{-\frac{x^3}{3} + x - y^2})^2((-2x) + (-x^2+1)^2)((-2) + (-2y)^2)\\
	&-&  (e^{-\frac{x^3}{3} + x - y^2})^24y^2(-x^2+1)^2\\
	\end{eqnarray}$$
	$$D(a,b) = (e^{-\frac{x^3}{3} + x - y^2})^2(((-2x) + (-x^2+1)^2)((-2) + (-2y)^2) - (4y^2(-x^2+1)^2)) $$
	$$D(1,0) > 0  \;\wedge \; f_{xx}(1,0) < 0 \;\Rightarrow (1,0)\text{ is a Local Maxmimum}$$
	$$D(-1,0) < 0  \;\Rightarrow (-1,0)\text{ is a Saddle Point}$$

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

5. 
	<br>$$\text{Given that }\frac{|x|}{\sqrt{x^2+y^2}} \leq 1$$$$|x| \leq \sqrt{x^2+y^2}$$
	$$\pm x \leq \sqrt{x^2+y^2}$$
	$$-\sqrt{x^2+y^2}\leq x \leq \sqrt{x^2+y^2}$$
	$$-1\leq \frac{x}{\sqrt{x^2+y^2}} \leq 1$$
	$$-y\leq \frac{xy}{\sqrt{x^2+y^2}} \leq y$$
	$$\lim_{(x,y) \rightarrow (0,0)}-y\leq \lim_{(x,y) \rightarrow (0,0)}\frac{xy}{\sqrt{x^2+y^2}} \leq \lim_{(x,y) \rightarrow (0,0)}y$$
	$$\lim_{(x,y) \rightarrow (0,0)}y \;= \lim_{(x,y) \rightarrow (0,0)}-y \; = 0$$
	$$0\leq \lim_{(x,y) \rightarrow (0,0)}\frac{xy}{\sqrt{x^2+y^2}} \leq 0$$
	$$\therefore  \lim_{(x,y) \rightarrow (0,0)}\frac{xy}{\sqrt{x^2+y^2}} = 0$$





<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
