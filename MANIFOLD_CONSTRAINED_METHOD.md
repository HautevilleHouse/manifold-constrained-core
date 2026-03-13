# Manifold-Constrained Method

## Purpose

The manifold-constrained method is a public architecture for making local-to-global reasoning explicit.
It is designed to expose the load-bearing structure of a proof, model, control law, or constrained system instead of leaving that structure implicit in prose or folklore.

## Canonical Shape

### 1. Admissible class

Specify the states, objects, or trajectories on which the method is defined.
The admissible class is not decorative. It is the legal domain of the architecture.

### 2. Projected core

Isolate the part of the system that carries the stable or coercive structure.
This may appear as a projected operator, constrained state sector, protected invariant, or comparison core.

### 3. Transport or continuation law

Define how local information moves.
The architecture requires an explicit law for how quantities propagate under deformation, iteration, evolution, or routing.

### 4. Restart logic

When direct continuation is not enough, the architecture must say how normalization, restart, surgery, or re-entry works.
A failure to define restart is a failure to define the method.

### 5. Remainder discipline

The unresolved or uncontrolled part is never dropped.
The method requires an explicit remainder, complement, or residual channel and an account of how it behaves.

### 6. Bridge or identification

The architecture must explain how the internal constrained object identifies with the intended external object.
Without an explicit bridge, closure inside the method does not automatically transfer outside it.

### 7. Final margin

Closure requires a nondegenerate endpoint condition.
In many theorem lanes this is a strict scalar margin. In other domains it may be a certificate, separation bound, or stability surplus.

## Generic Schematic

Let `X` denote the full domain and `X_mc` the manifold-constrained sector.

- `X = X_mc uplus R`
- `P_mc` projects onto the constrained sector
- `Q_rem = I - P_mc` tracks the remainder
- local continuation operates on `X_mc`
- restart keeps the process inside an admissible region
- final closure requires the remainder to be controlled rather than ignored

## Why The Method Is General

The same causal shape can appear in:

- theorem architecture,
- AI model design,
- control systems,
- physical constraint systems,
- large technical platforms.

The specific objects change. The architectural roles do not.
