# Pail Math

Event orchard apple pail, week, cost and time arithmetic. The 315 apples at 8 apples a pail take 40 pails, the last pail holding 3 apples.

## Named constants

None. Every number is the owner's own entry.

## What it computes

- **The pails truth** - the apples (1 to 1000000) divided by the apples a pail (1 to 1000), rounded up, with what the last pail holds.
- **The weeks truth** - the apples divided by the apples used a week (1 to 100000), with the apples left for the next week.
- **The cost truth** - the pails (1 to 100000) times the pail price ($0.01 to $999.99) to the cent, and spread over the apples, half rounded up.
- **The time truth** - the apples divided by the apples packed a minute (1 to 100), rounded up, in minutes and in hours and minutes.

## Boundary

Arithmetic only. Counting applied as written. It has not seen any apple, pail or venue and does not know whether apples will really stay fresh, a supplier will run out or a price will hold, and it gives no verdict that a pail is worth its price or an apple is right for an event. Every number is the owner's own entry.

## Files

- `index.html` - landing page with the boundary and starting examples.
- `app.html` - the calculator; every pail recomputes on each keystroke.
- `engine.js` - the four truths, shared by the page and the tests.
- `oracle.py` - an independent Python re-implementation; writes `expected.json`.
- `test.js` - runs the engine against `expected.json` (99 cases, 20 error cases).

## Tests

```
python3 oracle.py
node test.js
```
