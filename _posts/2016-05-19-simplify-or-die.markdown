---
published: true
title: Simplify or Die Retrying
layout: post
---
Have some years that I started with ERPNext, I worked in smalls, mediuns and now in a biggest project of customization of ERPNext, and on each new project, I fell that the things should be simplified!

The major issue is: The actual cicle of development is not able to scale! Code requires humans to code, and the most important not only simple humans, code requires programmers to touch with it.

Is very hard turn ideas in a real product, and in the major of times, the customer is not sure about what him really need! And the most important, code is not able of do everything! _Alan Turing_ describe what is computable and what is not, so basically, we have goals that are unreacheable by code!

Is because these issues, and the fact that code, takes too much of my time, that I started developing a project to save my professional life!

I started this project a year ago, I touch in the code too many times, without success to go ahead, and XKCD, have a nice visual description about why:

![Where I'm failling](http://imgs.xkcd.com/comics/automation.png)

The automation of code development, is not a simply task! It requires months of research, years of thoughts, a bit of luck and really patience! Too much patience!

_CoreFlow_ is the result of my last 8 years coding, after too much time, taking my focus in the code, and never changing my coding language (except from VB6 to Python 6 years ago) after these time, I fell that I'm full able to formulate some theories about the process of coding!

In my basic theory, I observed that:

# 1 - Code is too much inflexible to represent the real world!

Yes, this is a truth, being active in the process of development and customization of *ERPNext*, I understood that the code, is not the best way of represent the real world, this is because the code is inflexible! This is the nature of the code,  of a computer, of a program! You never can expect that a ERP made in India, will understand how the things are in Brazil, but you ever expect that a calculator returns 2 if you enter 1+1!

In fact __Accounting__ is __accounting__ everywhere, but the real words, affects directly the accounting! Since __Accouting__ is a [*Applied Social Science*](https://irresistibledisgrace.wordpress.com/2010/01/13/accounting-as-social-science/), it will be directly affected by the society!

# 2 - Code affects the real world, as the same way that the real world affects the code!

Do you can imagine a world without Internet, Google, Youtube, Wikipedia? If the code had never existed, the digital revolution never would have happened, so in the same manner that we try to represent the real world in lines of code, these lines of code, are current in our lives in the real world - This is recursion issue!

# 3 - The nature of inflexibility of the code is in the bit!

How do you know, computers are ruled by  sets of bits, each bit only can represent one of two states (on-off, true-false, 0-1 etc) and daily we talk about things that _Maybe_, _Will it_, _Yes, will!_ , _No will_, _Never will_, _Sometimes will_, _Everytime will_, etc . Each of these sentences have a contextual weight, that is impossible to represent in a computer due the nature of the math and for the fact that the weight change for each person, in each phase of life or from one society to another!

# 4 - I never will automate the code!

Another truth, that is a complement of the last observations! Due the code is inflexible, and the real world change on every minute, we never will be able of automate the code to generate complex programs that are able to do a full representation the real world! Because the real world change the code, and the code will change the real world!

---------------

A code can be segmented by:

- **Variables:** _Anything that change due a context_
- **Actions:** _Anything that is capable of cause changes_
- **Events:** _Anything that flag that something will occur or happened_
- **Operations:** _The action of observe something_

Returning to the principle of this article, that I started talking about _Alan Turing_, another important basis from him, are the **Finite State Machines (FSM)**.

FSM are the most simple, and most powerfull computers in the world! In fact a computer only runs, because it is a FSM, and the information is _computable_.

Given that a FSM is a basic programable computer, __CoreFlow__ is a Finite state machine, that _observe_ _variables_ to do _actions_!

The _events_ only exists to determine what is going on!

In the next weeks I'll start talking more and more about **CoreFlow**, because this is cause of all my actual headaches, and the solution for that!