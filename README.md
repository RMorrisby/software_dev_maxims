# Software Development Maxims

A collection of maxims & other thoughts, concering all aspects of software develoment.

- Agile / SCRUM
- Bugs
- Team health


## Agile / SCRUM

(for better or worse, most people treat "Agile" and "SCRUM" as being equivalent. For pragmatic reasons, we will not attempt to split the two terms here, but instead focus on good and bad practices across both)

Always remember the Agile Manifesto :

```
- Individuals and interactions over processes and tools
- Working software over comprehensive documentation
- Customer collaboration over contract negotiation
- Responding to change over following a plan

(while there is value in the items on the right, we value the items on the left more)
```

The Agile Manifesto can be largely distilled into : 
- **Do the minimum work required to satisfy your users in the long-term**

Therefore we should :

Determine what the long-term goals fo the project are, and what benefits the software will bring to your users.

Always aim for this long-term goal.

There will often be short-term constraints (e.g. "show X progress by Y date or your funding is removed"). The same principles apply - do the minimum work required to satisfy X, BUT still aim for the long-term.

If projects only aim for short-term goals, the project will die before it reaches the long-term.

Therefore the team should always invest in itself - develop tools, processes & people that will help it work more quickly, effectively and happily.

The earlier the team invests in itself, the more benefit they will reap (that's why it's called investment). This applies to the entire team, not just automated testing.




## Testing / QA

Broken until proven working.

Trust in a test's results must be earned.

If your test suite has a 100% pass rate, something's broken (or your test suite is too small).

Your Test environment should be as representative of your Live environment as possible.

Tests should use Live data (or data that at least looks like Live data).

Tests must be readable. A human should be able to execute the test simply by following the test script.

Automated tests must be easy to debug. The most important question anyone will ever ask an automated test is "what are you intending to do?". The quicker we can answer this question, the quicker we can validate the test. The quicker we can validate the test, the quicker we can trust it.

Make sure that tests are actually doing what they intend to be doing.

Conciseness is a virtue, but readability is a greater virtue.

Primary concerns for automated tests are : accuracy, readability, maintainability. 

Automated tests must be implemented with these as the primary questions : 
1) If a feature-change breaks a test, how quickly can you ascertain with 100% certainty that the test needs to be updated or has found a bug?
2) If the test needs to be updated, how quickly can this be done while keeping the test accurate, readable and maintainable?

Performance of automated tests is a secondary concern, not a primary one. Use a language & toolset that will provide the best long-term solutions to those two questions. 

Certain languages are inherently less readable than others (e.g. Java vs. Ruby). A lot of automated testing does not require advanced language usage - but does require good general software development skills. Therefore if your team does not have much skill in nimbler, more readable languages, always consider training & learning. Always remember the long-term goal. This is an investment!

An extreme example would be : would you write automated tests for a web-UI in Assembler? You could do it, but it would be quicker **in the long-term** to learn a more suitable language.





## Bugs

A bug is a bug.

The more bugs your software has, the more disgusting it is to use.

`TODO more`
















## Team health

Team health is a three-legged stool. The three legs are productivity, efficiency and morale. 

The project is the team; the team is the project.

Everyone is responsible for the team's health.

The more responsibility you have in your team, the more responsibility you have for its health.

The more power you have in your team, the more responsibility you have for its health.

Communication is hard.

Communication is vital.

Don't think "someone else will do it" until you've heard them say it.

If someone says they'll do something, hold them to it.

Cargo cults were bad; software development cargo cults are just as bad. If you don't understand why something has to be done a certain way, ask your leaders.

If you don't know why you're doing something a certain way, why are you doing it?

### Signs of poor team health

Your [Bus Factor](https://en.wikipedia.org/wiki/Bus_factor) is < 1 (your project is living on borrowed time)

Your [Bus Factor](https://en.wikipedia.org/wiki/Bus_factor) is < 2 (your project is like an aeroplane with one engine)

Any of your leaders say "we don't need to do Retrospectives".

Any of your leaders say "we don't have time to do Retrospectives".

Any of your leaders say "Retrospectives are a waste of time".

Some parts of the team are consistently underworked, while others are consistently overworked.

People don't talk to each other.

The team does not invest in itself :
 - training
 - building tools to help the team (e.g. a script to build & deploy your software)

### Retrospectives

Always hold regular 'Retrospective' sessions, every 2-4 weeks.

Make sure everyone can attend Retrospectives. If some people cannot attend one, schedule the next one at a time they can attend.

Focus on the good as well as the bad. Take time to understand why something has gone well, just as you take time to understand why something has gone badly.

Retrospectives take as long as they take. If they're taking too long, hold them more frequently.

Make sure that everyone gets a good chance to contribute.

The goal of Retrospectives is to identify problems faced by the team, so that they might be fixed and the team can be happier and more productive. It is not just for whinging!

[Retrospectives](https://github.com/RMorrisby/software_dev_maxims/blob/master/Retrospectives.md)

# Development

Always automate any set of steps that the team will do more than twice - executing tests, deploying your software, (re)building a dev environment for a new team member, etc.

Always add comments to your classes & methods. State what they intend to do, not what they are actually doing! The most common bugs occur when the intent differs from the action; the easier these differences are to spot, the fewer bugs you will have.

Conciseness is a virtue, but readability is a greater virtue.

Always put TODOs in your code.

`TODO more`