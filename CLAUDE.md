# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

APL Horse Race - an educational project demonstrating APL array programming through a horse race simulation. Recreates a classic program from the APL\360 era (1970s).

## Running the Code

Requires GNU APL interpreter installed with a Unicode-capable terminal.

```bash
# Run the verbose/educational version
apl -f src/race.apl

# Run the compact idiomatic version
apl -f src/idiomatic-race.apl

# Interactive with timeout (useful for testing)
timeout 30 apl --script -f src/idiomatic-race.apl
```

## Architecture

Two implementations of the same race simulation:

- **src/race.apl** - Verbose version with explicit variable declarations and separate functions; better for learning APL
- **src/idiomatic-race.apl** - Compact version demonstrating terse, idiomatic APL style

**Core algorithm:**
1. Initialize 5 horses at position 0, finish line at 15
2. Loop: add random 1-3 to each position (vectorized: `POS←POS+?5⍴3`), display progress, check for winner
3. Announce winner and exit

**Key APL constructs used:**
- `⍴` reshape, `?` roll (random), `/` reduce, `⊃` pick, `←` assignment
- `⎕←` output, `⎕DL` delay, `→` branch with labels

## Documentation

Detailed line-by-line explanations in `/docs/`:
- `race-apl-explained.md` - comprehensive breakdown of verbose version
- `idiomatic-race-explained.md` - explanation of compact version
