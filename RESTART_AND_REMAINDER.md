# Restart And Remainder

## Restart Logic

Restart is the rule for what happens when direct continuation cannot proceed on the current local chart, normalization, or state representation.

A serious architecture must answer:

- when is restart triggered,
- what data is preserved,
- what normalization is performed,
- what prevents restart accumulation or Zeno failure,
- what certifies legal re-entry.

This is why restart logic is part of the method rather than an implementation detail.

## Remainder Discipline

The remainder is the complement of the constrained sector.
It is the part of the problem that is not yet closed by the projected core.

The method requires:

- naming the remainder,
- preserving it as a first-class object,
- stating what is known and unknown about it,
- refusing to treat it as zero unless a gate actually closes it.

## Parent Decomposition

A canonical way to say this is:

- `X = X_mc uplus R`
- `P_mc X` is the constrained sector
- `Q_rem X = R` is the tracked remainder

This decomposition blocks a common failure mode of advanced reasoning: silently converting a local closure statement into a global one by forgetting the complement.

## Why This Matters

Restart without remainder becomes procedural folklore.
Remainder without restart becomes static bookkeeping.
The architecture needs both.
