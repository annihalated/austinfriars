---
title: Gig work
date: 2026-02-22
draft: true
featured: true
layout: post
url: /gigwork/
description: "How software ate delivery, and what that means for the people delivering"
---

*Disclaimer: Some descriptions here are stylised. The essay is not a work of reporting or original research and should not be read as one. Where I've generalised or compressed for clarity, I've probably  generalised too much. Mea maxima culpa.*

Food delivery generally involves three physical acts:

* the customer orders food
* the restaurant makes the food, and
* a delivery driver gets the food from the restaurant to the customer

If you're a local restaurant, you have a small delivery radius. You might deliver food, but only in your general neighbourhood. The restaurants that started solving the problem of delivery at scale did it through miracles of operational design, given the tools they had.

Domino's, for example, pioneered standardization, centralized commissaries that supplied their kitchens, corrugated pizza boxes, insulated packaging. The kitchens would have large maps of the covered neighbourhoods that delivery drivers would essentially memorise. This was the frontier of adaptation at a time when routing was still manual and GPS maps were not widespread. There was a limit to memorisation, though, and so they added more locations within an existing location's delivery radius. This strategy, called fortressing, was initially ruthless to the franchisees because it cannibalised the existing location's sales. However, at the system level, it made sense to fortress. Each restaurant could make more deliveries and make them quicker. I can't tell the whole story here, but rest assured that they performed miracles of capitalist efficiency.

Dominos was an exceptional firm in its industry. The average restaurant cannot sustain these levels of vertical integration and operational complexity. The restaurant would *like* to have and fulfill more orders. The customers would *like* more restaurants to deliver. There is value in the ether, in the imaginary space of capitalist possibility. There are transactions that *could* happen. There is consumer satisfaction to be produced.

Many people try to capture this value. It might be the guy who buys a motorcycle and starts freelancing deliveries for a few restaurants in his neighbourhood. It might be a small logistics company that literally just supplies drivers to everyone so that more restaurants offer a delivery phone number. The gap exists, and in a competitive market economy, people will try to fill the gaps, if it is profitable to do so.

Let's try. You start by solving for the customers in some part of a city — you make a directory of restaurants who will deliver. This is nice, but you've only solved discovery. You go further, you let the customer order through *one* centralised phone number. But delivery is still the restaurant's problem, and the restaurant is still bad at it. So you go further still, and you supply the drivers, becoming a logistics company. Congratulations, you have separated ordering and delivery from the restaurant.

It's a good business and now you might want to relax. But it's a good business, and this is a market economy, and now you have competitors who will grow even if you don't. "Let them grow," you say, "I will tend to my garden." But you realise soon that the economics of the delivery business gets *so much better with scale* that you are about to lose to a company that is ruthlessly optimising. 

A delivery business at scale will cover more areas, have more restaurants, and have more drivers. Its average delivery time will fall, making customers happier, which will bring in more orders, which will increase your scale further. All of this attracts more restaurants and more customers to join them. A small company covering one neighbourhood is less efficient per delivery than one covering ten. And one covering an entire city is still more efficient. The bigger the operation, the more the restaurant likes it, and the more the customer likes it. You are about to lose your neighbourhood logistics business to a software company.

So you become a software company too, or you die. And now you are coordinating across an entire city: matching thousands of orders to thousands of drivers to thousands of restaurants in real time. You have machine learning models that every day takes every active order and every available driver on your payroll and finds the assignment that minimises cost, where cost is a function of distance, [how long the food will take to make](https://bytes.swiggy.com/predicting-food-delivery-time-at-cart-cda23a84ba63), traffic, etc. 

The inputs to this model are themselves outputs of other complex models: forecasting demand by zone and time, calculating two-wheeler speed on every road segment, and *on and on and on.* Every week your machine learning models retrain on more data, and every marginal improvement compounds across millions of daily orders, and every improvement in delivery time attracts more customers, which produces more orders, which produces more data, which makes the models better still.

Except, most likely, you didn't end up doing this. Your neighbourhood delivery logistics company probably died. This is what people meant when they said "software is eating the world" and "every company is a software company." 

There were *so many* of these businesses when the technological revolution came, and most did not adapt. The flywheel of scale that software enabled was brutal to incumbents and the platforms swept their competitors away: implacably, inevitably, relentlessly. They conquered city after city, dismantling their existing logistics networks or absorbing them with endless process reengineering. 

The software companies did this without employing a single driver. They understood that demand for restaurant food is spiky: peaking sharply at lunchtime, dinnertime, during the IPL, on New Year's eve. The gap between a 9am trough and an 8pm peak could easily be four-fold, fivefold, tenfold. They understood that if you employ drivers, you staff for the peak hours, and they sit idle. And they were at war with other software companies. They understood that you either ruthlessly optimise or die. Civilisation is brutal.

## Finding the drivers

India is a country with cheap and plentiful labour: you can give practically anyone a phone and a two-wheeler and send them off to do deliveries. This was ideal for the platform companies. India also has some of the most intense labour laws in the world, that kick in at tiny thresholds. You attract a universe of legal obligations when you hire more than 10-20 workers, and it becomes impossible to fire them and much more expensive to keep them employed. Firms [stay small to avoid labour law](https://the1991project.com/sites/default/files/2024-09/4999_Rajagopalan_Shah_India_Labor_Edition_MR_v1-compressed.pdf), and more than 90% of the working population in India is outside serious labour protections:  street vendors, construction workers, agricultural labourers. And this is 90% of the *workforce*. Nearly \_\_% of the population are not even *in* the workforce: they're unemployed. The labour laws were designed to protect workers in factories in Bombay in 1881; the economy changed and everyone found inventive ways to ignore it.

This was a problem that was faced in manufacturing. They are covered by the labour laws once they breach a number-of-workers threshold, and so they stay small to avoid dealing with the state. Except, smart lawyers discovered that you could have *contract labour*. You'd hire a company which would hire the workers who were not absolutely *central* to your enterprise and you would avoid having direct obligations to those workers, who you wanted to engage and disengage easier. The Government retaliated with the Contract Labour (Regulation and Abolition) Act 1970, constraining the use of contract labour, and if they found that you were hiring "core" people through a middleman, they would become part of your permanent workforce and you would start owing labour law obligations to them.

There was a lot of back and forth, but contract labour use really started booming in the 2000s, after a Supreme Court decision that clarified that *you wouldn't have to absorb them into your workforce.* The tail risk of hiring a ton of contract labour and getting sued into all of them becoming employees you couldn't fire became much less likely, and so the firms began hiring. Labour became more of a flexible input again. The firms started hiring more, and [hiring more contract labour](https://onlinelibrary.wiley.com/doi/epdf/10.3982/ECTA20046).

There's a model here: the costs imposed by the labour laws meant that hiring was expensive and firing was nearly impossible, so firms stayed small, or found ways around it. [Bertrand, Hsieh and Tsivanidis (2025)](https://onlinelibrary.wiley.com/doi/epdf/10.3982/ECTA20046) estimate that the expansion of contract labour increased manufacturing productivity by 7.3%.

The food delivery platforms found a way around labour law too. And it was much more straightforward. They didn't employ the drivers or contract them through staffing agencies; they used the thing that literally everyone in India does, and engaged in "informal labour" that is not covered by the labour laws. Except they used software to intermediate the supply of informal labour, in a nice phrase I read from Shah and Ghatak.

India has had other non-software mechanisms for intermediating informal labour for a long time. In *A Free Man*, Aman Sethi describes the Mazdoor Chowks (literally, labourer market) of Delhi:

> If you want a job in Bara Tooti, wake up early, order a cup of chai, and wait by the main road—work will come to you. Shopkeepers looking to extend their storage space by knocking down a wall between two adjacent rooms; house owners looking to turn a balcony into an extra bedroom; contractors searching for extra labour; families looking for someone to whitewash their staircase the day before their daughter's wedding—they all come down to Bara Tooti in search of mistrys and beldaars, karigars and mazdoors.

So the platforms specialised and built an app to do it, and handled the logistical challenges of doing it, and optimised the process of giving orders and making them follow it. They talk about how it gives the worker flexibility, and it does, even more than the Mazdoor chowks were flexible, and they were too, as a labourer Ashraf in *A Free Man,* explains:

> 'Azadi is the freedom to tell the maalik to fuck off when you want to. The maalik owns our work. He does not own us. \[...\] If Choduram pays you on the first day, you work for him on the second. He pays on the second, work for the third. He stops paying, you stop working.

The delivery driver logging on to Swiggy at 7 PM and logging off at 10 PM is doing dehadi with better technology. The platform pays per delivery, almost immediately.
