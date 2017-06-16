# cppcon17_coroutines_what_cant_they_do
Proposal for CppCon 2017 talk

## Titles

* Ain't no party like a coroutine party 
* Coroutines: what _can't_ they do? 
* Coroutines: They're not just for async and generators anymore! 
* Coroutine all the things!
* You won't believe what coroutines can do!
* Stretching the Coroutines TS to breaking point

## Abstract (scary version)

Coroutines are coming. They're coming for your asynchronous operations. They're coming for your lazy generators. This much we know. But once they're here, will they be satisfied with these offerings? They will not. They will require feeding, lest they devour our very souls. We present some fun ways to keep their incessant hunger at bay. I, for one, welcome our new coroutine overlords.

## Abstract (boring version)

The Coroutines Technical Specification is an experimental extension to the C++ language that allows functions to be suspended and resumed, with the primary aim of simplifying code that invokes asynchronous operations. We present a short introduction to Coroutines followed by some possibly non-obvious ways they can help to simplify your code.

Have you ever wanted to elegantly compose operations that might fail? Coroutines can help. Have you ever wished for a zero-overhead type-erased function wrapper? Coroutines can help. We show you how and more.

## Outline

### Part 1. Introduction
* Introduction to Coroutines
* Generators
* Async
### Part 2. Weird and Wacky 
* Expected
  * Try to stay neutral on the various competing implementations 
* Type erasure
  * Gor's function thingy
* Wrapping function entry/exit
  * Instead of suspending, just log
### Part 3. Speculative Extensions 
* Cloning - not yet proven feasible
  * List comprehensions
  * Go Full Monad!
* Stackfullness
  * Maybe point out problems with hidden suspensions?
