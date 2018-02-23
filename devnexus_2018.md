## Dev Nexus 2018
[Schedule](https://devnexus.com/schedule)

### Feb 22
#### Software architecture for developers
Simon Brown @10:00 - A403

1. Not big design up front
  * Usual pattern: Big design vs. Nothing
  * Don't do either - use Evolutionary Design
    * What are you building?
    * Does it work?
    * Cost of change?
2. Every team needs to think about architecture
  * Avoids chaos
  * Not a relay sport
    * Architect must be involved in whole process
    * Must have continuous technical leadership
    * Different styles of leadership for different teams
    * Pair architecting
    * Soft skills important
      * **Book**: Talking with Tech Leads
    * Architects write code: be involved
    * Architects should be master builders
      * Must understand technology
      * **Book**: Progress Toward an Engineering Dicipine of Software
3. UML is not needed
  * Think about abstractions first
  * Focus on communicating intent
  * Use map keys:
    * Systems (context)
    * Containers
    * Components
    * Classes
  * Tool: Structurizr
4. Continuous Improvement mindset
  * Enables agility
    * Microservices / modular monolith
  * Agility is a quality attribute
  * **Book**: Clean Architecture, Uncle Bob

#### Continuous Delivery for Data Pipelines
Sabby Anandan @11:15 - A305

1. Spring Cloud Data Flow
  * Data Integration
    * Source -> Process -> Sink
  * DSL inspired by Unix pipes and filters
  * Easy to use different technologies
  * Difficult to change properties (flow) while running
2. Spring Cloud Skipper
  * Allows real-time flow manipulation
  * Rollback supported

#### How to Hire Good Programmers
Jennifer Bland @13:15 - A311

1. Normal interview process is suboptimal
  * Coding challenge
  * Whiteboard
  * Phone screens
2. Should do:
  * Stop at home coding challenges, standing up new projects / frameworks is a rare experience
  * Use short coding exercise, broken down like below (simple questions)
    1. HTML/CSS
      * Differance between id and class?
      * What does the box model refer to in CSS?
      * What are reset css file and normalize.css?
    2. JavaScript/jQuery
    3. Node.js
  * Allows objective scoring system based on answer details
  * Provide code sample, ask for simple manipulation
  * Building on the previous questions, add challenge to make more difficult
  * Create standard questions, share them with other interviewers
    * Can fabricate checklist of possible answer details
    * Consistency is the key
    * Decide on minimum score
      1. Does the canidate meet?
      2. How do they compare to other canidates?
      3. Resolution of same score
3. Have casual conversation
  * Non-threatening, non-challenging environment
  * Ask about preferences (Eg: Do you prefer Sass or LESS? Why?)
  * Ask about the tests they would write for a given scenario
  * Indicates character, motivations, ext
4. Resources
  * [www.codeprep.io](https://www.codeprep.io)
  * [www.in5days.tech](http://www.in5days.tech)
  * YouTube: [jenniferbland](https://www.youtureb.com/c/jenniferbland)
  * Twitter: @ratracegrad

#### Sifting Technologies - Separating the Wheat From the Chaff
Nathaniel Schutta @14:30 - A403

1. Challenge: Evaluate tech
  * Core skill
  * Technology continuously changes
  * _Old_ tech isn't always bad
2. Find where **not** to use tech
  * Trial and error
  * Develop expertise
3. Don't constantly change direction
  * Have a strategy
  * Explore communities
  * Read books
  * Develop a routine
  * Be selective, don't waste attention
  * If something is important enough, you will hear about it
4. Knowing where to invest your time
  * Don't relay on hunches
  * Beware of bias
  * Look at community consensus
  * Resource: ThoughtWorks Technology Radar
  * 20% time / Friday "hack time" / tech talk day
  * Architectural briefings
    * Why use a tech?
    * Not a howto
    * Keep it short (45 min or so)
    * What problems does this not solve?
    * Keep the message simple
    * Everyone must participate
5. Understand trade-offs
  * Heart of design
  * Always alternatives
  * Understand all costs
6. Implement
  * Workshop
  * Make it easy
7. Stay current in tech
8. Snowflakes are not safe: Rotate, Repair, Repave
  * Update versions
  * Patching strategy
  * N, or N-1, software (dependency) version policy
    * Measure and enforce
9. Determine what to evaluate (critical properties)
  * Documentation
  * Codebase
  * Maturity
  * Upgrade path
  * Frequency of updates
  * Stability
  * Ability to add
  * Support
  * Training
  * Developer / team interest
  * Corporate fit
  * Licensing

#### Modern software craftsmanship
Daniel Irvine @15:45 - A311

1. Focus on high quality product
2. Modern relevance
  * Quality
    * Not important for most of the industry
    * Quality Assurance: An admittance that developers are not good at quality
    * Not something that most users can see
    * Very important to longevity, ability to change
    * Measure is not: Coverage, linting, or documentation
  * Professionalism
    * Responsibility
    * Pride in work
  * Community
    * Life long learners
    * Deliberate practice
    * Mentoring
    * Not about "years of experience"
    * Sponsorship
3. European Communities
  * SoCraTes
  * Codebar
  * Ladies of Code
  * Queer Code
4. Future
  * Industry ethics
  * Socially responsible software

#### A Look Back at Enterprise Integration Patterns and Their Use into Today's Serverless Computing
Bruno Borges @17:00 - A404

1. What is Serverless?
  * Abstraction of servers
  * Event driven / instant scale
  * Micro billing
  * Evolution: hardware -> virtualisation -> kuberneties -> serverless platform
  * How?
    * Kubeless
    * Apache OpenWhisk
    * OpenFaaS
    * Fn Project
    * Cloud (AWS Lambda, Azure Functions, Google Cloud Functions)
  * Demo 1: Running a Java function from Azure Functions
2. What is EIP?
  * IF (this) THEN that;
  * Address common integration problems through messaging
  * Apache Camel: Framework that makes integrations easier
  * **Book**: Enterprise Integration Patterns


### Feb 23
#### SSL/TLS for mortals
Maarten Mulders @10:00 - A313

1. Why bother?
  * Using SSL correctly is often hard to achieve
  * Critical for secure connection between systems
2. Security in the Transport layer
  * TLS safe versions 1.1 & 1.2
  * Anyone can intercept http traffic
  * Implementation
    1. Pubic / private key encryption
      * RSA most frequently used encryption algorithm
    1. Signed certificates
    1. Certificate Authority
  * Distrust self signed certificates
3. Tools
  * `curl -v -k <address>`
  * `openssl s_client -showcerts -servername <address> -connect <address>:443`
  * `-Djavax.net.ssl.keystore=<file>`

#### Enable IoT with Edge Computing and Machine Learning
Jared Rhodes @11:15 - A305

#### Bootiful Kotlin
Josh Long @13:15 - A402

#### Building Real World Node.JS Microservices
James Truitt @14:30 - A411

#### Machine Learning Exposed
James Weaver @15:45 - A403
