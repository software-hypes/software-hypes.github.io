
# In software engineering... it depends


The hypes of the tulips. 

Hypes can be stupid and in that case, you should avoid them. 

Or hypes can be just exaggerations of the usefulness of tools, and in that case you should understand the tools and the right context of use. 


# Three Approaches to Microservices

There is a continuum between: 
- [The Majestic Monolith](https://signalvnoise.com/svn3/the-majestic-monolith/), at Basecamp
- Hybrid [Monolith + Microservices](https://www.infoq.com/presentations/github-rails-monolith-microservices/) at GitHub (monolith scales to 1B calls / day)
- [Microservices at Netflix](https://youtu.be/CZ3wIuvmHeM?t=584)

The paradox: “All three are ‘right’.


# Context is what determines the usefulness 

## Language Examples

- Python - ignored initially because it was too simplistic; but useful in the right context: e.g., data science, we applications
- JS - the trivial language - but because was the only way to build web apps, it took over the world
- etc.


## There are many dimensions of context in software engineering

- We discussed about the variables that you would have to take into account when doing a study on typed systems. 
- Many of those variables are the context that you have to take into account. 
- Every system exists within unique constraints
- Trade-offs shift based on context

### Dimensions of context

#### Technical context dimensions
- **Scale**: Users, data volume, request rate, geographic distribution
- **Performance requirements**: Latency, throughput, availability
- **Consistency needs**: ACID vs. eventual consistency trade-offs
- **Data characteristics**: Structured vs. unstructured, read vs. write heavy

#### Organizational context dimensions
- **Team size and skills**: 20 developers vs. 2000 developers
- **Development velocity needs**: MVP vs. long-term platform
- **Risk tolerance**: Startup agility vs. enterprise stability
- **Existing systems**: Greenfield vs. legacy integration


#### Business context dimensions
- Time constraints: 3-month deadline vs. long-term project
- Budget limitations: Open source only vs. enterprise tools available
- Compliance requirements: GDPR, financial regulations



# When Context Evolves

### Context isn’t static
- Startups become enterprises
- Teams grow and shrink
- Popularity of the service grows or shrinks 



### Evolution examples

#### Basecamp - moving away from the cloud

- [We have left the Cloud](https://world.hey.com/dhh/we-have-left-the-cloud-251760fb)
- what changed in the context? 

#### Prime video team moving away from Lambda

- [The Amazon Team that Moved Away from Lambda](https://web.archive.org/web/20240805183535/https://www.primevideotech.com/video-streaming/scaling-up-the-prime-video-audio-video-monitoring-service-and-reducing-costs-by-90)
- what changed in the context?

#### Company moving away from Elm 

- [On Endings: How and Why We Retired Elm at Culture Amp](https://kevinyank.com/posts/on-endings-why-how-we-retired-elm-at-culture-amp/) 
- what changed in the context? 

#### Twitter: Ruby on Rails → Scala services

- Started as a Rails monolith but faced severe scaling issues during rapid growth (2006-2010). 

- "Fail whale" became infamous as the platform couldn't handle traffic spikes

- Replaced Rails components with JVM-based services in Java/Scala

- [Moved to a service-oriented architecture](https://www.infoq.com/news/2012/11/twitter-ruby-to-java/) with hundreds of microservices


#### Shopify: Rails monolith → modular monolith

- [Decomposed the monolith](https://shopify.engineering/deconstructing-monolith-designing-software-maximizes-developer-productivity) into distinct bounded contexts within the same codebase

- Used Ruby's module system and careful dependency management

- Gradually extracted some services (like checkout) but kept most functionality in the modular monolith


# Conclusion

Ask context questions first before evaluating any technical solution, i.e. anamnesis at the doctor's.

Nothing is unalloyed good. A good tool in the wrong context is a bad outcome. 

# Project Implications

Your final reports should demonstrate this thinking - not just what a technology does, not only that it is hyped, but also when and why it’s the right choice.






