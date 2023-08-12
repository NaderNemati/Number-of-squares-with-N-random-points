# Counting Squares with N Random Points

Welcome to the **Counting Squares with N Random Points** repository. This project delves into the intriguing realm of geometric exploration, employing dynamic programming principles to analyze the relationships between random points in a plane and the formation of squares. Through a systematic approach, this endeavor offers insights into the patterns and possibilities inherent in geometric configurations.

## Unveiling Geometric Insights

The exploration commences with the generation of random points within a plane. Leveraging the power of dynamic programming, a novel idea is introduced: Fixing two points (X1, Y1) and (X2, Y2) and systematically iterating through pairs of fixed points. By rotating the vector connecting these points by 90 degrees, two additional points of a square can be deduced using the following equations:

X3 = X1 + (Y2 − Y1)
X4 = X2 + (Y2 − Y1)
Y3 = Y1 + (X1 − X2)
Y4 = Y2 + (X1 − X2)


It's worth noting that the initial time complexity of this approach is approximately O(n^4). However, through an astute optimization strategy, the points are sorted using a dictionary at the outset, resulting in a significant reduction of the time complexity to O(n^2).

## Methodical Exploration and Validation

The exploration journey embarks with a meticulous validation process. To establish the integrity of the approach, the code is initially executed for nine fixed points, with results carefully examined. Subsequently, the algorithm is tested with N randomly generated points, and the rich tapestry of possibilities begins to unfold.

Remarkably, the analysis reveals that for the fixed points:
(0, 0), (2, 2), (0, 2), (2, 0), (4, 2), (4, 0), (2, 4), (0, 4), (4, 4),

Five distinct squares emerge as feasible configurations. Furthermore, the program extends its computational prowess to ascertain that a total of 29 possible squares materialize when 50 random points are generated (referenced in the Python code).

## Engage and Collaborate

Embark on an exciting journey through the realm of geometric configurations. Dive into the code, immerse yourself in the dynamics of point manipulation, and uncover the intriguing world of squares formed by random points. Your involvement in this repository is both valued and encouraged, as we collectively unravel the captivating interplay between geometry and randomness.

For inquiries, collaborations, or insights, please connect with [Nader Nemati](mailto:nnevar@utu.fi).
