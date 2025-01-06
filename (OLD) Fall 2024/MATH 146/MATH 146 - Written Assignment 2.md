1. 
	$\int_0^{\pi/2}\cos(x)^5\sin(x)^{40}dx$
	$\Rightarrow \int_0^{\pi/2}\cos(x)^2\cos(x)^2\cos(x)\sin(x)^{40}dx$ 
	Using the identity $\sin(x)^2 + \cos(x)^2 = 1$
	$\Rightarrow \int_0^{\pi/2}(1-\sin(x)^2)(1-\sin(x)^2)\cos(x)\sin(x)^{40}dx$ 
	Let $u = \sin(x)$    $dx = \frac{du}{\cos(x)}$
	$\Rightarrow \int_0^{1}(1-u^2)(1-u^2)\cos(x)u^{40}\frac{du}{\cos(x)}$
	$\Rightarrow \int_0^{1}(u^4-2u^2+1)u^{40} \ du$
	$\Rightarrow \int_0^{1}u^{44}-2u^{42}+u^{40} \ du$
	$\Rightarrow \frac{u^{45}}{45} -\frac{2u^{43}}{43} + \frac{u^{41}}{41} \bigg\rvert^1_0$
	$\Rightarrow (\frac{1^{45}}{45} -\frac{2(1)^{43}}{43} + \frac{1^{41}}{41}) - (\frac{0^{45}}{45} -\frac{2(0)^{43}}{43} + \frac{0^{41}}{41})$
	$\Rightarrow \frac{1}{45} - \frac{2}{43} + \frac{1}{41}$
	$\Rightarrow \frac{8}{79335}$
	$\approx 0.0001008382177$

	$\int \frac{dx}{\sqrt{1-16x^2}}$
	let $x = \frac14 \sin(\theta)$    
	$dx = \frac14 \cos(\theta) \ d\theta$
	$\Rightarrow \operatorname{\Huge\int} \frac{\frac14 \cos(\theta)}{\sqrt{1-16(\frac14 \sin(\theta))^2}} \ d\theta$
	$\Rightarrow \frac14\int \frac{ \cos(\theta)}{\cos(\theta)} \ d\theta$
	$\Rightarrow \frac14\int 1 \ d\theta$
	$\Rightarrow \frac14 \theta + C$
	Recall $x = \frac14 \sin(\theta)$
	$\rightarrow \sin(\theta) = 4x$
	$\rightarrow \theta = \sin^{-1}(4x)$
	Substituting $\theta$ into the equation gives
	$\Rightarrow \frac14 \sin^{-1}(4x) + C$
	<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
2. 
	$\int e^{2x}\cos(3x) \ dx$
	Using Integration By Parts (IBP)
	let $u = e^{2x}$   
	$du = 2e^{2x}dx$   
	let $dv = \cos(3x)dx$  
	$v = \frac13 \sin(3x)$
	$\int u \ dv = uv - \int v \ du + C_0$
	$\Rightarrow \int e^{2x}\cos(3x) \ dx = \frac13 e^{2x}\sin(3x) - \frac26 \int e^{2x}\sin(3x) \ dx + C_0$
	Let $R_0 = \frac13 e^{2x}\sin(3x)$	
	Let $R_1 = \int e^{2x}\sin(3x) \ dx$
	$\Rightarrow \int e^{2x}\cos(3x) \ dx = R_0 - \frac26 R_1 + C_0$  

	Now we do IBP for $R_1$
	$R_1 = \int e^{2x}\sin(3x) \ dx$
	let $u = e^{2x}$  
	$du = 2e^{2x}dx$   
	let $dv = \sin(3x)dx$ 
	$v = -\frac13 \cos(3x)$
	$\int u \ dv = uv - \int v \ du + C_1$
	$\Rightarrow R_1 = \int e^{2x}\sin(3x) \ dx = -\frac13 e^{2x}\cos(3x) + \frac26 \int e^{2x}\cos(3x) \ dx + C_1$
	Let $R_2 = -\frac13 e^{2x}\cos(3x)$
	Let $R_3 = \int e^{2x}\cos(3x) \ dx$
	$\Rightarrow R_1 = R_2 + \frac26 R_3 + C_1$

	Notice how $R_3$ is our original equation, because of this we substitute $R_0, R_1, R_2, \text{ and } R_3$ back into the equation $\int e^{2x}\cos(3x) \ dx = R_0 - \frac26 R_1 + C_0$
	$\int e^{2x}\cos(3x) \ dx = R_0 - \frac26 R_1 + C_0$  
	$\int e^{2x}\cos(3x) \ dx = R_0 - \frac26 (R_2 + \frac26 R_3 + C_1) + C_0$  
	$\int e^{2x}\cos(3x) \ dx = R_0 - \frac26 R_2 - \frac49 R_3 + \frac26 C_1 + C_0$,      $\quad C_2 = \frac26 C_1 + C_0$    
	$\int e^{2x}\cos(3x) \ dx = (\frac13 e^{2x}\sin(3x)) - \frac23 (-\frac23 e^{2x}\cos(3x)) - \frac49 (\int e^{2x}\cos(3x) \ dx) + C_2$
	$\int e^{2x}\cos(3x) \ dx + \frac49 \int e^{2x}\cos(3x) \ dx= \frac13 e^{2x}\sin(3x) + \frac46 e^{2x}\cos(3x) + C_2$
	$\int e^{2x}\cos(3x) \ dx (1 + \frac49) = \frac13 e^{2x}\sin(3x) + \frac46 e^{2x}\cos(3x) + C_2$
	$\int e^{2x}\cos(3x) \ dx (\frac{13}{9}) = \frac13 e^{2x}\sin(3x) + \frac46 e^{2x}\cos(3x) + C_2$
	$\int e^{2x}\cos(3x) \ dx = (\frac{9}{13})(\frac13 e^{2x}\sin(3x) + \frac46 e^{2x}\cos(3x) + C_2)$
	$\Rightarrow (\frac{9}{13})(\frac13 e^{2x}\sin(3x) + \frac23 e^{2x}\cos(3x) + C_2)$
	$\Rightarrow \frac{9}{39} e^{2x}\sin(3x) + \frac{18}{39} e^{2x}\cos(3x) + \frac{C_2}{13}$,     $\quad C_3 = \frac{C_2}{13}$
	$\Rightarrow \frac{9}{39} e^{2x}\sin(3x) + \frac{18}{39} e^{2x}\cos(3x) + C_3$
	$\Rightarrow \frac{3}{13} e^{2x}\sin(3x) + \frac{2}{13} e^{2x}\cos(3x) + C_3$
		<div style="page-break-after: always; visibility: hidden">\pagebreak</div>
3. 
	$I_n(x) = \int[ln(x)]^n \ dx$
	Using Integration By Parts
	let $u = [ln(x)]^n$      
	$du = \frac nx[ln(x)]^{n-1} \ dx$    
	let $dv =1dx$    
	$v = x$
	$\int u \ dv = uv - \int v \ du + C_1$
	$\Rightarrow x[ln(x)]^n - \int x \frac nx[ln(x)]^{n-1} \ dx + C_1$,    $\quad C_1 = 0$
	$\Rightarrow x[ln(x)]^n - n\int [ln(x)]^{n-1} \ dx$
	Notice that $\int [ln(x)]^{n-1}$ is the same as $I_{n-1}$, substituting this into the above equation gives
	$\Rightarrow I_n(x) = x[ln(x)]^n - nI_{n-1}$
	