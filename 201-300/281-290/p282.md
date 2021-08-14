# 282 : アッカーマン関数

非負整数$$m, n$$に対し、アッカーマン関数$$A(m, n)$$は次のように定義される：

$$A(m,n) = \left \{ \begin{array}{ll} n + 1 & \textrm{if} \; m = 0 \\ A(m-1,1) & \textrm{if} \; m > 0 \land n = 0 \\  A(m-1,A(m,n-1)) & \textrm{if} \; m > 0 \land n > 0\end{array} \right .$$

例えば$$A(1, 0) = 2, A(2, 2) = 7, A(3, 4) = 125$$である。

$$\displaystyle \sum_{n=0}^{6} A(n, n)$$を求め、$$14^{8}$$で割った余りを答えよ。

