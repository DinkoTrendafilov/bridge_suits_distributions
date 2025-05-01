# Bridge Suit Distribution Analyzer

![Bridge Distributions Visualization](bridge_distributions.png)

This Python script calculates and visualizes all possible suit distributions in a 13-card bridge hand, showing how cards are divided among the four suits (Spades, Hearts, Diamonds, Clubs).

## Features

- Calculates all possible 13-card suit distributions from a 52-card deck
- Determines the probability of each specific distribution
- Analyzes symmetry variants (how many equivalent distributions exist)
- Generates a formatted table of the most common distributions
- Creates a horizontal bar chart visualization of the top 20 distributions
- Provides detailed statistics about distribution types

## Mathematical Background

In bridge, the standard deck has:
- 4 suits (Spades, Hearts, Diamonds, Clubs)
- 13 cards in each suit
- 52 cards total
- Each player gets 13 cards

The number of possible hands is C(52,13) = 635,013,559,600.

Each distribution is represented as a 4-tuple (S,H,D,C) showing how many cards are in each suit.

## Variant Analysis

Distributions can be symmetric in different ways:
- **24 variants**: All four suit lengths different (e.g., 5-4-3-1)
- **12 variants**: Two suits share the same length (e.g., 5-4-3-1)
- **6 variants**: Two pairs of suits with same lengths (e.g., 4-4-3-2)
- **4 variants**: Three suits share same length (e.g., 4-3-3-3)
- **1 variant**: All four suits same length (only possible with 3-3-3-4)

## Usage

1. Ensure you have Python 3 installed
2. Install required dependencies:

pip install matplotlib numpy

3. Run the script:

python bridge_suit_distribution.ipynb
