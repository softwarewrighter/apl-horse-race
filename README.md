# APL Horse Race

A recreation of the classic horse race simulation from the APL\360 era (1970s), demonstrating APL's array programming paradigm.

![APL Race Listing](images/race-apl-listing.png)

## Overview

This project contains two implementations of a horse race simulation:

- **[src/race.apl](src/race.apl)** — Verbose version with explicit variable declarations; better for learning APL
- **[src/idiomatic-race.apl](src/idiomatic-race.apl)** — Compact version demonstrating terse, idiomatic APL style

## Documentation

- [Verbose Race Explained](docs/race-apl-explained.md) — Comprehensive line-by-line breakdown with historical context
- [Idiomatic Race Explained](docs/idiomatic-race-explained.md) — Explanation of the compact implementation

## Installing GNU APL

### macOS (Homebrew)

```bash
brew install gnu-apl
```

### Arch Linux (yay)

```bash
yay -S gnu-apl
```

## Running the Demos

```bash
# Run the verbose/educational version
apl -f src/race.apl

# Run the compact idiomatic version
apl -f src/idiomatic-race.apl
```

Requires a Unicode-capable terminal.

## Sample Output

APL uses special glyphs (⍴, ⍳, ∇, ⎕, ←, etc.) that may not display correctly without Unicode fonts. PNG versions are provided to ensure visibility:

| Version | Source Code | Sample Output |
|---------|-------------|---------------|
| Verbose | [race.apl](src/race.apl) ([PNG](samples/race-source.png)) | [Text](samples/race-output.txt) / [PNG](samples/race-output.png) |
| Idiomatic | [idiomatic-race.apl](src/idiomatic-race.apl) ([PNG](samples/idiomatic-race-source.png)) | [Text](samples/idiomatic-race-output.txt) / [PNG](samples/idiomatic-race-output.png) |
