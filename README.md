# PetrolPump-Management-System [DBMS] Implementation Environment

## Frontend

The frontend of this project is built using the well-known Python library, Streamlit.

Streamlit is an open-source framework in Python designed for creating web applications for data science and machine learning quickly. It integrates seamlessly with major Python libraries like scikit-learn, Keras, PyTorch, SymPy (latex), NumPy, pandas, Matplotlib, and more.

With Streamlit, CRUD (Create, Read, Update, Delete) operations can be easily performed.

A custom function calculates the total price in the Tanker table, and a trigger in the Employee table activates when someone tries to update the salary field, ensuring the salary is not less than 300,000.

## Backend

The backend involves creating and populating tables in MySQL. It utilizes libraries such as Pandas, SQL Connector, and Streamlit, with the primary development language being Python.

## Project File Structure

The project folder contains the following files:

- **create_database.py**: Creates the `Petrolpump_Management` database.
- **app.py**: The main file to execute after database creation, containing the GUI code.
- **databases.py**: Includes all essential function calls.
- **create.py**: Adds new rows to the tables.
- **delete.py**: Implements functionality to delete specific rows from the tables.
- **read.py**: Reads data from the tables and sends it to the view function for display.
- **update.py**: Updates data in the tables.

## How to Run

1. Create the database by running `create_database.py`.
2. Install all required libraries.
3. Execute the `app.py` file using the command:
   ```
   python -m streamlit run app.py
   ```
