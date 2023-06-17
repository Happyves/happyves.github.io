---
layout: post
title: The Combinatorial Nulstellensatz, a note on the final argument.
date: 2023-06-17
tags: math
categories: sample-posts
related_posts: false
---

This is a note on the proof of the combinatorial Nullstellensatz as it's written in the proof of Theorem 16.8 of the second editin of S. Jukna's "Extremal Combinatorics".

It's also my first blog-post using MathJax.



Here's why "it is impossible to have such a monomial on the right-hand side".


The monomials on the left-side of the equation have form $$ (a_1 ,..., a_i +j,..., a_n ) $$, where $$ (a_1 ,..., a_n ) $$ is a monomial of $$ h_i $$ and $$ j \leq \vert S_i \vert $$, corresponding to the monomials of $$ g_i $$. Now, if one of them was $$ (a_1 ,..., a_i +j,..., a_n ) = (t_1 ,..., t_n ) $$, then since $$ a_i \geq 0 $$ and $$ t_i < |S_i | $$, we must have $$ j < |S_i | $$. However, the product of monomial $$ (a_1 ,..., a_n ) $$ of $$ h_i $$ and the leading monomial of $$ g_i $$ will produce monomial $$ (a_1 ,..., a_i +|S_i | ,..., a_n ) $$, which must be in $$ f $$. This is a contradiction on the degree of $$ f $$, since $$ deg(f) = t_1 +...+ t_n = a_1 +...+ a_i +j+...+ a_n \leq a_1 +...+ a_i +|S_i | +...+ a_n $$.



