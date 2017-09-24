# The Building Blocks of DevOps
## Culture Change
* Blame Game
* Conways Law
* Evangelism/Public relations
* Overcoming organizational barriers
* Moving from a “ticket” culture to “ownership” culture
* Cross-functional teams with end-to-end ownership of services
* Innovators/Followers/Laggards
* Overcoming traditional project attributes
  * Hero cult
  * Shadow responsibilities
  * Emphasis on title
  * Favor a plan over planning
* Mike Rother in his “Toyota Kata” book points out that of the many who try to emulate Toyota, most miss the invisible side of what they were doing. The key, as Rother suggests, is that it wasn’t the tools that made Toyota great, it was the culture and specific behavior associated behind those tools.

## Measurement and Metrics
* “Change” serves as a shared unit of measurement.
* Cycle Time
* Focus on leading quality metrics instead of lagging
* Definition of Done
* SonarQube (Required to be part of CI, quality gates)
* Measure DevOps Progress (Specification by Example)
* Measure Cultural Change (surveys)

## Improve and Accelerate Delivery
* Incremental releases
* Versioning
* SCM Required
* Baselines
* By reducing batch size, we can deploy more frequently because reducing batch size drives down cycle time.

## Automatic Releasing
* The key goal of automatic releasing is to reduce the risk of releasing.
* Should you automate everything? NO
* Law of Marginal Costs
* Required to flip the testing pyramid

## Apply Releases Incrementally and Iteratively
* An iteration is a mini-project that may result in an increment of the software. Iterating starts with an idea of what is wanted, and the code is refined to get the desired result. An increment is a small unit of functionality. Incrementing allows you to build a better understanding of what you need, assembling the software piece by piece.
* Upgrading all of the components in one big-bang release is the highest-risk way of rolling out new functionality.
* Instead, deploy the components independently in a side-by side configuration wherever possible.

## Monitoring
* Automatic releasing must be accompanied by monitoring.
* Monitoring is the activity of continuously collecting and storing data about the state of the application, middleware, and infrastructure and making this state visible to the whole team.
* Monitoring is used to detect (or even prevent) production incidents and to minimize MTTR and MTTD. (Mean Time to Resolution/Detection)
* Monitoring Driven Development – The Holy Grail – Health Dashboard
* Running Automated Tests in Production – Yes
* Smoke Tests – There is a reason we do this
* DevOps fundamental – Never break the customer (internal or external)

## Decoupled Deployment and Release
* Decoupling deployment and release improves and accelerates delivery, which is one building block of DevOps.
* We no longer use traditional branching strategies.
* Branch by Abstraction
* Feature Toggles
* Dark Launching
* Blue-Green Deployment

## Specification by Example
* Behavior Driven Development/Acceptance Driven Development (BDD/ATDD)
* DevOps requires a common language (Release example)
* Living/executable documentation
* It provides the traceability for everything you’re doing

## Infrastructure as Code
* We treat the infrastructure the exact same as application code.
* Lives in an SCM
* Is tested just like application code (TDD)
* Is monitored constantly just like application code

## Additional DevOps Benefits
* Security
* A/B Testing
* Performance and Load Testing
* Chaos Monkey
* Mobile (treat just like binary files)
* Moving away from outsourcing and investing in engineering practices

## Cutting Edge DevOps Practices
* Dojos
* Information Radiators
* Internal DevOps Days
* Internal Software Engineering Conferences
* Hackathons
* DevOps/IT Academies
* Engineering Blogs
* Communities of Practice
* Jidoka/Andon Cord
* Chaos Cord
* Improvement Kata
* “Sensei”, or Masters
