---
layout: page
title: from highschool to uni
description: A description of the differences between math at highschool and math at uni, with some advice on how to succeed in uni.
img: assets/img/Blog_HighschoolUni_logo.png
importance: 1
category: Blog
---

<head>
   <style>
       .center-container {
    display: flex;
    justify-content: center;  /* Horizontally center */
    align-items: center;      /* Vertically center */
    height: 750vh;            /* Use 100% of the viewport height */
}

.centered-image {
    max-width: 100%;          /* Ensure the image doesn't exceed its container */
}
   </style>
</head>


This post is dedicated to highschool students that want to study maths at university. At the end of this post, you'll find a list of book recommendations that may be useful to anyone.

## Why this post ? Why read it ?

I was in this situiation a while ago. I thought that the description given by teachers and older siblings of freinds of mine were enough information to judge the situation. In retrospect, I would have prefered to know what I'll tell you in this blogpost, which I wasn't told or failed to understand.
If you're a highschool student reading this, you've already done something right that I hadn't: you've seeked proper information.

## Learning by doing

In that philosophy, a good advice on how to find out what university math is like, is to show up a university for a day, and/or to read university level textbooks. Many universities hold sepcial events that allow future students to join university level classes for a day or two. In them, you won't really get a feel for what university level math is like, as either the topic is too advanced for you, or it's tailored for highschool students and doesn't reflect the actual contents of the classes. However, you get a good feeling for what lectures (content sessions) and tutorials (exercise sessions) are like. If the lecturer and the tutor where helpful, then you were lucky. Usually, both are a lot bussier then your highschool teachers, and both are usually worse at explaining math too. This is because their main interest is in research, not teaching, and the fact that good teaching isn't rewarded careerwise. It's likely, you just won't find the same dedication for teaching your highschool teachers had.

A good option to learn what university math is like is to work through the first few chapters of some textbooks.
You can access those for free in the university library (often, you may come in the library without being a member of the university, or at least, no one will check), or find sripts of lectures and exercise sheets online on the professors and tutors websites.
In this blogpost, I will advocate learning from books. The problem with this method is that you have no one to ask questions to when reading them, but its advantages are that you can take as long as you like to read them, and they usually contain more information then the scripts of professors lectures (which often cover a subset of the books content anyway).
When reading the first few chapters of one of these textbooks, one of which should be on linear algebra and the other on analysis, you can see how this method works out for you.
However, don't be to hard on yourself if you strugle with the content of these books: it might not be the method of learning from books, nor the quality of the books that's causing you trouble, but simply the fact that university math is quite different and quite harder then highschool math. 

## The difference between uni math and highschool math

You will note that university math is about writing proofs and solving problems that aren't necessarily of a calculatory nature.
When I first heard this claim, I didn't quite belive it or understand it. This why I will give some examples of proofs to illustrate what I mean.

#### Non-calculatory proofs

A not too calculatory proof you may have already encountered in highschool is the irrationality of $$\sqrt 2$$.
We show that the contrary is impossible, so we show that there are no integers $$a,b$$ such that $$2b^2 = a^2$$ (an equivalent way of stating that $$\sqrt 2$$ is rational) by deriving contradiction from assuming that there actually are such numbers.
We start by noting that $$2b^2 = a^2$$ implies that $$a^2$$ is even, which can only happen when $$a$$ is even.
Indeed $$(2k+1)^2 = 2(2k^2+2k) +1$$, so that sqaures of odd numbers are odd, and $$(2k)^2 = 2(2k^2)$$, so that squares of even numbers are even, hence $$a=2q$$ must be even.
But then $$2b^2 = a^2$$ becomes $$b^2 = 2q^2$$ so that by the same argument, $$b$$ is even as well.
This causes a contradiction when the numerator $$a$$ and the denominator $$b$$ of the fraction we chose to represent $$\sqrt 2$$ are coprime, so that they have no common factors other then $$1$$, as even numbers have common factor $$2$$.
Now, all fractions can be represented by a coprime numerator and the denominator (cancel all common factors in a given representaton), so to avoid contradiction, the assumption that $$\sqrt 2$$ was rational must have been false.

This proof still contained some computational elements, such as the parity of squares.
You will encounter proofs that contain little to no claculational arguments at all, such as that of the Bolzano-Weierstrass theorem.
This theorem says that a sequence $$(u_n )$$ of real numbers with values in some bounded interval $$[ a,b]$$ will always contain a convergent subsequence.
The idea is that either $$[ a,(a+b)/(2)]$$ or $$[(a+b)/(2) , b]$$ contains infinitely many terms of the series.
If we choose $$v_1$$ to be a $$u_m$$ in the interval among the two that contains infinitely many terms, we can apply that argument again on the subsequence $$u$$ starting at $$m+1$$ that takes values in that interval.
We will contruct a subsequence of $$u$$ that will be in smaller and smaller intervals (they get halved at each step), and will therefore converge.
My exposition involved quite some handwaving (= mathematicall slang for leaving things unexplained), and you will find a better exposition in analysis textbooks.
What I wan't you to note is that not a single calculational trick showed up in this proof: it was purely ideas and properties.

#### Problem solving

Next, I want to introduce you to problem solving.
You will be asked to solve problems who's solution involves non-obvious application of one - and often multiple - results you'll have seen in class.
In highschool problems, it's quite easy to tell which theorem from class is to be used in an exercise, at least from the perspective of a university sutdent.
This is not the case for university exercises, in which a lot more innovative steps are required to reach the solution.

An example for this is the following problem: show that for any five points in a unit length square, there is at least a pair that is at distance at most $$\sqrt 2 /2$$.
Try to solve this one before reading the solution that follows.

The idea is to subdivide the square into 4 squares by cutting it along its egde midpoints.
For five points, two of them will end up in the same sub-square.
The largest distance two points can be at in such a sub-square is the length of the sub-squares diagonal, which you can compute to be $$\sqrt 2 /2$$.

The step of subdividing the square in 4 required some initiative from your part.
It's not a technique you will learn in a combinatorics class, where this type of exercise could be asked of you.
It is, even at an advanced level, quite difficult to solve problems that require a lot of originality, so don't feel bad if you didn't get this one.
This example illusrates (or is supposed to illustrate) the fact that problem solving requires a lot of creativity.
You will get better at this over the years, but your beginings will be quite rough.

An unfortunate thing is that university math classes often make no attempt at explaining how the ideas for showing a problem or even a result from class are to be reached.
After all, it's quite difficult to explain how you got an idea, isn't it ?
However, I encourage you to read books that attempt to adress this.
The least I encourage you to do, is to - whenever you have an idea or read a proof - try to find what it is that pushed you or the author of the proof to take the steps you/they took.
I'm conviced this helps your brain make connections between mathematical objects more easily.

Another way of getting good at problem solving is to solve a lot of problems, or in general, to read a lot of math. Though, I think it's always best to try a exercise yourself before reading the solution, if its provided.
I'm no neuroscientist, but I think the bodybuilder wisdome "no pain, no gain" applies in some sense. You have to push your brain to get used to making connections and long searches.

A side effect of this is that uni math can be quite hard and quite frustrating.
It will often happen that you'll get angry at yourself and ask : why didn't I think of this ?
Don't let these moments drag you down. They happen to highly competent professional mathematicians all the time.
However, if you dislike these moments too much then math may not be for you, and there is no shame in that.
Working on problems all day does not create a sane environnement: you should compensate with a good amout of social life, sports and hobbies.

#### Formalism

Another difference between highschool and uni math is formalism.
At uni, math is written in a language that may feel almost like a programming language.
In fact, if you check my projects on this website, you can find the Lean projects, in which I present Lean, a programming language for formal verification of mathematicl proofs.

To illustrate this, we'll take the example of the fact that there are $$n\times (n-1) \times ...\times 1$$ ways to order $$n$$ different objects.
A proof of this you may have gotten in highschool may have been based on a diagram such as the following one.


<div class="center-container">
    <img src="{% if site.baseurl %}{{ site.baseurl }}{% endif %}/assets/img/Blog_HighschoolUni.png" alt="Your Image Description" class="centered-image">
</div>


It represents the possible orderings as paths determined by successive choices of what object to place on spot $$k$$ in the ordering, starting from spot $$1$$ where we have $$n$$ choices, to spot $$2$$ where we have $$n-1$$ choices for the second object (all but the first object are candidates), and so on.

At uni, this will be shown by induction.
I was taught induction in highschool, but in case you weren't, I'll quickly explain it.
To show some property depending on a natural number $$n$$ is true for all such natural numbers, we can show that it's true for $$n=0$$ (or $$n=1$$ depedning on where you consider natural numbers to start), and that when it's true for $$n$$, then it's also true for $$n+1$$.

In our formal proof of the fact that there are $$n\times (n-1) \times ...\times 1$$ ways to order $$n$$ different objects, we will first explain what it means to order objects.
For our purposes, think of an ordering as an association of spots with objects that is one-to-one: we associate one spot to one object exactly.
We then use induction on the number of objets.
If there is just one object, there is $$1$$ way to associate it to the single spot, so the property is true in that case.
For the so-called induction step, we consider $$n+1$$ objects.
Associations can be partitioned into $$n+1$$ sets of assocations, depending on which object they place in the first spot.
On each such set, when we look at what the association does with the other $$n$$ spots, we note that they can be considered as associations of $$n$$ objects.
So we know by the fact that the property is true for $$n$$, that all these $$n+1$$ sets have size $$n\times (n-1) \times ...\times 1$$, so that there are $$(n+1)\times (n \times ...\times 1)$$ associations in total, which is precisely the property for $$n+1$$.
So we conclude by induction that the property is true for any number of objects.

This proof may have fealt like a strange reformulation of the idea behind the previous picture.
Or it may have sounded nonsensical, which wasn't my intent, but is how far I can go in discussing formalism without develloping actual formalism.
The moral of the story is that at uni, especially in the first semesters, loose arguments or diagrams, or even good arguments won't be enough: you'll be asked to write formal proofs.

Formalism is, in my opinion, misunderstood.
It's not there to annoy you. It's an attempt at creating the highest proof standard that leaves no place for ambiguity, to the point of being mechanically checkable (and painfull to read for humans).
I encourage you to think of it as a programming language: you have to talk to the computer in that pendatic way, because it doesn't know better, it's just a buch of circuits.

Paradoxically, in contrast to the formalism you'll be asked to learn in the first semesters, most professors frequently skip explanations, arguments, whole/parts of proofs in their classes.
They do this either to gain time or because they can't relate to students anymore and can't therefore imagine that student can't - or can only with much effort - fill in the missing explanations.
I recommend trying your hardest to fill out the parts left out by your profs. It makes for a good exercise and will even help you memorize the class content.
Also, again, don't feel bad if you take a long time to fill in these parts, or fail to do so: remember that you're still a beginner.

## My advice

Now that you've seen the difference that universtity math has to highschool math, you should be thrilled to start your studies, as this uni type math is much more exiting than the highschool math, but you should also be worried about how well you'll perform at uni type math.
This blog-post is here to give you some advice on how to succeed at studying math at uni.

#### Options

My first advice is to explore your options whenever you're given any.

The first choice you'll make is deciding where to study.
As you can check in my CV, I've studied both in France and Germany.
My experience is that the differences educational systems have is astounding.
They have advantages and disadvantages, and I recommend you consider studying abroad, if you have the capability for it, and you prefer a different educational system then your native one.

Some advantages of the french system (or at least from math at the university of Strasbourg) over the german one are that you're guided quite well in your first semesters: what the germans will try to shove into you in a year in terms of analysis and algebra is often spread over two years in french unis.
Some advantages of the german system (or at least from math at the universities of Bonn and Berlin) over the french one are that you can take as long for you degree as you like, which allows you to have a job besides your studies.
This is just an example. Of course, advantages and disadvantages are a question of taste, but I'd just like to point out that differences between systems exist.

Another aspect of choosing where to study is prestige. Let's face it, you've probabily looked at a uni ranking at some point or another.
It is a difficult question to answer whether this truely matters. I'm actually don't have an answer I can fully get behind for this.

Other options you'll have to choose from are subjects. This may depend on the educational system you're in: I rememeber there being relatively few choices of classes to take in Strasbourg, and quite a lot of choices at an early stage in Bonn. My advice is to try out all areas of math before specializing. There might be areas you haven't heard of, or that you've been given a bad treatement of and may actually enjoy if done right. I remeber being fairly interested in dynamical systems and differential geometry before discovering discrete math, which I came across almost accidentally, after taking an obligatory class in Bonn. I've now specialized in discrete math and I'm confident I made the right choice in doing so.

#### READ BOOKS !

The next choice you'll have is to chose a learning resource for each of your classes.
Indeed, there is more then just the lecturer's script amd the tutor's exercises you can learn from.
Some books will contain more content, more explanantions and even better explanations then other books or your teachers script.
At the end of this post, I've included a bunch of good books you can look at.
It may seem difficult to believe that this choice has a great effect on your understanding of the subject.
But a good book will contain complete information that it places in a context, it will even anticipate some common errors students make and point them out for you, it will illustrate the information for you, and finally train you with exercises that follow a learning curve, providing you just with the right difficulty level one exercise after another.
If you learn with a bad resource, you'll quickly be confused, you'll waste time trying to complete or arange the scattered information, you won't understand why your learning this subject, and you'll gain nothing from exercises that are either to simple or too difficult.
Trust me when I say that learning with a good resource makes the whole difference.

The downside of not strictly following your lecturers notes is that you'll have to find the time for reading the other resources and that you'll have to synchronise notations, contents and order of contents between the resources.
In my opinion, this is worth the price.

#### Applied math

The choices of teaching content aren't in our favour if you like applying math to the real world.
Professors are either not intereseted in applications of their work, sometimes even applications within math itself, or they don't want to waste time on teaching about applications, as mathematical content is more important in a lecture.
To remedy this, I can only recommend finding the applications yourself. You can search the internet for them, or flick through books on disiplines from the natural and social sciences and look at the math they use, until you find a field that uses the type of math you're intersted in, and then read about this area.

I like applied math. In case you don't, I must warn you that even in academia, finding jobs where you work exclusively on pure math is becoming increasingly difficult, as these positions get increasingly rare. So you maximise you chances at a good job, either in or outside of academia by looking into application areas of math.

#### And most importantly

"Mens sana in corpore sano". Meet freinds, do sports, enjoy life. You will face a lot more and work and stress at uni then you did in highschool.
The best way to handle this is to maintain the life-work balance !

# Book recommendations

Here are my book recomendations for undergraduates (Bachelor/Licence level).
These are books I would recommend.
There may be other fantastic books that I haven't come across.
This list just happens to be those books I read (partially), enjoyed, and remembered to put in this list.
In fact, you may recognize a certain bias towards discrete math in the list, which due to it being my field of expertise.
I highly recommend you to read these books, even if the contents aren't part of lectures provided by your university: they are a joy to read.

## Appetizers 

Good to read before a lecture or to find out about a field.

#### Discrete math:

* A Beginners Guide to Discrete Mathematics by W. D. Wallis
* The Fascinating World of Graph Theory by Arthur Benjamin, Gary Chartrand, Ping Zhang

#### Algebra:

* Elements of Algebra Geometry, Numbers, Equations by John Stillwell
* Elements of Number Theory by John Stillwell

#### Analysis:

* Calculus Concepts and Contexts by James Stewart
* A Radical Approach to Real Analysis by David Bressoud

#### Geometry and Topology:

* Geometry by D. Brannan, M. Esplen and J Gray
* The Knot Book by Colin Adams

## Main courses 

* Good to accmpany lectures, so as to better understand their content.

#### Discrete math:

* Discrete Mathematics by László Lovász, József Pelikán and Katalin Vesztergombi
* Discrete Mathematics by Martin Aigner
* Invitation to Discrete Mathematics by Jiří Matoušek and Jaroslav Nešetřil
* Olympiad Combinatorics by Pranav A. Sriram
* Concrete Mathematics A Foundation for Computer Science by Ronald L. Graham, Donald E. Knuth, Oren Patashnik

#### Analysis:

* Advanced Calculus A Geometric View by James Callahan
* Petit guide de calcul différentiel à l'usage de la licence et de l'agrégation by J. Rouvière.

#### Stochastics:

* The Theory of Probability by S. Venkatesh

#### Geometry and Topology:

* Elementary Differential Geometry by Christian Bär
* Differential Geometry of Curves and Surfaces by Kristopher Tapp

## Desert 

Good to accompany or to close off lectures, to learn about advanced topics usually not covered at the undergraduate level, though they should for so many reasons:

#### Discrete math:

* Thirty-three Miniatures Mathematical and Algorithmic Applications of Linear Algebra by Jiri Matousek
* The game of cops and robbers on graphs by Anthony Bonato, Richard J. Nowakowski
* Game Theory A Playful Introduction by Matt Devos, Deborah A. Kent
* Discrete and computational geometry by Devadoss S., ORourke J.
* Algorithm Design by Jon Kleinberg, Eva Tardos
* Extremal Combinatorics With Applications in Computer Science by Stasys Jukna
And at least one of:
* Graphs Digraphs by Gary Chartrand, Linda Lesniak, Ping Zhang
* Graph theory by Adrian Bondy, U.S.R. Murty
* Graph Theory by Reinhard Diestel

#### Algebra:

* Ideals, varieties, and algorithms an introduction to computational algebraic geometry and commutative algebra by David A. Cox, John Little, Donal O’Shea

#### Analysis:

* Differential equations, dynamical systems, and an introduction to chaos by Robert Devaney, Morris W. Hirsch
* Nonlinear Dynamics and Chaos by Steven H. Strogatz
* Robert L. Devaney - An Introduction To Chaotic Dynamical Systems

#### Geometry and Topology:

* Knots and links by Peter R. Cromwell
* Geometry by Its History by Alexander Ostermann, Gerhard Wanner
* Tristan Needham - Visual Differential Geometry and Forms A Mathematical Drama in Five Acts

