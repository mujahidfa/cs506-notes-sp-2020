# Sofware Engineering Processes

Date: Jan 27, 2019, Monday

## Logistics

Proposals due this **Friday (Jan 31, 2020)**
Proposal criteria:

- Usefulness
- Creativity
- Feasibility
  - enough work for 5-6 people, but not too much
  - avoid feature creep

An ideal project is:

- Core functionality is reasonably attainable, but cool features can be implemented as time permits
- warning: avoid "social" apps!

**Next deadline**:

- Monday Feb 3: proposal ranking begins
- Wednesday Feb 5: team self enrollment begins

## Clients/customers vs Users

Clients/customers are the company or entity that buys your software.

User is the actual person who's using your software.

## What is software engineering

A system of building software that needs a blueprint (i.e. the requirements)

What is SE for?

- **Two problems** we solve in SE:

  1. How will we know it works

  - From the customer vs developer perspective
    - You follow customer's requirements
    - BUT, ou want to impress the customer i.e. by making beautiful UI

  2. How will we know we developed the system efficiently

  - The project dynamics triangle: quality software, time, under budget.
    - If time/cost is low, then quality is low
    - If time/quality is high, then cost is high

## Software engineering layers

**Tools**: automate processes and methods

- front/back end framework (Vue, Rails etc), testing (Jest, Mocha etc)

**Methods**: technical "how to"

**Process**: framework utilized

- Waterfall, agile etc

## SE Process

SE boils down to several steps:

- Planning: How do we determine if it is a feasible project?
- Specification: How do we know what the client wants done?
- Design: How do we develop an efficient outline for doing it?
- Programming: How do we “do” it?
- Validation: Can we check that was delivered is what was wanted?

The first engineering process was the **waterfall method**.

## **Waterfall method**

- First version had no iteration
- Process: Planning->requirements->design->implementation->testing->product delivery->maintenance
- **Pros**:
  - great for 10k lines of code
  - very structured and linear approach
  - emphasis on understanding the project before you did it
  - documentation heavy
  - good for large systems with a large team
- **Cons**: assumes the client does not change their mind

  - does not take into account change in user requirement
  - relies heavily on being able to accurately assess requirements from the start
    - What happens when client requests a new requirement was that you have to complete the process until the end (version 1) before starting back from the beginning again to satisfy the new requirement (version 2)
  - super time consuming, very costly for clients

Next, was the **Evolutionary Model** i.e. **Rapid Application Development (RAD)** method.

## **Evolutionary Model**

- very little documentation while very quick in prototyping
- clients will receive many versions/drafts to give feedback
- however, during the drafts, they avoided documentation until the final draft
- **Pros**:
  - good for short lifespan apps
  - small/medium-size interactive systems
  - very quick prototyping; clients get to see early on what their app will look like
- **Cons**:
  - lack of process visibility
  - lack of documentation

## **Iterative model**

Iteratively approach building the software little-by-little, pushing features to the next iteration.

Has the best of both worlds: allow requirement change, documentation heavy, while having prototypes for the client.

**Pros**:

- system functionality is available for the client earlier
- lower the risk of project failure
  - allows clients to have better introspection on whether a requirement is truly needed given the cost and time
- highest priority functionalities tend to receive the most testing
- early iterations act as prototype to help elicit requirements for later iterations
