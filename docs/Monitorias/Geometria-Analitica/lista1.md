# Lista 1 - Vetores

## Exercício 1
Sendo $ABCDEFGH$ o paralelogramo abaixo, expresse os seguintes vetores em função
de $\overrightarrow{AB}$, $\overrightarrow{AC}$ e $\overrightarrow{AF}$:

**a) $\overrightarrow{BF}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
  Note que
  
  $$\overrightarrow{AB} + \overrightarrow{BF} = \overrightarrow{AF}$$
  
  Isolando $\overrightarrow{BF}$, temos,
  
  $$\tag{a.1} \overrightarrow{BF} = \boxed{\overrightarrow{AF} - \overrightarrow{AB}}$$
</details>

**b) $\overrightarrow{AG}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
  Note que
  
  $$\tag{b.1} \overrightarrow{AG} = \overrightarrow{AC} + \overrightarrow{CG}$$
  
  Além disso, perceba que, pelo exercício anterior, temos,
  
  $$\tag{b.2} \overrightarrow{CG} = \overrightarrow{BF} = \overrightarrow{AF} - \overrightarrow{AB}$$
  
  Então, substituindo $(b.2)$ em $(b.1)$, concluímos,
  
  $$\overrightarrow{AG} = \boxed{\overrightarrow{AC} + \overrightarrow{AF} - \overrightarrow{AB}}$$
</details>

Arrumar daqui pra baixo

**c) $\overrightarrow{AE}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
  $$\overrightarrow{AE} = \overrightarrow{BF} \overset{(a.1)}{=} \boxed{\overrightarrow{AF} - \overrightarrow{AB}}$$
  
</details>

**d) $\overrightarrow{BG}$**

  
$$\tag{d.1} \overrightarrow{BG} = \overrightarrow{BC} + \overrightarrow{CG}$$

$$
  \begin{alignat}{1}
  \overrightarrow{BC} &=  &\overrightarrow{BA} + \overrightarrow{AC} \\
  \tag{d.2}           &= -&\overrightarrow{AB} + \overrightarrow{AC}
  \end{alignat}
$$

$$\begin{alignat}{1}
  \overrightarrow{CG}       &=  \overrightarrow{BF} \\
  \tag{d.3} &\overset{(a.1)}{=} \overrightarrow{AF} - \overrightarrow{AB}
  \end{alignat}
$$

$$\begin{alignat}{1}
  \overrightarrow{BG} &\overset{(d.1)}{=} &\overrightarrow{BC}                        &+ &\overrightarrow{CG} \\
                    &\overset{(d.2)}{=} &-\overrightarrow{AB} + \overrightarrow{AC} &+ &\overrightarrow{CG} \\
                    &\overset{(d.3)}{=} &-\overrightarrow{AB} + \overrightarrow{AC} &+ &\overrightarrow{AF} - \overrightarrow{AB} \\
  \end{alignat}
$$

$$\overrightarrow{BG}=\boxed{-2\overrightarrow{AB} + \overrightarrow{AC} + \overrightarrow{AF}}$$
  



**e) $\overrightarrow{AG}$**

Repetido em (b)

**f) $\overrightarrow{AB} + \overrightarrow{FG}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
  $$
    \tag{f.1}
    \overrightarrow{FG} = \overrightarrow{BC}
      \overset{(d.2)}{=} -\overrightarrow{AB} + \overrightarrow{AC}
  $$

  $$
    \overrightarrow{AB} + \overrightarrow{FG}
      \overset{(f.1)}{=} \overrightarrow{AB} - \overrightarrow{AB} + \overrightarrow{AC}
      = \boxed{AC}
  $$
</details>

**g) $\overrightarrow{AD} + \overrightarrow{HG}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
  $$
    \overrightarrow{AD} + \overrightarrow{HG}
      = \overrightarrow{AD} + \overrightarrow{DC} = \boxed{AC}
  $$
  
</details>
  


**h) $2\overrightarrow{AD} - \overrightarrow{FG} - \overrightarrow{BH} + \overrightarrow{GH}$**

<details>
  <summary>Clique para revelar a resposta</summary>
  
$$
\overrightarrow{AD} = \overrightarrow{EH} = \overrightarrow{FG}
  = \overrightarrow{BC} \overset{(d.2)}{=}
  -\overrightarrow{AB} + \overrightarrow{AC}
$$

$$\begin{alignat}{1}
BH                 &=&   &BA + &AE +        &EH \\
                   &=&  -&AB + &BF +        &BC \\
   &\overset{(a.1)}{=}& -&AB + &(AF - AB) + &BC \\
   &\overset{(d.2)}{=}& -&AB + &(AF - AB) + &(-AB + AC) \\
                   &= &&&&-3AB + AC + AF
\end{alignat}$$
  
</details>



ARRUMAR

$$
BH =   BA +  AE       +  EH
   =  -AB +  BF       +  BC
   =  -AB + (AF - AB) +  BC
   =  -AB + (AF - AB) + (-AB + AC)
   = -3AB + AC + AF
$$

$$GH = BA = -AB$$

$$2AD - FG - BH + GH = 2(-AB + AC) - (-AB + AC) - (-3AB + AC + AF) + (-AB)
  = \boxed{AB - AF}$$


## Exercício 2

## Exercício 3

## Exercício 4

## Exercício 5

## Exercício 6

## Exercício 7

## Exercício 8

## Exercício 9

## Exercício 10

## Exercício 11

## Exercício 12

## Exercício 13

## Exercício 14

## Exercício 15

