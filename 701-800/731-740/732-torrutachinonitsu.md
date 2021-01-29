# 732 : トロールたちの肩に立つ

$$N$$人のトロールが深さ$$D_n$$cm の穴の中にいる。$$n$$番目のトロールは以下の特徴を持つ。

* 肩までの身長$$h_n$$cm
* 腕の長さ$$l_n$$cm
* IQ（Irascibility Quotient, 短気指数\) $$q_n$$

トロールたちは下にいるトロールの肩の上に立つことにより、積み上がることができる。一番上のトロールの手が地表に届いたとき、そのトロールは穴から脱出できる。脱出できたトロールはこの脱出作戦にはもはや関与できなくなる。

トロールたちは、脱出するトロールのIQの合計$$Q(N)$$を最大にするように最適の作戦を立てる。

トロールたちの特徴は以下の式で与えられる。

$$r_n = ((5^n \mod (10^9 + 7)) \mod 101) + 50$$  
$$h_n = r_{3n}$$  
$$l_n = r_{3n+1}$$  
$$q_n = r_{3n+2}$$  
$$\displaystyle D_N = \frac{1}{\sqrt 2} \sum_{n=0}^{N-1} h_n$$

たとえば、最初のトロール$$(n=0)$$は肩までの身長51cm、腕の長さは55cm、IQ は75である。

$$Q(5)=401, Q(15)=941$$である。

$$Q(1000)$$を求めよ。

\(\* $$r_n$$の式、最外のカッコが$$[ \dots ]$$なのだけど多分$$[ \{ ( \dots ) \} ]$$なだけで特別な意味はなさそうなので、誤解のないように丸括弧に揃えた。違っていたらごめんなさい。\)
