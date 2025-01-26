# Freemarket RPG Setup for Screentop.gg

This repository provides a set of JSON files and mockup PNG assets designed for use with [Screentop.gg](https://screentop.gg), enabling online play of **Freemarket**, the RPG by Jared A. Sorenson and Luke Crane.

> **Disclaimer**: I do not own the rights to Freemarket. This setup is a fan-made tool for facilitating online play. Please support Jared and Luke by purchasing the game at [Memto Mori Theatricks's store](http://memento-mori.com/pdf/freemarket-collection-pdf) or your favorite RPG retailer.

## General Overview

This setup includes the following features to help you play Freemarket online:
- **User Decks**: Customizable card decks for each player.
- **Tech Decks**: Shared or individual decks for technology cards.
- **Attaboys**: Components for representing positive feedback mechanics.

All assets are formatted to work within Screentop.gg's JSON-based configuration system, along with mockup `.png` files for visual elements. 

---

## Contents

### JSON Files
The JSON files are organized in a structure to mimic the breadcrum structure presented in screentop. Follow these steps to configure your tabletop:

1. Start by pasting the top level items into Screentop, you will need to create a set number of "dummy" object before screentop will let you paste. These are outlined below:
  - Start by creating 4 **Assets**, select all, edit, then paste **Assets.JSON** and save.
  - Start by creating 10 **Components**, select all, edit, then paste **Components.JSON** and save.
  - Start by creating 5 **Seats**, select all, edit, then paste **Seats.JSON** and save.
  - Your game should include 1 **Surfaces**, select all, edit, then paste **Surfaces.JSON** and save.
2. Click into each of the **Assets** and upload the appropriately named `.png` file.
3. Move on to the nested **Components** objects, these are any file containing a `Components>` in the file name. There are three types of Components; Cards, Holders, Attaboys.
  - **Cards**: Click into the Card Component (e.g., `Components > Challenge Card`), create the correct number of **Variants** (e.g., 45 for Challenge Cards, 10 for Tech Cards), select all, edit, then paste the (e.g., `Components>Challenge Card>Variants.json`) **.JSON** and save.
  - **Holders**: Click into the Holder Component (e.g., `Components > Card Holder`), create 1 additional **Dropzone** (there should be 2 in total), select all, edit, then paste the (e.g., `Components>Card Holder>Dropzones.json`) **.JSON** and save, click into **Dropzone 2**, then **Anchors**, create 1 **Anchor**, select all, edit, then paste the (e.g., `Components>Card Holder>Dropzone 2>Anchors.json`) **.JSON** and save.
  - **Attaboys**: Click into the Attaboy Component (e.g., `Components > Attaboy`), create 1 **Variants**, select all, edit, then paste the (e.g., `Components>Attaboy>Variants.json`) **.JSON** and save.
4. Move on to the nested **Surface** object, this is the file containing `Surface>Objects.json`. Click into Surface, then Objects, create 22 Objects, select all, edit, then paste the `Surface>Objects.json` and save.
5. Join the game as Super User and rearrange the objects so that each aligns with its space on the surface background.

### PNG Assets
The `.png` files included in this repository are rough mockups for various components of the game. These need to be uploaded as assets within Screentop.gg and associated with the correct component or variant as described in the JSON instructions above.

---

## How to Play

1. **Set Up the Room**: 
  - Create a new room in Screentop.gg from your games page.
  - Invite players by clicking the *Invite* button and sharing the copy/paste link.

2. **Player Setup**:
  - Each player has their own deck area with slots for *Draw Pile*, *In Play*, and *Discard Pile*.
  - There is a shared **Tech Deck** *Draw Pile* and *Discard Pile*, the game should limit where a Tech Card is allowed to be placed.
  - Players can only interact with their own decks, helping to keep virtual decks organized.
  - Players can pass their Attaboy token by dragging it.

3. **Super User Role**:
  - The Super User can interact with all players' decks and components.
  - This is ideal for facilitating the game, helping players, or running the game on stream without requiring other players to interact directly with Screentop.

---

## Support the Creators

Freemarket is an amazing RPG and one of my favorites. Please support Jared and Luke by [purchasing a PDF copy of Freemarket](http://memento-mori.com/pdf/freemarket-collection-pdf).

---

Please enjoy playing Freemarket online.
