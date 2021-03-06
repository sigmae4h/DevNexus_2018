## Dev Nexus 2018
[Schedule](https://devnexus.com/schedule)

### Feb 22
#### Software architecture for developers
Simon Brown @10:00 - A403

* Not big design up front
  * Usual pattern: Big design vs. Nothing
  * Don't do either - use Evolutionary Design
    * What are you building?
    * Does it work?
    * Cost of change?
* Every team needs to think about architecture
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
* UML is not needed
  * Think about abstractions first
  * Focus on communicating intent
  * Use map keys:
    * Systems (context)
    * Containers
    * Components
    * Classes
  * Tool: Structurizr
* Continuous Improvement mindset
  * Enables agility
    * Microservices / modular monolith
  * Agility is a quality attribute
  * **Book**: Clean Architecture, Uncle Bob

#### Continuous Delivery for Data Pipelines
Sabby Anandan @11:15 - A305

* Spring Cloud Data Flow
  * Data Integration
    * Source -> Process -> Sink
  * DSL inspired by Unix pipes and filters
  * Easy to use different technologies
  * Difficult to change properties (flow) while running
* Spring Cloud Skipper
  * Allows real-time flow manipulation
  * Rollback supported

#### How to Hire Good Programmers
Jennifer Bland @13:15 - A311

* Normal interview process is suboptimal
  * Coding challenge
  * Whiteboard
  * Phone screens
* Should do:
  * Stop at home coding challenges, standing up new projects / frameworks is a rare experience
  * Use short coding exercise, broken down like below (simple questions)
    * HTML/CSS
      * Differance between id and class?
      * What does the box model refer to in CSS?
      * What are reset css file and normalize.css?
    * JavaScript/jQuery
    * Node.js
  * Allows objective scoring system based on answer details
  * Provide code sample, ask for simple manipulation
  * Building on the previous questions, add challenge to make more difficult
  * Create standard questions, share them with other interviewers
    * Can fabricate checklist of possible answer details
    * Consistency is the key
    * Decide on minimum score
      * Does the canidate meet?
      * How do they compare to other canidates?
      * Resolution of same score
* Have casual conversation
  * Non-threatening, non-challenging environment
  * Ask about preferences (Eg: Do you prefer Sass or LESS? Why?)
  * Ask about the tests they would write for a given scenario
  * Indicates character, motivations, ext
* Resources
  * [www.codeprep.io](https://www.codeprep.io)
  * [www.in5days.tech](http://www.in5days.tech)
  * YouTube: [jenniferbland](https://www.youtureb.com/c/jenniferbland)
  * Twitter: @ratracegrad

#### Sifting Technologies - Separating the Wheat From the Chaff
Nathaniel Schutta @14:30 - A403

* Challenge: Evaluate tech
  * Core skill
  * Technology continuously changes
  * Old tech isn't always bad
* Find where **not** to use tech
  * Trial and error
  * Develop expertise
* Don't constantly change direction
  * Have a strategy
  * Explore communities
  * Read books
  * Develop a routine
  * Be selective, don't waste attention
  * If something is important enough, you will hear about it
* Knowing where to invest your time
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
* Understand trade-offs
  * Heart of design
  * Always alternatives
  * Understand all costs
* Implement
  * Workshop
  * Make it easy
* Stay current in tech
* Snowflakes are not safe: Rotate, Repair, Repave
  * Update versions
  * Patching strategy
  * N, or N-1, software (dependency) version policy
    * Measure and enforce
* Determine what to evaluate (critical properties)
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

* Focus on high quality product
* Modern relevance
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
* European Communities
  * SoCraTes
  * Codebar
  * Ladies of Code
  * Queer Code
* Future
  * Industry ethics
  * Socially responsible software

#### A Look Back at Enterprise Integration Patterns and Their Use into Today's Serverless Computing
Bruno Borges @17:00 - A404

* What is Serverless?
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
* What is EIP?
  * IF (this) THEN that;
  * Address common integration problems through messaging
  * Apache Camel: Framework that makes integrations easier
  * **Book**: Enterprise Integration Patterns


### Feb 23
#### SSL/TLS for mortals
Maarten Mulders @10:00 - A313

* Why bother?
  * Using SSL correctly is often hard to achieve
  * Critical for secure connection between systems
* Security in the Transport layer
  * TLS safe versions 1.1 & 1.2
  * Anyone can intercept http traffic
  * Implementation
    * Pubic / private key encryption
      * RSA most frequently used encryption algorithm
    * Signed certificates
    * Certificate Authority
  * Distrust self signed certificates
* Tools
  * `curl -v -k <address>`
  * `openssl s_client -showcerts -servername <address> -connect <address>:443`
  * `-Djavax.net.ssl.keystore=<file>`

#### Enable IoT with Edge Computing and Machine Learning
Jared Rhodes @11:15 - A305

* IoT is everywhere
  * Electronics are cheep and easy to integrate
* Azure IoT Edge
  * Modules: deploy from cloud to device
    * Docker container communicate across service bus
  * Used for immediate response
  * Edge runtime
    * Manages modules
  * Be aware of computational power on IoT devices

#### Bootiful Kotlin
Josh Long @13:15 - A402

* [Code](https://github.com/joshlong/bootiful-kotlin)
* **Book**: Cloud Native Java
* Kotlin: Has features that are not yet in Java 10
* Spring framework 5: 2.0.0 RC2
  * Contains Kotlin DSL
* Kotlin
  * Classes default to final
    * Kotlin-maven-allopen: Adjusts some Kotlin attributes
  * Default class getters and setters
  * Null checking unneeded
    * Elvis operator is also a part of the language
  * Expose
    * org.jetbrains.expose
    * exposed-spring
    * Easy way of interfacing with databases
  * Many external libraries are included

#### Building Real World Node.JS Microservices
James Truitt @14:30 - A411

* Principals of Microservices
  * Self contains small services implementing a single business capability
  * Small, independent and loosely coupled
  * Each service is a separate codebase
  * Independently deployable
  * Persist own data or external state
  * Use well defined APIs to communicate
  * Can use different technologies, libraries, or frameworks
  * When to use
    * Large apps that require high release velocity
    * Complex highly scaleable apps
    * Small teams
  * Benefits
    * Independent deployments
    * Independent development
    * Small, focused teams
    * Mixed tech stacks
    * Granular scaling
  * Challenges
    * Complexity
    * Development and integration tests
    * Team integration
    * Data integrity
    * Versioning
  * Best practices
    * Model services around business domain
    * Decentralize everything
    * Data storage should be private to the service that owns it
    * Communicate through well defined APIs
    * Avoid coupling between services
    * Offloading cross-cutting concerns, such as authorization and SSL termination, to the gateway
    * Keep domain logic out of the gateway
* Deployment Options
  * Containers
    * Azure Container Services (AKS)

#### Machine Learning Exposed
James Weaver @15:45 - A403

* Twitter: @JavaFXpert
* Science of getting machines to do things without explicit programming
* Categories
  * Supervised Learning
    * Data provided has correct answers
    * Example: Iris flower data set
  * Unsupervised Learning
    * Data does not contain answers
    * Machine must find structure in unstructured data
  * Reinforcement Learning
    * Rewards given for correct behavior
* Visualize with TensorFlow tool
* Anatomy (deep learning)
  * Input layer
  * hidden layers
  * Output layers
* Library: deepLearningForJ
  * [deeplearning4j.org](https://deeplearning4j.org)
* Three blue one brown
* Back propagation: training the network
* **Book**: Make Your Own Neural Network
* [TensorFlow playground](http://playground.tensorflow.org)
