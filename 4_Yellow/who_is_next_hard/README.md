問題文
=====

(難易度目安 : $600$点)

自然数$M$が与えられた時、$0$以上 $1$以下であり、分母が$M$以下であるような規約分数を小さい順に並べた結果得られる数列を$F_{M}$と定義します。

例えば、

$F_2$ = $\{0,1 / 2,1 / 1\}$

$F_4$ = $\{0,1 / 4, 1 / 3, 1 / 2, 2 / 3,3 / 4,1 / 1\}$

です。


自然数$T$が与えられます。

以下の$T$個のクエリに解答してください。

---

◎自然数$M$と互いに素な自然数のペア$(p,q) (p < q)$が与えられる。

分数$\frac{p}{q}$は$F_M$の要素かつその$K$番目の項であるとする。

$F_M$の$K + 1$番目の要素を$\frac{u}{v}$と表すとき、自然数のペア$(u,v)$を求めよ。


制約
-----

・テストケースは$T$個与えられる。

・$1\le T \le 10^{4}$

◉全てのテストケースに対して以下が成り立つ。

・入力はすべて正の自然数

・$1\le M \le 10^{9}$

・$p < q$かつ$\frac{p}{q}$は$F_M$の要素である

入力
-----
はじめに$T$ = (テストケースの数)が与えられる。

その後$T$回にわたって,$i(1 \le i \le T)$番目のクエリが与えられる。

各クエリは以下の形式で与えられる。
```
M
p q
```
テストケース全体での入力は以下で与えられる。
```
T
M_1
p_1 q_1
M_2
p_2 q_2
.
.
.
M_T
p_T q_T
```

出力
-----
全部で$T$行出力してください。

$i$行目には、$i$番目のクエリの自然数のペア$(u,v)$を出力してください。

最後に改行してください。

サンプル
=====
```入力1
4
2
1 2
6
4 5
7
2 3
6
3 5
```

```出力1
1 1
5 6
5 7
2 3
```

$1$つめのクエリにおいて、$F_2$ = $\{0,1 / 2,1 / 1\}$を見ると、$\frac{1}{2}$の次は$\frac{1}{1}$です。

```入力2
4
726
45 188
885
181 205
305
169 282
62
37 41
```

```出力2
152 635
626 709
172 287
28 31
```

```入力3
4
705114717
590136178 616807693
400822285
8708089 86329833
808186475
236869257 466568537
394895154
99700898 208593159
```

```出力3
415141047 433903565
35546168 352395887
238027112 468849199
139333797 291512689
```