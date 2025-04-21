# RogueDoc

API documentation generator for Rogue.

About     | Current Release
----------|-----------------------
Version   | 1.3
Date      | April 20, 2025
Platforms | Windows, macOS, Linux
Author    | Brom Bresenham

# Installation

## Morlock Install

1. Install [morlock.sh](https://morlock.sh)
2. `morlock install brombres/vimage`

Update an existing installation with `morlock update vimage`

## Manual Build

1. Install [Rogue](https://github.com/brombres/Rogue) and [Rogo](https://github.com/brombres/rogo).
2. `rogo build`
3. `rogo install`

# Usage

## Generating Standard Library Documentation

    > roguec --doc
    Writing documentation metadata to API.json

    > roguedoc API.json --output=Wiki --split
    Generating documentation...
      Wiki/API.md
      Wiki/Codec-Library-API.md
      Wiki/Collection-Library-API.md
      Wiki/Console-Library-API.md
      Wiki/Control-Library-API.md
      Wiki/Core-Library-API.md
      Wiki/DateTime-Library-API.md
      Wiki/FileIO-Library-API.md
      Wiki/Geometry-Library-API.md
      Wiki/Graphics-Library-API.md
      Wiki/Introspection-Library-API.md
      Wiki/IO-Library-API.md
      Wiki/Math-Library-API.md
      Wiki/Network-Library-API.md
      Wiki/Standard-Library-API.md
      Wiki/StandardMacros-Library-API.md
      Wiki/UI-Library-API.md
      Wiki/Utility-Library-API.md

## Generating Rogue Project Documentation

"RogueDoc" is used as the example project.

    ~/Projects/Tools/RogueDoc> roguec --doc=Source --output=RogueDoc
    Writing documentation metadata to RogueDoc.json

    ~/Projects/Tools/RogueDoc> roguedoc RogueDoc.json --output=Wiki
    Generating documentation...
      Wiki/API.md
