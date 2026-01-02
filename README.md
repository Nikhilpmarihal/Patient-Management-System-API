# Patient Management System API

A FASTAPI-based application for managing patient records efficiently. This API allows for creating, reading, updating, and deleting patient data, stored in a local JSON file.

## Features

- **CRUD Operations**: Complete management of patient records (Create, Read, Update, Delete).
- **Data Validation**: Uses Pydantic models to ensure data integrity for fields like age, height, weight, and gender.
- **Computed Fields**: Automatically calculates BMI and provides a health verdict (Underweight, Normal, Obese, etc.).
- **Sorting**: Ability to sort patients by height, weight, or BMI in ascending or descending order.
- **Local Storage**: Persists data in a `patients.json` file.

## Tech Stack

- **Framework**: FastAPI
- **Language**: Python
- **Data Validation**: Pydantic
- **Server**: Uvicorn

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Nikhilpmarihal/Patient-Management-System-API.git
   cd Patient-Management-System-API
   ```

2. **Create a virtual environment (optional but recommended):**

   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS/Linux
   source .venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the server:**

   ```bash
   uvicorn main:app --reload
   ```

2. **Access the API:**
   Open your browser and navigate to `http://127.0.0.1:8000`.

3. **Explore the Documentation:**
   FastAPI provides automatic interactive documentation. Visit:
   - **Swagger UI**: `http://127.0.0.1:8000/docs`
   - **ReDoc**: `http://127.0.0.1:8000/redoc`

## API Endpoints

### General

- `GET /`: Welcome message.
- `GET /about`: Description of the API.

### Patient Operations

- `GET /view`: Retrieve all patient records.
- `GET /patient/{patient_id}`: Retrieve a specific patient by ID.
- `POST /create`: Create a new patient record.
- `PUT /edit/{patient_id}`: Update an existing patient's details.
- `DELETE /delete/{patient_id}`: Delete a patient record.

### Utilities

- `GET /sort`: Sort patients by specific criteria (`height`, `weight`, `bmi`) and order (`asc`, `desc`).

## Project Structure

- `main.py`: The main application file containing API endpoints and logic.
- `patients.json`: JSON file used for data storage.
- `.gitignore`: Specifies intentionally untracked files to ignore.
