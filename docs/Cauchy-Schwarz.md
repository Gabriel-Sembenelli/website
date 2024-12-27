# Desigualdade de Cauchy-Schwarz

No *Principles of Mathematical Analysis*, de Walter Rudin, encontramos uma demonstração dessa desigualdade que, a princípio, parece passe de mágica. Com um olhar mais cuidadoso, porém, percebemos que é uma ligeira variação de uma demonstração clássica. Após algumas horas dissecando essa demonstração e finalmente entender sua motivação, resolvi escrever esse texto para nunca mais esquecer.

## Forma vetorial

Seja $V$ um espaço vetorial sobre um corpo $\mathbb{K}$, munido de um produto interno $\left< \cdot, \cdot \right> : V^2 \rightarrow \mathbb{K}$. A desigualdade de Cauchy-Schwarz afirma, para quaisquer $x,y\in V$, que

$$\left|\left<x,y\right>\right|^2 \leq \left<x,x\right> \left<y,y\right>$$

### Prova

A prova vem da observação que, para qualquer escalar $t \in \mathbb{K}$, vale $|x-ty|^2 \geq 0$, afinal, estamos falando sobre a norma de um vetor. Uma escolha esperta para $t$ permite deduzir a desigualdade.

Antes, porém, vamos eliminar o caso trivial em que $y=0$. Nesse caso, a desigualdade dirá que $0\leq 0$, o que obviamente é válido. Dessa forma, considere daqui em diante que $y\neq 0$, de modo que $\left<y,y\right> > 0$.

Agora observe que, para todo $t \in \mathbb{K}$, vale

$$\begin{align}
|x-ty|^2 &= \left< x-ty, x-ty \right> \\
&= \left<x,x\right> + \left<x,-ty\right> + \left<-ty,x\right> + \left<-ty,-ty\right> \\
&= \left<x,x\right> - \overline{t}\left<x,y\right> - t\left<y,x\right> + t\overline{t}\left<y,y\right> \geq 0.
\end{align}$$

Em particular, isso vale para $t = \frac{\left<x,y\right>}{\left<y,y\right>}$ que, quando substituído na última expressão, resulta em

$$\begin{align}
&\left<x,x\right> - \overline{\left(\frac{\left<x,y\right>}{\left<y,y\right>}\right)}\left<x,y\right> - \left(\frac{\left<x,y\right>}{\left<y,y\right>}\right)\left<y,x\right> + \left(\frac{\left<x,y\right>}{\left<y,y\right>}\right)\overline{\left(\frac{\left<x,y\right>}{\left<y,y\right>}\right)}\left<y,y\right> = \\
=\;&\left<x,x\right> - \frac{\overline{\left<x,y\right>}\left<x,y\right>}{\left<y,y\right>} - \frac{\left<x,y\right>\left<y,x\right>}{\left<y,y\right>} + \frac{\left<x,y\right>\overline{\left<x,y\right>}}{\left<y,y\right>} \\
=\;&\left<x,x\right> - \frac{\overline{\left<x,y\right>}\left<x,y\right>}{\left<y,y\right>} \geq 0 \\
\Rightarrow\;& \left<x,x\right> \geq \frac{\overline{\left<x,y\right>}\left<x,y\right>}{\left<y,y\right>} \\
\Rightarrow\;& \left<x,x\right> \left<y,y\right> \geq \left|\left<x,y\right>\right|^2. \;\;_\blacksquare
\end{align}$$

## Forma analítica

Se $a_1,\dotsc,a_n$ e $b_1,\dotsc,b_n$ são números complexos, então

$$\left|\sum_{j=1}^{n}a_j\overline{b_j}\right|^2 \leq \left(\sum_{j=1}^{n} |a_j|^2\right) \left(\sum_{j=1}^{n} |b_j|^2\right).$$

Note que, no caso anterior, se $V = \mathbb{C}^n$, $x=(a_1,\dotsc,a_n)^T$, $y=(b_1,\dotsc,b_n)^T$ e $\left<x,y\right>:=\sum_{j=1}^{n}a_j\overline{b_j}$, então o resultado já estaria provado como um corolário. Entretanto, gostaria de apresentar uma prova similar, que encontrei no livro do Rudin.

### Prova

Denote $A = \sum_{j=1}^{n}|a_j|^2$, $B = \sum_{j=1}^{n}|b_j|^2$, $C = \sum_{j=1}^{n}a_j\overline{b_j}$. Se $B=0$, isso significa que $b_1=\dotsb=b_n=0$, e a conclusão é trivial. Assuma portanto que $B>0$.

A partir daqui, se continuarmos seguindo o mesmo caminho da prova anterior, vamos observar que, para qualquer $t\in\mathbb{C}$ vale

$$\left<x-ty,x-ty\right> = \sum_{j=1}^{n} |a_j - t b_j|^2 \geq 0.$$

Então escolheremos $t=\frac{\left<x,y\right>}{\left<y,y\right>}=\frac{\sum a_j \overline{b_j}}{\sum |b_j|^2}=\frac{C}{B}$ para finalizar.
Mas é possível fazer de uma forma ligeiramente diferente.

Observe que, para quaisquer $s,t\in\mathbb{C}$, vale

$$\left<sx-ty,sx-ty\right> = \sum_{j=1}^{n} |s a_j - t b_j|^2 \geq 0.$$

Em particular, isso vale para $s=B$ e $t=C$, de modo que teremos

$$\begin{align}
&\sum_{j=1}^{n} |B a_j - C b_j|^2 \\
=\;&\sum_{j=1}^{n} (B a_j - C b_j)\overline{(B a_j - C b_j)} \\
=\;&\sum_{j=1}^{n} (B a_j - C b_j)(B \overline{a_j} - \overline{C} \overline{b_j}) \\
=\;&B^2\sum_{j=1}^{n}a_j\overline{a_j} - B\overline{C}\sum_{j=1}^{n}a_j\overline{b_j} - BC\sum_{j=1}^{n}\overline{a_j}b_j + C\overline{C}\sum_{j=1}^{n}b_j\overline{b_j} \\
=\;&B^2A - B\overline{C}C - BC\overline{C} + C\overline{C}B \\
=\;&B(AB - |C|^2) \geq 0.
\end{align}$$

Mas como $B > 0$, a última desigualdade implica que $AB - |C|^2 \geq 0$, donde $|C|^2 \leq AB$ é a desigualdade desejada.$\;\;_\blacksquare$

> Talvez a motivação de Rudin foi evitar denominadores da expressão $x - \frac{C}{B}y$, escalando por um fator de $B$ para obter $Bx-Cy$ e, consequentemente, expressões mais elegantes.