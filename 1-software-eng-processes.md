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

## Software Development Lifecycle/Process

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

We understand some requirements, we design/develop it, we let the client see it, then we iteratively add new features according to the client.

Has the best of both worlds: allow requirement change, documentation heavy, while having prototypes for the client.

- comes about because we are starting to develop UI sites
- so, it needs small increments of improvements so that customers can see the product piece-by-piece before it is finished

**Pros**:

- system functionality is available for the client earlier
- lower the risk of project failure
  - allows clients to have better introspection on whether a requirement is truly needed given the cost and time
- highest priority functionalities tend to receive the most testing
- early iterations act as prototype to help elicit requirements for later iterations

**Cons**:

- The client doesn't necessarily know what they want so it's hard to find a direction.
- Requires clients to be present (not suitable for remote).
- A lot more work than it has to be.

### **Agile (Extreme programming or Scrum)**

Approach development through very small increments of functionality.

Relies on constant code improvement, user/client involvement in the dev team and pairwise programming.

Agile, in practice, uses a version of Waterfall/Extreme in between because it works better and faster. A lot of companies have their own flavor.

## **Spiral method**

Process is represented as a **spiral** rather than as a sequence of activities with backtracking.

Each loop in the spiral represents a phase in the process.

No fixed phases such as specification or design.

Loops in the spiral are chosen depending on what is required.

Risks are explicitly assessed and resolved throughout the process.

Steps:

1. Set specific objectives
2. Assess risks and put activities in place to mitigate those risks
3. Choose a development model for the system (can be any of the generic models, very depends on the system)
4. Review the projects and plan the next phase of the spiral

Microsoft uses Spiral because they have so many systems to support so they have to be backwards compatible (i.e. Windows updates).

**Pros**:

- Good for mission critical or highly sensitive systems i.e. military/medical apps
- The only software process model that has explicit risk management
- Extensive documentation
- Multiple versions of the system can be developed

**Cons**:

- There's no "clear" end to the project
- Can get very expensive
- Process is risk averse/reluctant (pro/con?)

## **Extreme programming/Scrum (XP)**

XP is like Iterative but taken to the extreme.

- A lot more iterations because every iteration has only little scope to cover and small functionality.
- Shorter development cycles/sprints (2-4 week development cycles)
- No break between iterations to meet clients.

### Cycle

1. Meet with clients to elicit requirements.

   - User stories/backlog items + acceptance test: acceptance test is to ensure it is something the user can do.
   - User stories is what the user wants in detail.

2. Planning

   - Break stories into tasks and estimate costs i.e. how much effort needed to complete the task. The effort is based on previous baselines (i.e. effort points).
   - Best if client gives their story priorities because if software is shipped not complete, at least the client can be satisfied.

3. Implementations

   - Write unit tests first
   - Write simplest code to pass the tests
   - Refactor code
   - Pair programming

4. Finish one part and iterate the process

### XP Customer

Have them as direct communication with the client.

### User stories

Have small Kanban boards that have user stories, and start asking what-if questions for specific details. We don't include implementation detail here (i.e. use Axios to call apis)

### Acceptance tests

Almost like unit tests, we build tests that test the interaction between functionalities.

### Planning game

**Pros**:

- Code developed earlier has better quality because it gets tested multiple times on every iteration after it.

## **Conclusion**

1. If requirements are poorly understood or expected to change, best use a process with flexibility like Evolutionary, Iterative, Agile.

2. If a big software system has so many moving parts that depend on each other, best use a sequential process like Spiral.

3.

### Mixed processes

- With Spiral, new components may be developed using any of the 3 other methods
- When UIs have to be tested by users, we will have to use a version of Iterative.
