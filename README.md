# Traveler's Guide

Welcome to the Traveler's Guide repository! This Python script provides a simple tool for travelers to discover attractions in various destinations based on their interests.

## How it Works

The `script.py` file in this repository contains functions to manage a list of destinations and their attractions. Here's a breakdown of its functionalities:

1. **Destination Management**: 
   - The `destinations` list holds the names of different destinations.
   - You can add attractions to each destination using the `add_attraction()` function.

2. **Attraction Retrieval**:
   - The script allows users to find attractions in a specific destination based on their interests.
   - You can use the `find_attractions()` function to retrieve attractions matching certain interests in a given destination.

3. **Traveler Recommendations**:
   - By providing a traveler's destination and interests, the script suggests attractions they might enjoy.
   - The `get_attractions_for_traveler()` function generates personalized recommendations for travelers.

## Usage

1. **Adding Attractions**:
   - To add attractions to a destination, use the `add_attraction(destination, attraction)` function.
   - Provide the destination name and a list containing the attraction name and its associated interests.

2. **Finding Attractions**:
   - Use the `find_attractions(destination, interests)` function to search for attractions in a destination.
   - Input the destination name and a list of interests to filter attractions.

3. **Getting Recommendations**:
   - For personalized recommendations, utilize the `get_attractions_for_traveler(traveler)` function.
   - Input the traveler's name, destination, and interests to receive tailored suggestions.

## Example

Here's an example of how to use the script:

```python
# Add attractions
add_attraction("Paris, France", ["the Louvre", ["art", "museum"]])

# Find attractions in a destination
attractions_in_paris = find_attractions("Paris, France", ["art"])

# Get recommendations for a traveler
traveler_recommendations = get_attractions_for_traveler(['John Doe', 'Paris, France', ['art']])
print(traveler_recommendations)
