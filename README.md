<style>
.bjimg{
  position: fixed;
  top: 0;
  left: 0;
  width:100%;
height:100%;
min-width: 1000px;
z-index:-10;
zoom: 1;
  background-image: url();
  background-repeat: no-repeat;
  background-size: contain;
  background-position: center 0;
  opacity: 0.3;
  }
</style>
<head>
<script src="https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML" type="text/javascript"></script>
    <script type="text/x-mathjax-config">
        MathJax.Hub.Config({
            tex2jax: {
            skipTags: ['script', 'noscript', 'style', 'textarea', 'pre'],
            inlineMath: [['$','$']]
            }
        });
    </script>
</head>
<div class="bjimg"></div>

# 因为开学了不知道写什么所以整一个烂活其实是为了祈祷问题有进展以及明天天气再暖和点吧

<font size="2" color="grey">发布于2024.2.28</font><br/>
> **“定理”.** 所有自然数都是有趣的.

*证明*. 用反证法. 假设所有无聊的自然数构成的集合$B$非空，那么由最小数原理$B$有最小数，记为$n$. 但是**$n$是最小的无聊自然数**真的很有趣，与$n\in B$矛盾！所以所有自然数都是有趣的. $\Box$

笔者其实想强调最小数原理的好处(集合论学者更喜欢称其为**良序原理**)，贴一个严格证明和一个应用.

> **最小数原理** 任意一个自然数的非空子集都存在最小数.

*证明*. 任取$\mathbb{N}$的非空子集$S$，构造

$$
L:=\{ n\in\mathbb{N}: n\leq a, \forall a\in S\}.
$$

首先$0\in L$，因为所有自然数都大于等于$0$(自然$L$非空)；同时$L\neq \mathbb{N}$，因为对任取$a\in S$，$a+1\notin L$. 所以一定存在$n_0\in L$使得$n_0+1\notin L$，否则数学归纳法(Peano公理)给出$L=\mathbb{N}$从而导致矛盾. 我们断言$n_0$就是$S$中的最小数，因为$n_0\in L\Rightarrow n_0\leq a, \forall a\in S$；同时$n_0+1\notin L\Rightarrow $存在$k\in S, k<n_0+1$，联合前一个结论可得$n_0=k\in S$，所以最小数存在. $\Box$

> **练习.** 用最小数原理证明每个自然数都可以分解为若干素数的乘积(即质因数分解的存在性).

<br/>
[<font size="3">少女祈祷中...</font>](https://senyuyangpdelearner.github.io/)

