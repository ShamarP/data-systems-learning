# Reliability

## What this concept means (in my own words)
Reliability is how well the system performs as intended, even when unexpected issues arise.

## Why this concept matters

Reliability is important when designing a system as users are relying on you to provide a service. If the service goes down this is a loss of productivity or revenue and can harm your reputation. 

## Core ideas
- Faults vs Failiure: 
	- Fault is when a component isn't operating as intended
	- Failure is when the system goes down.
- Types of Faults:
	- Hardware: Hard disks crashing, power goes out. Solution to this is adding redundancy in hardware components when possible
	- Software Errors: Bug that causes app to crash when given bad input.No quick solution to this just carefully understanding the requirements of this system.
	- Human error: errors cause by people using the system. Designing systems that encourages users to do the right things is one solution.

## Simple example

An alarm clock app that goes off every morning at the time you set, even after your phone restarts overnight.

## Real-world systems that use this
- Redundancy in Databases -> Replicating data over multiple disks
- Netflix lowers video quality when bandwidth drops instead of stopping playback.
- Microservices isolate failures to one service -> This contains the blast radius of a failure

## Tradeoffs / limitations
- Things break and it's impossible to make a system completely fault tolerant.

## Related concepts

## Misunderstandings I corrected


## Questions I still have
- What do you look for when making a system reliable?
