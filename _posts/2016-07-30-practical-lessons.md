---
layout: post
comments: true
title:  "Practical learnings in Machine Learning / AI"
excerpt: "Just some observations from working in the machine learning and AI field."
date:   2016-07-30 00:00:00
---

# Practical Learnings

Math and computer science are only one component of machine learning and AI. Here are a few ideas that I've found pretty important.

**Balances**.

As with most things in life, it's good to keep in mind the idea of balance.

* Research Optimism / Skepticism - The fundamental idea behind the scientific method is skepticism. For example, look at the connotation on how we deal with hypotheses: we don't prove hypotheses; rather, we reject the null hypotheses. We are often wary of results that have not been replicated, no matter how sound the explanation. It's a great skill to be able to take an idea and break it down into its component pieces, understand the logical inconsistencies, and have an intuition on the practical failure modes. Relentless re-evaluation of our own ideas can help us be more precise and create better solutions. But at the same time, I've seen people get so bogged down in a pessimistic/skeptical viewpoint that they fail to see the beauty and progress of intermediate ideas and results. Great potential ideas are sometimes ignored because we were too quick to dismiss them based on small, tangential details.

* Precision / Simplicity - We want to convey our ideas accurately and concisely, and those two aspects can be in direct conflict with each other. Richard Feynman was probably one of the best practitioners of this balance.

* Generality / Specificity - I fall strongly on the side of encouraging generality of the approaches we develop. But I do understand the concern that if you focus too much on generality, the systems you build might not be all that applicable in specific, practical use-cases. However, from experience, I've found that it's not impossible to get the best of both worlds. For example, let's assume there's some "optimal solution" for different applications. Now let's say you have a general solution that achieves 90% relative to the optimal solution on 20 applications. You also have a handcrafted solution that achieves 99% of optimal on one application. When you compare 90% to 99% percent, it seems like you should pursue the handcrafted solution. But when you look at the overall picture, it's more obvious why we should focus on the general solution -- even if it takes more upfront cost.

**It's okay being wrong**.

I'm reminded how stupid I am all the time. We’ve got to be okay with the fact that -- sometime in the near future -- we’re going to find out our current implementations and ideas were obviously sub-optimal. If you can do that, that's a good thing! It means you’re making good progress – the fact that old, hard ideas that lead to real value that were so difficult in foresight could be so obvious in hindsight mean you’re making tangible, buildable progress. Along with that, I think it also helps have a better sense of appreciation. Saying “it’s trivial to do X” belies a lot of the importance and impressiveness of really thinking about and doing X. However, there's also value in being able to distill a big idea into a few fundamental principles -- and understand that the big idea is actually feasible.

**Have fun and be kind**.

I hear a lot about "10X" engineers and scientists, or things about program management efficiency with scrum/agile/whatever. I think this is all secondary to a much simpler principle -- work on things you enjoy, encourage your teammates to work on the things they enjoy, and develop an environment where everyone feels valued and supported. I've learned that most people will surprise you with how capable they are if they're put in a position to do well. Similarly, very intelligent people can perform poorly if they're in an environment that doesn't excite them or encourage them. It takes patience, but if you allow for some freedom and unknowns on deliverables, this can be huge. This aspect is far more important than the specifics of how many lines of code you write, how many papers you read, or what task-tracking structure you use.

**Understand the difference between presentation and underlying meaning**.

This is one of the most fundamental and subtle ideas. I don't think many people have ever been able to 100% perfectly explain an idea they have in their head using just words. There's just too many components, too many dimensions, too many nuances. So sometimes we draw pictures, write equations, act it out, show tabular results, visualize simulations, etc. The key idea here is that it's difficult to take an idea and convey it to others with no transformation or loss of information.

I think understanding that fact -- that presentation is a lossy transformation -- is an important component of learning (and understanding different viewpoints). For example, we've all read academic papers we've disagreed with or that we thought were wrong. Similarly, we've all heard big ideas that we dismiss as "hype with no substance." But we shouldn't just dismiss these ideas -- it's much better to ask, "What are they trying to get at?" Having this approach is so much more powerful -- no matter what you're reading or what you're listening to, you can always learn something new (even if it's not explicitly what the author intended...).

**Don't focus too much on terminology**.

This is related to the balance of precision, and the understanding about presentation. At some level, we need a common framework from which to discuss ideas -- and one good way of doing that is with established terminology. Establishing what the convolution operation is, having named optimizing strategies, etc. -- there's value in having these names have a common meaning among the community. However, I think we fall way too far on the side of strict adherence to terminology.

Take Whorf's "linguistic relativity" hypothesis -- the way you think is partially shaped by the expressibility of the language(s) you know. For example, there may be much better descriptions of an abstract idea or feeling in one language versus another (e.g. what's a good English equivalent of "umami"? How do you describe certain types of body language?). Acknowledging that there are different approaches to an idea is a good thing.

**A big source of creativity is crosscutting ideas**.

I think the more important reason to not be too linked to terminology is that it can hinder creativity. A lot of creativity comes from crosscutting ideas. Here's the irony, though: big ideas go through stages -- at first the big idea sounds crazy, then you start talking about how the idea combines logical things from different fields. At that point, the idea gains a little traction, but the terminology in the different fields makes it hard to see the compatibility. But then if you make it work, and for some reason, that big idea seems obvious and not crosscutting at all.

In other words, you take a new approach not for the sake of being different, but rather, because when framed from the new perspective, it makes creative, useful ideas much more obvious and apparent.

Let's take a pretty powerful example -- computation. People have been thinking about computation for a long time -- long before we had transistor-based computers. Abacuses, mental tricks, algorithmic procedures, inductive proofs -- these all are examples of people thinking about computation without even using a transistor or electricity. In fact, we didn't get Maxwell's equations on electromagnetism until the late 1800s, and we didn't get a modern transistor until Shockley's/Bardeen's/Brittain's in 1947 -- the idea of some electrical contraption performing computation would have appeared crazy for most of history -- why combine the completely different fields of computation and electronics? Yet, now, if someone hears the term "computer," they will invariably think of something electronic like a laptop, PC, or cloud server. What was once a crazy combination of fields turned out to be extremely powerful. (I'll talk about why a crazy crosscutting idea between deep learning and quantum computation isn't that crazy at all in another post).

**Be aware of confirmation bias**.

It's very easy to fall into confirmation biases without realizing it. I see a lot of this in how people describe the history of deep learning, and in explanations of why it has gained so much traction recently. People have been studying neural networks for a long time -- yet the popular support for them has grown in a short period of time. A common explanation for this is that we just didn't have (a) the computational power and (b) a wealth of large, easily available data at the time the neural networks were being developed. This is probably somewhat accurate, but it doesn't give any huge insights on how we push AI further. Instead, we should understand that there are more nuances -- some of which are unrelated to the science -- that contributed to the field's development and impact. And through that, we can find non-trivial ways of making improvements beyond the computation/data scaling.

For example, could the big data and big computation be a red herring for another cause -- namely, that strategic approximations and randomness in networks are important to large-scale learning? Let's say the data grew faster than the computation -- and practitioners wanted to train on the large data, but the computation ability was in a middle ground. The computation could scale to the data if we made approximations -- convolutions only locally connected, reducing parameter and update FP precision, inexact synchronization on distributed systems, etc. Under this view, it wasn't that we finally got computers (FPGAs, ASICs, GPUs, etc.) that were powerful enough for full deep learning. Rather, it was important that our computation was better but still lagged somewhat, which led researchers to be scrappy in how they milked performance on the Pareto curve, and those scrappy approximate tricks actually turned into powerful drivers of progress... Obviously, this is an exaggeration, but I think understanding the nuances of development as more than just "A causes B, which causes C" is valuable to making new progress. Especially considering how much of scientific development is shaped by personal relationships and personal quirks outside of the science.

Another extension of this is in the analysis of how far out general AI is. One of the big arguments is that we need to have artificial neural networks with a number of nodes and connections similar to that of the human brain. Then, from that, we can use transistor development projections to guess when the overlap will happen. I think this analysis is somewhat misguided, as it makes this very linear assumption about "more connections, better networks." What if our learning methods are far less efficient than the human brain? What if they're far more efficient? What if ANNs aren't the best approach for general AI? I'm one of the biggest proponents of deep neural networks, but I'm not too tied to it to think there couldn't be better approaches. Determining whether the alternate approaches really "are different" is more a question of semantics.

**Novelty is subjective**.

As researchers and engineers, we stand on the shoulders of giants before us. And they stood on the shoulders of those who came before them. It can sometimes feel impossible to truly come up with something entirely novel -- that's okay! I don't think I know of any big ideas that were truly 100% novel. Work on things you enjoy, things that are challenging, things that will have an impact if they're successful. Appreciate the work that others before you have done to allow you to be in a place to make further progress.

**A lot of things seem impossible until they aren't**.

This is common in AI -- it's hard to say exactly what we're trying to achieve with AI, so different people come up with different sub-goals that seem difficult/impossible. As these sub-goals are accomplished, we get a moving target, and say that the accomplished sub-goal wasn't actually AI now that we can do it (e.g. solving ReCAPTCHA puzzles, image classification, etc.). Don't get too discouraged if things seem difficult at first!

**We need to be responsible in how we develop AI**.

AI and machine learning are going to be very transformative. Large industries are going to change, and the effects of a transition to more AI and ML systems are going to be widespread. As engineers, scientists, and business leaders involved in this transition, we need to be cognizant of this impact. Moreover, we need to take responsibility and actively educate ourselves on ways we can best use these new technologies for beneficial uses. Just as important, we need to encourage people of all different backgrounds to enter the field -- diversity is key. And with a field that is as data-driven as ML/AI, we need to be very cognizant of the inherent biases in the data that are informing our models.
