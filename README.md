# J.victor

# Competitions Platform

An application for students to showcase their participation in coding competitions.

## Features

- Create Competition
- Import Competition Results from File
- View Competitions List
- View Competition Results

## Installation

### 1. Clone the Repository

```bash
git clone <your_repository_url>
cd <your_repository_folder>
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Set Up the Database

```bash
flask db init
flask db migrate
flask db upgrade
flask init
```

### 4. Run the Application

```bash
flask run
```

## CLI Commands

### 1. Create a Competition

```bash
flask competition create "Competition Name" YYYY-MM-DD --description "Description"
```

### 2. List Competitions

```bash
flask competition list
```

### 3. Import Results from File

Prepare a CSV file (e.g., `results.csv`) with the following columns:

```csv
student_name,score,rank
Alan,95.5,1
Starc,88.0,2
Charlie,82.5,3
```

To import the results:

```bash
flask result import COMPETITION_ID PATH_TO_CSV_FILE
```

### 4. View Competition Results

```bash
flask result view COMPETITION_ID
```

## Files Changed and Created

- **Modified Files**:
  - `App/models/__init__.py`
  - `App/controllers/__init__.py`
  - `wsgi.py`
  - `README.md`

- **New Files**:
  - `App/models/competition.py`
  - `App/models/result.py`
  - `App/controllers/competition_controller.py`
  - `App/controllers/result_controller.py`

---

## How to Compile and Run the Application

1. Clone the Repository

```bash
git clone <your_repository_url>
cd <your_repository_folder>
```

2. Install Dependencies

```bash
pip install -r requirements.txt
```

3. Set Up the Database

```bash
flask db init
flask db migrate
flask db upgrade
flask init
```

4. Run the Application

```bash
flask run
```

5. Use CLI Commands

Follow the instructions in the CLI Commands section of the README.md to interact with the application.
