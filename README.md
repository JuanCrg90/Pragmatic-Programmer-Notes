# Pragmatic Programmer Notes


## Table of contents
* [Chapter 1 - A Pragmatic Philosophy](#chapter1)
* [Chapter 2 - A Pragmatic approach](#chapter2)
* [Chapter 3 - The Basic Tools](#chapter3)
* [Chapter 4 - Pragmatic Paranoia](#chapter4)
* [Chapter 5 - Bend or Break](#chapter5)
* [Chapter 6 - While You Are Coding](#chapter6)


<a name="chapter1">
<h1> A Pragmatic Philosophy </h1>
</a>

## The cat ate my source code
- Take responsibility from your code.
- Don't blame provide Solutions not excuses.
- Provide options dont make lame excuses.

 
## Software Entropy
- Don't live with broken windows.

 
## Stone Soup and Boiled Frogs
- Be a catalyst for change
- The difference between the broken windows and the boiled frog is: people lose the will to fight entropy because they perceive that no one else cares. The frog just doesn't notice the change.

## Good Enough Software
- Make quality a requirements issue.
- Know when to stop. Don't spoil a perfectly good program by overembellishment and over-refinement.

## Your knowledge portfolio
- It's similar to a financial portfolio, you should to invest regularly, diversify, manage the risk, buy low sell high (early adopter) review and rebalance.

Goals
- Learn at least one. New language every year.
- Read a technical book each quarter.
- Read non technical books too.
- Take classes.
- Participate in local user groups.
- Experiment with different environments.
- Stay current.
- Get wired.

Critical thinking
- Analyze what you read and hear. You need to ensure that the knowledge in your portfolio is accurate and unswayed by either vendor or media hype.


## Communicate
- Know what you want to say.
- Know your audience (Wisdom).
  - **W**hat do you want them to learn?
  - What is ther **i**nterest in what you've got to say?
  - How **s**ophisticated are they?
  - How much **d**etail do they want?
  - Whom do you want to **o**wn the information?
  - How can you **m**otivate them to listen to you?
- Choose your moment (is this a good time to talk about ...).
- Choose a style.
- Make it look good.
- Involve your audience.
- Be a listener.
- Get back to people (It's Both What You Say and the Way That You Say It).

<a name="chapter2">
<h1> A Pragmatic Approach </h1>
</a>

## The evils of duplication
- Every piece of knowledge must have a single, unambiguous, authoritative representation within a system.
- DRY: Don't repeat yourself

## How does duplication arise?
- Imposed duplication.
- Inadverted duplication.
- Impatiend duplication.
- Interdeveloper duplication.

## Orthogonality
- In computing, the term  has come to signifify a kind of independence or decoupling.
- The helicopter controls are not orthogonal.
- The orthogonality elimiate effects between unrelated things.

## Reversibility
- There are not final decisions.

## Tracer Bullets
- Use tracer bullets to find the target.

## Prototypes ans Post-it Notes
- Prototype to learn.

## Domain Languages
- Program close to the problem domain.

## Estimating
- Estimate to avoid surprises.
- Iterate the schedule with the code.


<a name="chapter3">
<h1> The Basic Tools </h1>
</a>

> Tools amplify your talent, The better your tools, and the better you know how to use them, the more productive you can be.

## The Power of Plain Text

- Keep Knowledge in Plain Text.

## Shell Games

- Use the power of Command Shells

As a pragmatic programmer, you will constantly want to perform ad hoc operarions-things that the GUI may not support. The command line is better suited when you want to quickly conbine a couple of commands to perform a query oos some other task. 

## Power Editing
- Use a Single Editor Well (vim FTW)
> The editor will be an extension of your hand.

## Source Control
- A good source code control system helps to track changes, answering questions like: 
  - who made changes in this line of code?
  - What's the difference between the current version and last weekes?
  - How many lines of code did we change in this release?
  - Which files get changed most often?
  
## Debugging

  - Fix the problem, Not the blame.
  - Adopt the right mindset. Turn off the defenses that you use each day to protect your ego and **Don't panic**.
  - Before start to look at the bug, make sure you are working on code that compiled cleanly-without warnings.
  - Use the phrase **"Select isn't broken"** as a gentle reminder whenever you or your peers start to blame the system for a fault that is likely to be your own.
  - Remember is you see hoof prints, think horses-not zebras. The OS is probably not broken. And the database is probably fine.
  - **Don't Asume It-Prove It**

## Text Manipulation
  - Learn a Text Manipulation Language.

## Code Generators
  - Write Code that Writes Code.


<a name="chapter4">
<h1> Pragmatic Paranoia </h1>
</a>

  - You Can't Write Perfect Software

## Design By Contract
 - If all the routine's preconditions are met by the caller, the routine shall guarantee that all postconditions and invariants will be true when it completes.

## Dead Programs Tell no lies
  - Crash early.
   
## Assertive Programming
  - If It Can't happen, Use Assertions to Ensure That It Wont't.
  - Turning off assertions when you deliver a program to production is like crossing a high wire without a net because you once made it accross in practice.
## When to use exceptions
  - Use Exceptions for exceptional problems.

## How to balance resources
  - Finish What you start (memory, transactions, threads, files, timers)

<a name="chapter5">
<h1> Bend or Break </h1>
</a>

## Decoupling and the law of Demeter
  - Minimize coupling between modules.
  - Using the Law of Demeter Will make your code more adaptable and robust but at a cost: as a "general contractor" your module must delegate and manage any and all subcontractors directly, without involving clients of your module.

## Metaprogramming
  - Configure, Don't Integrate.
  - Put Abstractions in Code Details in Metadata.
  - Without metadata, your code is not as adaptable or flexible as it could be. Is this a bad thing? Well, out here in the real world, species that don't adapt die.

## Temporal Coupling
  - Analize Workflow to Improve Concurrency.
  - Design Using Services.
  - Always Design for Concurrency.

## It's Just a View
  - Separate Views from Models.
  - Model. The abstract data model representing the target object. The model has no direct knowledge of any views or controllers.
  - View. A way to interpret the model. It subscribes to changes in the model and logical events from the controller.
  - Controller. A way to control the view and provide the model with new data. It publishes events to both the model and the view.

## Blackboards
  - Use Blackboards to coordinate workflow.


<a name="chapter6">
<h1> While You Are Coding </h1>
</a>

## Programming By Coincidence
  - Don't Program by Coincidence.
  - Always be aware of what you are doing.
  - Don't code blindfolded. Attempting to build an application you don't fully understand, or to use a technology you aren't familiar with, is an invitation to be misled by coincidences.
  - Proceed from a plan, whether that plan is in your head, on the back of a cocktail napkin, or on a wall-sized printout from a CASE tool.
  - Rely only on reliable things. Don't depend on accidents or assumptions. If you can't tell the difference in particular circumstances, assume the worst.
  - Document your assumptions. Design by Contract, can help clarify your assumptions in your own mind, as well as help communicate them to others.
  - Don't just test your code, but test your assumptions as well.
  - Prioritize your effort. Spend time on the important aspects; more than likely, these are the hard parts. If you don't have fundamentals or infrastructure correct, brilliant bells and whistles will be irrelevant.
  - Don't be a slave to history. Don't let existing code dictate future code. All code can be replaced if it is no longer appropriate.
  
## Algorithm Speed
  - Estimate the Order of Your Algorithms.
  - Test Your Estimates.

## Refactoring
  - Rewriting, reworking, and re-architecting code is collectively known as refactoring.
  - When Should You Refactor?
    - Duplication.
    - Nonorthogonal design.
    - Outdated knowledge.
    - Performance. 
  - Refactor Early, Refactor Often.
  - Don't try to refactor and add functionality at the same time.
  - Make sure you have good tests before you begin refactoring. Run the tests as often as possible. That way you will know quickly if your changes have broken anything.
  - Take short, deliberate steps: move a field from one class to another, fuse two similar methods into a superclass. Refactoring often involves making many localized changes that result in a larger-scale change. If you keep your steps small, and test after each step, you will avoid prolonged debugging.

## Code That's Easy to Test
  - Design to Test.
  - All software you write will be tested—if not by you and your team, then by the eventual users—so you might as well plan on testing it thoroughly.

## Evil Wizards
  - Don't Use Wizard Code You Don't Understand.
