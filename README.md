# Grazioso Salvare Rescue Dog Dashboard

## Overview of the Project

This project is a web-based dashboard designed for Grazioso Salvare, an international rescue-animal training company. The dashboard enables users to visualize canine data for identifying and categorizing potential search-and-rescue candidates by connecting to the Austin Animal Center Outcomes database hosted on MongoDB. 

### Key Features:
- **Interactive Filter Options**: Users can filter by rescue types including:
  - Reset
  - Disaster/Individual Tracking
  - Mountain/Wilderness Rescue
  - Water Rescue
- **Dynamic Data Table**: Displays unfiltered animal data that adapts to filtering settings.
- **Geolocation Chart**: Visualizes animal locations based on the selected data.
- **Breed Breakdown**: A pie chart illustrating the distribution of breeds according to the selected rescue type.

### Screenshots:
*Include screenshots of the dashboard here.*

## Tools and Technology

### MongoDB
The Austin Animal Center Outcomes data is stored in MongoDB, which serves as the model component of the application. MongoDB provides:
- **Flexibility**: Efficiently manages semi-structured and unstructured data.
- **Python Integration**: The `pymongo` module allows for smooth CRUD operations in Python.
- **Scalability**: Capable of handling large datasets effectively, which is crucial for managing data across multiple animal shelters.

### Dash Framework
The view and controller layers of the dashboard are implemented using Dash. Its advantages include:
- **Interactivity**: Easily creates interactive data visualizations without extensive front-end development knowledge.
- **Integration with Plotly**: Seamlessly creates charts and graphs for data visualization.
- **Support for Jupyter Notebooks**: Facilitates dashboard development and testing within Jupyter.

### Python Libraries Used:
- `pandas` for data manipulation.
- `pymongo` for MongoDB interaction.
- `dash`, `dash_table`, and `dash_leaflet` for dashboard components.

## Project Setup

To replicate this project, follow these steps:

1. **Download the project files** or clone the repository.
2. **Install the necessary libraries**:
   ```bash
   pip install dash pandas plotly dash-leaflet pymongo
