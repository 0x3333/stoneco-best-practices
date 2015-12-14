![alt text](https://github.com/beeva-danielpetrovic/beeva-best-practices/blob/master/agile/developerTeamScrum/ATDD/static/atdd-cycle.png "ATDD")
# ATDD (Acceptance Test-driven development)
At this point we're going to talk about atdd

## Index

* [What is ATDD?](#what-is-atdd)
* [Based Features](#based-features)
* [Objectives ATDD](#objectives-atdd)
* [Criteria acceptance vs Acceptance test](#criteria-acceptance-vs-acceptance-test)
* [Writing acceptance tests](#writing-acceptance-tests)
* [Properties acceptance tests](#properties-acceptance-tests)
* [Good and Bad Practices](#good-and-bad-practices)
* [Workflow ATDD](#workflow-atdd)
* [References](#references)

### What is ATDD??
The definition of wikipedia express:
> "Acceptance Test-Driven Development (ATDD) is a development methodology based on communication between the business customers, the developers, and the testers.ATDD encompasses many of the same practices as Specification by Example, Behavior Driven Development (BDD), Example-Driven Development (EDD), and Story Test-Driven Development (SDD). All these processes aid developers and testers in understanding the customer’s needs prior to implementation and allow customers to be able to converse in their own domain language. ATDD is closely related to Test-Driven Development[TDD]. It differs by the emphasis on developer-tester-business customer collaboration. ATDD encompasses acceptance testing, but highlights writing acceptance tests before developers begin coding"

Its acronym define it as test driven development of acceptance. ATDD is a requirements specification methodology that more testing methodology. ATDD is the beginning of the iterative development cycle level, because the basis of an acceptance test we deepen implementation through successive TDD unit testing to shape the code that finally meets the defined acceptance criteria.

### Based Features
ATDD methodology provides a basis features:

|Written by clients (ATDD)|
| :-------------|
| What the system does|
| Test of features|
| Business Vocabulary| 
| Without implementation detail|

### Objectives ATDD
ATDD focuses on the implementation of a completely different way to traditional methods. One of the main objectives is to provide customer ATDD rapid feedback of the progress of development by acceptance tests. The business analyst's job becomes to replace pages and pages of requirements written in natural language, for example executable consensus emerged among the various team members, including of course the client. I speak not replace all the documentation, but the requirements, which I consider a subset of the documentation. For this, a specification of less ambiguous and more specific requirements is performed by using examples of Users stories. Written great novels are left behind in defining requirements years ago. The examples do not replace the talks, it is achieved between foster these customer, testers and developers.
The methodology helps both the client understand what you want and developers understand what the customer wants specifying the behavior of each user story and avoiding the free interpretation of casuistry not covered by the specification.

### Criteria acceptance vs Acceptance test
People often make mistakes when defining the criteria and acceptance test. Often we confuse who defines the criteria and acceptance test.

* What is the difference between acceptance criteria and test?

> Criteria are the set of conditions to be met by a story to be given for good.
> The acceptance criteria consist of:
> * Actor
> * Verb (describes a behavior on the system actor)
> * Observable result

* Who should write the test for acceptance?

> The acceptance test must write the Product Owner, but unlike what many people think do not have to do alone, this methodology is based ultimately on communication and collaboration among all stakeholders of the system. We all know that the tests require a technical component that in some cases the customer can get to have it but in other cases, so the customer can ask for help from developers or QA technical aspects. The same happens in reverse when developers need help understanding the test as business rules are often confusing.

### Writing acceptance tests
The acceptance test must be automated to be meaningful in an agile environment. The tests must be specific and not allow ambiguity and avoid generic scenarios. An example of incorrect test could be "add cards to the system ", this is very generic. Instead "Add Card 4777308023346398" , making specific test.
Moreover avoid the implementation details acceptance test. An example of incorrect test could be "By introducing the card and click the Add button, a new record is created in DB" aspects are entering records databases, Web events etc. Instead "The user saves card 4777308023346398 in the payment screen" has a vocabulary of business and is not in technical parts of the system.

### Properties acceptance tests
The acceptance test must meet the following properties:

> * **SPECIFIC**: Explicitly defined and definite.
> * **MEASURABLE**: Possible to observe and quantify.
> * **ARCHIEVABLE**: Capable of existing or taking place.
> * **RELEVANT**: Having a connection with the story.
> * **TIME BOUND**: When will the outcome be observed.

### Good and Bad Practices
As best practices we can enumerate:

> * Allow the customer to add new test without breaking the build.
> * Keep acceptance test along with the code in version control system.
> * Independence : a test can not depend on others
> * Leave the system in the same state it was before his execution
> * Use tools continuous integration
> * Avoid dependencies with external systems
> * Write the test as close to real environment as possible.
> * Avoid too large or multipurpose test

As bad practices we can enumerate:

> * Developers write test of acceptance for themselves.
> * Acceptance test as write unit tests.
> * Developers write test of acceptance for themselves.
> * Write acceptance tests which are dependent on implementation details or data structures.

### Workflow ATDD
The iterative cycle ATDD:

![alt text](https://github.com/beeva-danielpetrovic/beeva-best-practices/blob/master/agile/developerTeamScrum/ATDD/static/Flujo_atdd_tdd_v3.png "WorkFlow ATDD")

The components that interact in the flow are:

> * The user stories.
> * The acceptance criteria that determine the stories.
> * Automated test criteria generated from the history.
> * The acceptance test development refined level.
> * Exploratory tests performed by the QA team.
> * Las pruebas no funcionales.

Example of use of flow ATDD-TDD:

We started in the sprint planning with one of the prioritized stories doing the questions PO team so that they are reflected all acceptance criteria. Imagine that we`re going to tokenize card, the computer can ask questions such as:

> * What happens if we try to tokenize an expired card?
> * Are all cards valid?
> * How do we know that has been tokenized card?
> * What happens if we try to tokenize a card tokenized?
> * Can you give me a card validates and invalidates tokenize?

### References

* [Link](https://www.beeva.com/beeva-view/metodologiasagiles/atdd-la-clave-del-exito-en-equipos-agiles/) Beeva ATDD

___

[BEEVA](http://www.beeva.com) | 2015

