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
3. **Install MongoDB**: Ensure the Austin Animal Center Outcomes dataset is in a MongoDB collection and that MongoDB is operational.
4. **Set up your database connection**: Modify the credentials in the `ProjectTwoDashboard.ipynb` file.
5. **Launch the application**: Open the Jupyter Notebook and run the cells to start the dashboard. Access it through the local web server.

### Challenges Faced
- **Connection to MongoDB**: Correctly setting the authentication mechanism was initially challenging, resolved by using `pymongo` and storing sensitive credentials securely.
- **Callback Logic in Dash**: Managing interdependencies between the data table and charts required meticulous planning to ensure synchronized updates.
- **Data Visualization**: Preprocessing the data to format it correctly for display involved using `pandas` to eliminate unnecessary fields and adjust the data structure.

### Resources and Links
- [MongoDB](https://www.mongodb.com/)
- [Dash Documentation](https://dash.plotly.com/)
- [Plotly](https://plotly.com/)
- [Pandas](https://pandas.pydata.org/)
- [JupyterDash](https://medium.com/plotly/introducing-jupyterdash-811f1f57c02e)

### GitHub Repository Information

#### Maintainability, Readability, and Adaptability
Writing maintainable, readable, and adaptable programs is crucial for long-term success. The use of the CRUD Python module from Project One exemplifies this approach, as it allowed for clean interactions between the dashboard widgets and the database. This module can be reused in future projects, promoting efficiency and consistency.

#### Problem-Solving Approach
As a computer scientist, I approached the requirements for Grazioso Salvare by first gathering detailed specifications and understanding their needs. This approach emphasized thorough documentation and iterative design, differing from previous assignments that may not have required such depth. For future projects, I would implement similar strategies, ensuring I fully comprehend client requests and utilize best practices in database design.

#### The Role of Computer Scientists
Computer scientists design systems and applications that enhance productivity and effectiveness across various domains. My work on this project aids Grazioso Salvare in identifying suitable dogs for training, ultimately improving their operational efficiency and effectiveness in search-and-rescue scenarios.
