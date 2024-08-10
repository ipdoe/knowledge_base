# AMMs

## Constant Product Formula

$x$... Token amount  
$u$... Liquidity amount (USD, ETH, SOL, ...)  
$k$... Constant

$$x \cdot u = k$$

## Pump Fun Math

$LP$... Liquidity  
$MC$... Marketcap  
$Pr$... Price  
$S_\mathrm{T}$... Total Supply  

Subscripts:  
0... Initial  
$n$... Final

### Equations

$$x_0 \cdot u_0 = k$$

$$x_n \cdot u_n = k$$

$$Pr_n = u_n/x_n$$

$$LP_n = 2u_n, \ \ \ \ \ MC_n = Pr \cdot S_\mathrm{T}$$

### Concrete example
$LP_n = 12\mathrm{k}$  
$MC_n = 69\mathrm{k}$  
$S_\mathrm{T} = x_0 =1\mathrm{B}$

Initial seed capital needed to satisfy the above:

$$u_0 \cdot x_0 = k = u_n \cdot x_u \Rightarrow u_0 \cdot x_0 = {LP_n \over 2}\cdot {S_\mathrm{T} \over MC_n}$$

$$u_0 = {LP_n^2 \over 4MC_n}$$

$u_0 = {(12\mathrm{k})^2 \over 4*69\mathrm{k}} = 521.74 \mathrm{usd}$

Resulting LP for given initial seed and final MC

$$LP_n = \sqrt{4u_0 \cdot MC_n}$$

$LP_n = \sqrt{4*550 \cdot 69\mathrm{k}} =  12\ 321 \mathrm{usd}$
