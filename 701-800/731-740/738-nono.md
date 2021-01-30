# 738 : 昇順の因数分解の個数

$$n$$を$$k$$個の昇順の整数の積で表す方法の個数を$$d(n, k)$$とする。

$$n = x_1 \times x_2 \times x_3 \times \dots \times x_k \hspace{2em} x_1 \leq x_2 \leq \dots \leq x_k$$

さらに、$$D(N,K)$$を$$1 \leq n \leq N, 1 \leq k \leq K$$における$$d(n, k)$$の和とする。

$$\displaystyle D(N,K) = \sum_{n=1}^N \sum_{k=1}^K d(n,k)$$

$$D(10, 10) = 153$$, $$D(100, 100) = 35384$$である。

$$D(10^{10}, 10^{10})$$を$$1\,000\,000\,007$$で割った余りを答えよ。

