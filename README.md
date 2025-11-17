README
Overview

This repository contains an anonymised demonstration notebook illustrating the analytical logic behind a regain to progression workflow in football event data. The aim is to provide a clear and transparent example of how raw event information can be processed, structured, and transformed into meaningful tactical insights. All data used in the notebook is synthetic and generated within the file, and no external or proprietary information is required.

The notebook follows the same principles and methodological structure that I apply in professional and academic analysis projects. It offers a simplified yet representative walkthrough of how regain actions are identified, how subsequent progressions are detected and linked, and how this information can be visualised to understand team behaviours in possession and during transitions.

What the Notebook Demonstrates

The notebook is organised to reflect a typical football data analysis workflow and includes the following stages:

Data Inspection and Validation

Initial checks are performed on the event dataset to ensure column completeness, coordinate consistency, time structure, and team identification. This establishes a reliable foundation before deriving any tactical metrics.

Normalisation

Event coordinates are standardised to a 105 by 68 metre pitch, and the game clock is converted into a continuous 0 to 5400 second scale. Team direction is also standardised to ensure that all visualisations and metrics follow a consistent orientation.

Regain Identification

The notebook identifies defensive ball recovery actions, such as interceptions, duels, and loose ball recoveries. These moments represent the starting point of the regain to progression sequence.

Progression Identification

Actions that move the ball forward or laterally, such as passes, carries, and dribbles, are detected and classified. The code establishes criteria that distinguish between forward, backward, and lateral movement.

Regain to Progression Linking

A regain is linked to the first meaningful progression that occurs shortly afterwards. This creates regain to progression chains that can be counted, grouped, and analysed across pitch zones, time periods, or player roles.

Categorisation Layers

Each event is assigned a pitch third (defensive, middle, attacking), a corridor (wide, half-space, central), and a time segment within the match. These labels help contextualise behaviours and support the creation of structured reports.

Example Visualisation

The notebook concludes with a demonstration heatmap that uses synthetic data to illustrate progression density and average directional movement following regains in the opponent’s half. This mirrors the type of visual explanation often included in match reports or opposition analysis.

Relevance

This notebook reflects how I organise and explain analytical processes related to football events. Although simplified, the workflow mirrors practical conditions, emphasising data structure, metric development, and communication of insights. It is designed to demonstrate analytical clarity and methodological thinking rather than to replicate any specific dataset or match situation.

Running the Notebook

The notebook is self-contained. It uses only Python standard scientific libraries and generates its synthetic dataset internally. It can be executed in Jupyter Notebook, JupyterLab, or Visual Studio Code without any additional data sources.

Repository Contents

regain_progression_demo.ipynb
Main notebook containing the full demonstration workflow.

README.md
Project overview and instructions.
