1. 
	<br>(a)
	$$0 = \frac{N}{10}\left(1-\frac {N}{1000} \right) - 20\frac{N}{200+N}$$
	Has roots of $N = 0, N = 800$ but 0 is the trivial solution so we ignore it
	
	Given that $H_3 = 20$ and $A = 200$, the differential equation has an equilibrium solution at $N = 800$. The phase line below shows that when $N < 800, \quad N' > 0$ and $N > 800, \quad N' < 0$
	   Thus $N = 800$ is a stable equilibrium solution
	```tikz
	\usepackage{tikz}
	
	\newcommand*{\TickSize}{2pt}%
	
	\newcommand*{\AxisMin}{0}%
	\newcommand*{\AxisMax}{0}%
	
	\newcommand*{\DrawHorizontalPhaseLine}[5][]{%
	    % #1 = axis tick labels
	    % #2 = right arrows positions as CSV
	    % #3 = left arrow positions as CSV
	    \gdef\AxisMin{0}%
	    \gdef\AxisMax{0}%
	    \edef\MyList{#2}% Allows for #1 to be both a macro or not
	    \edef\Labels{#5}
		
	    \foreach \X [count=\c,evaluate=\c as \y using {{\Labels}[\c-1]}] in \MyList {
	        \draw  (\X,\TickSize) -- (\X,-\TickSize) node [below] {$\y$};
	        \ifnum\AxisMin>\X
	            \xdef\AxisMin{\X}%
	        \fi
	        \ifnum\AxisMax<\X
	            \xdef\AxisMax{\X}%
	        \fi
	    }
	
	    \edef\MyList{#3}% Allows for #2 to be both a macro or not
	    \foreach \X in \MyList {% Right arrows
	        \draw [->] (\X-0.1,0) -- (\X,0);
	        \ifnum\AxisMin>\X
	            \xdef\AxisMin{\X}%
	        \fi
	        \ifnum\AxisMax<\X
	            \xdef\AxisMax{\X}%
	        \fi
	    }
	
	    \edef\MyList{#4}% Allows for #3 to be both a macro or not
	    \foreach \X in \MyList {% Left arrows
	        \draw [<-] (\X-0.1,0) -- (\X,0);
	        \ifnum\AxisMin>\X
	            \xdef\AxisMin{\X}%
	        \fi
	        \ifnum\AxisMax<\X
	            \xdef\AxisMax{\X}%
	        \fi
	    }
	
	    \draw  (\AxisMax+1,0) -- (\AxisMin-1,0) node [left] {#1};
	}%
	
	
	\begin{document}
	\begin{tikzpicture}[thick]
	    \DrawHorizontalPhaseLine[$N$]{0,0}{-1}{1}{"800", "800"}%
	\end{tikzpicture}
	\end{document}
	```
    (b)
	
	$$0 = \frac{N}{10}\left(1-\frac {N}{1000} \right) - 20\frac{N}{50+N}$$
	Has roots of $N =0, N = 200, N = 750$ but again 0 is the trivial solution so we ignore it
    
	Given that $H_3 = 20$ and $A = 50$, the differential equation has equilibrium solutions at $N = 200, \; N =750$. The phase line below shows that $N = 200$ is an unstable solution and $N = 750$ is a stable solution
	```tikz
		\usepackage{tikz}
		
		\newcommand*{\TickSize}{2pt}%
		
		\newcommand*{\AxisMin}{0}%
		\newcommand*{\AxisMax}{0}%
		
		\newcommand*{\DrawHorizontalPhaseLine}[5][]{%
		    % #1 = axis tick labels
		    % #2 = right arrows positions as CSV
		    % #3 = left arrow positions as CSV
		    \gdef\AxisMin{0}%
		    \gdef\AxisMax{0}%
		    \edef\MyList{#2}% Allows for #1 to be both a macro or not
		    \edef\Labels{#5}
			
		    \foreach \X [count=\c,evaluate=\c as \y using {{\Labels}[\c-1]}] in \MyList {
		        \draw  (\X,\TickSize) -- (\X,-\TickSize) node [below] {$\y$};
		        \ifnum\AxisMin>\X
		            \xdef\AxisMin{\X}%
		        \fi
		        \ifnum\AxisMax<\X
		            \xdef\AxisMax{\X}%
		        \fi
		    }
		
		    \edef\MyList{#3}% Allows for #2 to be both a macro or not
		    \foreach \X in \MyList {% Right arrows
		        \draw [->] (\X-0.1,0) -- (\X,0);
		        \ifnum\AxisMin>\X
		            \xdef\AxisMin{\X}%
		        \fi
		        \ifnum\AxisMax<\X
		            \xdef\AxisMax{\X}%
		        \fi
		    }
		
		    \edef\MyList{#4}% Allows for #3 to be both a macro or not
		    \foreach \X in \MyList {% Left arrows
		        \draw [<-] (\X-0.1,0) -- (\X,0);
		        \ifnum\AxisMin>\X
		            \xdef\AxisMin{\X}%
		        \fi
		        \ifnum\AxisMax<\X
		            \xdef\AxisMax{\X}%
		        \fi
		    }
		
		    \draw  (\AxisMax+1,0) -- (\AxisMin-1,0) node [left] {#1};
		}%
		
		
		\begin{document}
		\begin{tikzpicture}[thick]
		    \DrawHorizontalPhaseLine[$N$]{-1,1}{0,0}{-1.5,1.5}{"200", "750"}%
		\end{tikzpicture}
		\end{document}
	```
	(c)
	
	The threshold extinction population for (b) is $N = 200$
	The main difference between this model and the constant harvesting model is that in this model the amount taken from the population by harvesting is dependent on the size of the current population while the constant harvesting model takes the same amount every time.

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

2. 
   <br>(a)
	$$\frac{dP}{dz} = -p(z)g$$
	$$dP = -gp_0\;dz$$
	$$\int dP = -g p_0 \int dz$$
	$$P(z) = -g p_0z + C$$
	Given that $P_0 = P(0) = 101.325 \; kP a \quad C = P_0$ 
	$$P(z) = P_0 - g p_0z$$
	
	Pressure on top of Mount Robinson: $P(3954) = 101.325 - (9.8)(1.225)(3954) = -47366.445$
	Pressure on top of Mount Everest: $P(8848) = 101.325 - (9.8)(1.225)(8848) = -106118.915$
	
	I'm no physicist but I don't think pressure is supposed to be negative, meaning we probably need a better model
	
	(b)
	
	$$\frac{dP}{dz} = -\frac{M}{RT}P(z)g$$
	$$\frac{dP}{P(z)} = -\frac{Mg}{RT} \;dz$$
	$$ \int \frac{dP}{P(z)} = -\frac{Mg}{RT} \int dz$$
	$$ P(z) = \pm e^{-z\frac{Mg}{RT} + c_1}$$
	$$ P(z) = \pm e^{c_1}e^{-z\frac{Mg}{RT}}$$
	$Let \; C = \pm e^{c_1}$
	$$P(z) = Ce^{-z\frac{Mg}{RT}}$$
	Given that $P_0 = P(0) = 101.325 \; kP a \quad C = P_0$ 
	$$P(z) = P_0e^{-z\frac{Mg}{RT}}$$
	Pressure on top of Mount Robinson: $P(3954) = 101.325e^{-(3954)\frac{0.02897(9.8)}{(8.314)(288)}} = 63.4029486229$
	Pressure on top of Mount Everest: $P(8848) = 101.325e^{-(8848)\frac{0.02897(9.8)}{(8.314)(288)}} = 35.4893436386$
	
	That looks a lot more accurate as the previous calculations
	
	(c)
	
	$$\frac{dP}{dz} = -\frac{gMP(z)}{R(T_0 - Lz)}$$
	$$\frac{1}{-gMP(z)}dP = \frac{1}{R(T_0 - Lz)}dz$$
	$$\frac{1}{-gM} \int \frac{1}{P(z)}dP = \int \frac{1}{R(T_0 - Lz)}dz$$
	$$\frac{R}{-gM} ln|P(z)| =  -\frac{1}{RL} ln|R(T_0 - Lz)| + c_1$$
	$Let \; c_2 = \frac{-Mg}{R}c_1$
	$$ P(z) =  \pm e^{\frac{Mg}{RL} ln|R(T_0 - Lz)| + c_2}$$
	$$ P(z) =  \pm e^{c_2}e^{\frac{Mg}{RL} ln|R(T_0 - Lz)|}$$
	$Let \; C = \pm e^{c_2}$
	$$ P(z) =  Ce^{\frac{Mg}{RL} ln|R(T_0 - Lz)|}$$
	Given that $P_0 = P(0) = 101.325 \; kP a$
	$$ P_0 =  Ce^{\frac{Mg}{RL} ln|RT_0|}$$
	$$ C =  \frac{P_0}{e^{\frac{Mg}{RL} ln|RT_0|}}$$
	$$ P(z) =  \frac{P_0}{e^{\frac{Mg}{RL} ln|RT_0|}}e^{\frac{Mg}{RL} ln|R(T_0 - Lz)|}$$
	$$ P(z) =  P_0e^{\frac{Mg}{RL} \left(ln\left|\frac{T_0 - Lz}{T_0}\right|\right)}$$
	$$ P(z) =  P_0\left|\frac{T_0 - Lz}{T_0}\right|^{\frac{Mg}{RL}}$$
	
	Pressure on top of Mount Robinson: 
	$P(3954) = 101.325\left|\frac{288 - (0.0065)(3954)}{288}\right|^{\frac{(0.02897)(9.8)}{(8.314)(0.0065)}} = 62.0076242892$
	Pressure on top of Mount Everest: 
	$P(8848) = 101.325\left|\frac{288 - (0.0065)(8848)}{288}\right|^{\frac{(0.02897)(9.8)}{(8.314)(0.0065)}} = 31.4389655792$
	
	This is similar to part (b) but slightly lower as the temperature at high altitudes is lower so the pressure should be lower as well. Also I looked it up and these numbers seem pretty close to the actual values, or at least closer than part (b)

<div style="page-break-after: always; visibility: hidden">\pagebreak</div>

3. 
	 <br>(a)
	
	$$\frac{dP}{dt} = k(t)P\left(1-\frac{P}{M(t)}\right)$$
	$z = \frac1P$
	$$\frac{dz}{dt} = \frac{1}{-P^2}\frac{dP}{dt}$$
	$$\frac{1}{-z^2}\frac{dz}{dt} = \frac{dP}{dt}$$
	$$\frac{1}{-z^2}\frac{dz}{dt} = k(t)\frac1z\left(1-\frac{\frac1z}{M(t)}\right)$$
	$$\frac{dz}{dt} = -k(t)z^2\left(\frac1z-\frac{\frac{1}{z^2}}{M(t)}\right)$$
	$$\frac{dz}{dt} = k(t)\left(-z+\frac{1}{M(t)}\right)$$
	$$\frac{dz}{dt} = -zk(t)+\frac{k(t)}{M(t)}$$
	$$\frac{dz}{dt}+zk(t) = \frac{k(t)}{M(t)}$$

	(b)

	$$I(t) = e^{\int k(t) dt}$$
	$$I(t) = e^{kt}$$
	$$\frac{d(I(t)z)}{dt} = I(t)\frac{k(t)}{M(t)}$$
	$$z = \frac{1}{I(t)}\int \frac{I(t)k(t)}{M(t)}dt+C$$
	$z = \frac1P$
	$$P = \frac{I(t)}{C + \int \frac{I(t)k(t)}{M(t)}dt}$$
	$$P = \frac{e^{kt}}{C + \int \frac{ke^{kt}}{M(t)}dt}$$
	
	(c)
	
	$$I(t) = e^{\int k(t)dt}$$
	$$\frac{d(I(t)z)}{dt} = I(t)\frac{k(t)}{M(t)}$$
	$$z I(t) + c= \frac{1}{M}\int I(t)k(t)dt$$
	$$\int I(t)k(t)dt = \int e^{\int k(t)dt}k(t)dt$$
	$Let \; u = e^{\int k(t)dt}$
	$\frac{du}{dt} = e^{\int k(t)dt}k(t)$
	$$\int uk(t)\frac{du}{e^{\int k(t)dt}k(t)}$$
	$$\int \frac{uk(t)du}{uk(t)} = \int du = u = e^{\int k(t)dt} = I(t)$$
	$$z I(t) + c = \frac{I(x)}{M}$$
	$Let \; C = -c$
	$$z = \frac{1}{M} + \frac{C}{I(z)}$$
	$$z = \frac{I(t)}{MI(t)} + \frac{MC}{I(z)M}$$
	$$z = \frac{I(t) + MC}{MI(t)}$$
	$$z = \frac{1 + MCI(t)^{-1}}{M}$$
	$z = \frac1P$
	$$P = \frac{M}{1 + MCe^{-\int k(t)dt}}$$
	
	(d)
	
	$k(t) = e^{-t}$
	$$P = \frac{M}{1 + MCe^{-\int e^{-t}dt}}$$
	$$P = \frac{M}{1 + MCe^{e^{-t}}}$$
	
	To find what happens to the population in the long term we look at the equation's asymptotic behaviour
	
	$$\lim_{t \to \infty}\frac{M}{1 + MCe^{e^{-t}}} = \frac{M}{1 + MC}$$
	
	Given that $P(0) = P_0$ for some initial value $P_0 < M$
	
	$$P_0 = \frac{M}{1 + MC}$$
	$$C = \frac{1}{P_0} - \frac1M$$
	$$\lim_{t \to \infty}\frac{M}{1 + MCe^{e^{-t}}} =\frac{M}{1 + (\frac{M}{P_0} - 1)}$$
	$$\lim_{t \to \infty}\frac{M}{1 + MCe^{e^{-t}}} = P_0$$

	This means that in the long term the population with stabilize around the value of the initial population, this makes sense as the growth rate $k(t) = e^{-t}$ asymptotically goes down to 0 with time so eventually the growth rate will be so low that the population essentially never changes, making it stabilize at some initial population size $P_0 < M$