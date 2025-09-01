# Introduction

The story with Elon Musk and Paypal from *Founders at Work*.
- The story shows the importance of technical choices. 
- And strategy. Where you put your effort really makes a difference if your company stays in business. And this might not be only about technology... 

## Examples of Software Engineering Hypes

- 1990s - **OOP** was going to revolutionize software engineering
- 2000s - **SOA** revolutionizing enterprise architecture
- 2010s 
	- **NoSQL** killing relational databases
	- **Blockchain** replacing banks and *fiat* currency
	- **AI** replacing all developers

Do you have other examples? 


## Learning objectives

By the end, you will:
- Recognize the anatomy of technical hypes
- Understand why hypes emerge and spread


# Part 1: The Anatomy of Hype

## The Hype Cycle 

A Gartner model illustrates the expectation vs. reality gap over time with respect to new technologies. 

Phases are: 
- **Innovation trigger** - starts when an event, like a technological breakthrough or a product launch, gets people talking
- **Peak of inflated expectations** - is when product usage increases, but there’s still more hype than proof that the innovation can deliver what you need
- **Trough of disillusionment** - the original excitement wears off and early adopters report performance issues
- **Slope of enlightenment** - occurs when early adopters see initial benefits and others start to understand how to adapt the innovation
- **Plateau of productivity** - innovation goes mainstream

(From: [online](https://www.gartner.com/en/documents/5659723) at gartner.com)

Note that, as my colleague Sebastian Baltes observes, Gartner is themselves responsible for many of the hypes [2]. They are one of the amplifiers. 


### Case Study 1: Walkthrough: Microservices

It started with the [API Mandate](https://nordicapis.com/the-bezos-api-mandate-amazons-manifesto-for-externalization/) by Jeff Bezos. Every team must expose their business via an API. Thankyouverymuch. 

- 2011 - Microservices term coined in a workshop
- 2012 - Netflix and Amazon pioneer it 
- 2014: “Death of the monolith!” 
	- The word monolith starts to be considered as bad as the word waterfall
	- Martin Fowler writes a [guide](https://martinfowler.com/articles/microservices.html) to Microservices
- 2016-2018: Everyone migrating everything 
	- Search on YouTube for "migrating from monolith to microservices"
	- consulting business flourishes
- 2019-2020: “Distributed monolith” problems emerge - while at the same time, people are still giving talks about how to migrate from monoliths to microservices. 
	- strawman - you don't need microservices if you have a monolith; you might split it in services
- 2021+: “Maybe start with a monolith” wisdom
	- Read: [The Majestic Monolith](https://signalvnoise.com/svn3/the-majestic-monolith/), by DHH (10min read) 


# Part 2: Why Hypes Happen

Reasons are often multifaceted but I think a combination of the following factors: 

- **Real technical problems needing solutions**
	- software engineering is complex
	- large systems are hard to build and maintain
	- e.g.. when a single DB does not fit your data you have to find solutions to distribute it
- **Innovators develop new solutions**
	- Especially true in software -- a culture of creative people 
		- Programmers and doctors *some of the most creative people*... i don't remember where I read it, but I liked to believe it :)
		- A culture of iconoclasts - throwing everything out and starting from scratch (are we more creative as personalities? no law student thought that they could build their own code of law; but the MongoDB authors were convinced that their new DB is better than the *old* relational ones)
	- ... and often present them in an oversimplified manner - out of enthusiasm. 
- **Many actors are incentivized** to amplify the benefits. The *attention economy* is especially sensitive to novelty and high promises 
	- Vendor/consultant economic incentives ("Consultants are selling everything that’s hyped")
	- Developers like to learn new stuff => *resume-driven development* empirical study [3]
	- Companies want to *look cool* because they need developers 
	- Conference/blog echo chambers
	- Journalists must exaggerate to get "clicks" 
	- FOMO in competitive industries
- **Psychology factors**
	- Novelty bias
	- Silver bullet thinking
	- Complex corporation politics and incentives (the guy with the big team)
	- Survivorship bias (only success stories get publicized)
	- The developer that retreats in his technical corner because he does not care about the company problems - see paper by Sebastian 
	- Cargo culting -- just because Google does it, we should also do it

The argument from the Broy article: in our domain the entry barrier is low and people even w/o education can enter.




# Part 3: Hype Patterns in Software Engineering

Common hype archetypes. 

## The Killer: “X will kill Y” 
- NoSQL kills SQL (rant about MongoDB)
- AI kills software development
- Quantum computing kills cryptography 

## Technology X will solve a social problem

- Blockchain replaces banks
- MOOCs will replace universities (I guess we will soon see the ChatBots will replace universities? )


## The Multiplier: “10x faster/better/cheaper”
- 3rd GL languages
- GenAI - makes developers 10x - studies show that it’s more modest than expected and for complex tasks can be even slower. 

## The Savior: “Solves all your problems”

- SCRUM - I once heard the scrum book author give a talk. He thinks that scrum could scale at the whole humanity level. He believes that all the cells in our body could be organized with scrum. 


# Part 4: Current and Historical Examples

Historical hypes that settled:
- Object-oriented programming (valuable but not revolutionary)
- Service-oriented architecture (good idea, overhyped execution)
- Agile (transformed industry, but not a silver bullet)
- NoSQL - useful in situations where eventual consistency is acceptable

Recent hypes in various stages:
- AI/ML everywhere - including AI-powered mattresses and AGI
- Kubernetes for everything
- Serverless and the cloud as default
- Low-code/no-code platforms
- GraphQL -- was also overhyped but for a shorter time
- Blockchain / Web 3 - the slowest distributed global network is useless for any other use case but for dark web sales and people who have interests in going around the 

Quick poll - “Which of these do you think is most overhyped right now?”


# Part 5: Are Hypes Good? 

Innovation is good.

The hype by definition is not. Exagerating the value of something is at the least, unethical; and much more likely, dangerous because it wastes resources. And misleads people. 

How do hypes waste resources? Cf. The Effects of Hype in the Software Domain: Causes, Consequences, and Mitigations [1], we have: 
- academic efforts are squandered
- people who are not that good technically fall for the sales presentation

The opportunity cost of falling for the hype
- While you spend time and money rebuilding everything with the new technology, the guy that has the server-side rendering rails application is collecting all the money. 
- Those money wasted on moving townhall records on the blockchain could not be used for something else

The story of Map-Reduce where everybody run to copy Google, and in the meantime, Google had already moved on because they realized it did not work not even for them. 



# Wrapping Up

To think about: “In every hype there is something useful. Can you detect it? At the same time, falling too strong for it can be fatal for you and your company. Or maybe wasteful. Or maybe just you are too proud to be fooled. 

Next time, we’ll learn how to systematically analyse technologies to see through the hype. 


# Group assignment

- Choose a technology/methodology that’s been hyped (past or present)
- Briefly describe the context that gave rise to it
- Document its promises
- No judgment yet - just understand what was promised and why people got excited





# References
1. M. Broy, B. Selic - The Effects of Hype in the Software Domain: Causes, Consequences, and Mitigations, [online](https://www.computer.org/csdl/magazine/so/2025/02/10884672/24j4eFje1IQ) 
2. Sebastian Baltes - Effects of hype in software development, [online](https://empirical-software.engineering/blog/hype-in-software-development)
3. Jonas Fritzsch; Marvin Wyrich; Justus Bogner; Stefan Wagner - Résumé-Driven Development: A Definition and Empirical Characterization,  [online](https://ieeexplore.ieee.org/document/9402191 )

