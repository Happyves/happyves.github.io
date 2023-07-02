---
layout: page
title: Automated Theorem Proving with Lean
description: Formally verifying proofs with the lean programming language, with a glimpse of how this may be automated.
img: assets/img/projects_lean_logo.png
importance: 1
category: Current
---

When writing a proof, applying lemmata or theorems may feel like applying a function. The assumptions would be the inputs of that function, and its output would be the conclusion of the lemma/theorem.

In the field of formal proof verification, this idea is implemented a programming language. One such language is [Lean](https://leanprover-community.github.io/). To get a picture of what Lean looks like, a good way is to play Kevin Buzzards [natural numbers game](https://www.ma.imperial.ac.uk/~buzzard/xena/natural_number_game/).

Here's what Lean looks like in practice. The code is to the left, and to the right, the VS code extention for Lean allows us to get messages from the compiler.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Blog_lean_proof.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

Consider the first example, which states that the complement of a union of sets is the intersection of the complements of these sets. Below the statement is the formal proof, which may look incomprehensible, but is actually a classic proof of set identities, where we take an element of one set and show that it's contained in the other, un-/folding definitions of union, intersction, and complements.

In the info-view to the right, we're told which stage of the proof we're at, with the current assumptions and known facts at the top, and the current goal that remains to be proved at the bottom. In the figure, the cursor is at the part of the proof in which we have to show the second inclusion used to show equality of sets.

Lean has a mathematical library named mathlib, in which mathematical concepts are built and shown from very basic axioms, and that we may use to prove more complicated math. Lemmata and theorems are given particular names, which are needed every time we want to use them in a proof. A first step of automation in formal proof verification is the following:

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Blog_lean_libsearch.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

The property we want to show has already been implemented in mathlib, and the command initating a library search will point us to it in the info-view.

At the current stage, this isn't very impressive automation, but it's still useful. You want to know if certain assumptions imply certain conclusions ? Imagine a very complete mathematical library in which many theorems have been implemented. Then with a quick library search, you could check if your assumptions imply your conclusions and get a link to a proof.

However, we can dream of better automation. What if we allowed the library search to use an itermediate step ? We could search for all properties who's assumptions are those we queried, then search if among their conclusions, there were some that implied our queried conclusions, with another search. What if we add deeper layers of intermediate results ?

This is where the theoretical aspects of automated theorem proving start showing up. Are there efficient algorithms for handling this huge search space ? What if we use data from mathlib to guide these searches with some notion of likelyhood of where to search for intermediate steps ?

At this stage, there are few advances on these questions, but they are quite fascinating, and I hope you are as thrilled to hear of them as I was.

An example of some automation is the so called simp tactic. In our running example, in the lemma, it allows us to prove the same result almost instantly. This isn't cheating! The tactic does the same hard work we did in the first example, but this work has been automated. On the right of the following figure, we can see what exactly simp did, as we're shown the proof that simp built.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/blog_lean_simp.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

A good chunk of math has already been implemented in Lean, as you can tell from the libraries [mathlib](https://github.com/leanprover-community/mathlib) and [mathlib4](https://github.com/leanprover-community/mathlib4). The library is however just the top of the iceberg. Many more results have been implemented in Lean and can be found on their producers personal repositories.

My goal is to learn Lean. I'll then write a tutorial on Lean and mathlib that I'll post on this project page. To put my knowledge to practice, my goal is to implement proofs from [Proofs from THE BOOK](https://link.springer.com/book/10.1007/978-3-662-57265-8) by Martin Aigner and Günther Ziegler. Perhaps, I'll also implement proofs from combinatorial optimization, discrete geometry and positional game theory. This will be done in the context of a Masters thesis supervised by [Christoph Spiegel](https://christophspiegel.berlin/).
