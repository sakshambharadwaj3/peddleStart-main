## Getting Started

### Prerequisites

- Python 3.6+
- Virtualenv

### Setup

To set up the project locally on Windows, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/task_management.git
    cd task_management
    ```

2. Create a virtual environment:

    ```bash
    python -m venv venv
    ```

3. Activate the virtual environment:

    - For Command Prompt:

      ```bash
      venv\Scripts\activate
      ```

    - For PowerShell:

      ```bash
      .\venv\Scripts\Activate.ps1
      ```

4. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

5. Run the application:

    ```bash
    python main.py
    ```

The application should now be running on `http://localhost:5000`.

### API Endpoints

#### Get All Tasks

- **URL:** `/tasks`
- **Method:** `GET`
- **Success Response:**
  - **Code:** 200
  - **Content:** `[{ id, name, title, description }]`

#### Create a New Task

- **URL:** `/tasks`
- **Method:** `POST`
- **Payload:**
  ```json
  {
    "name": "Task Name",
    "title": "Task Title",
    "description": "Task Description"
  }
  ```
- **Success Response:**
  - **Code:** 201
  - **Content:** `{ id, name, title, description }`

#### Get a Single Task

- **URL:** `/tasks/<task_id>`
- **Method:** `GET`
- **Success Response:**
  - **Code:** 200
  - **Content:** `{ id, name, title, description }`

#### Update a Task

- **URL:** `/tasks/<task_id>`
- **Method:** `PUT`
- **Payload:**
  ```json
  {
    "name": "Updated Task Name",
    "title": "Updated Task Title",
    "description": "Updated Task Description"
  }
  ```
- **Success Response:**
  - **Code:** 200
  - **Content:** `{ id, name, title, description }`

#### Delete a Task

- **URL:** `/tasks/<task_id>`
- **Method:** `DELETE`
- **Success Response:**
  - **Code:** 200
  - **Content:** `{ "message": "Task deleted" }`

## Frontend

The frontend is built using HTML, CSS (Bootstrap), and JavaScript (Axios for API requests). It includes the following features:

- A landing page displaying a list of tasks.
- Ability for users to add new tasks with a name, title, and description.
- Ability for users to view detailed information about each task.
- Option to edit existing tasks.
- Option to delete tasks.
- Responsive design to ensure usability on both desktop and mobile devices.

## Running the Application

### Setup and Activation

1. **Create a virtual environment**:
   ```bash
   python -m venv venv
   ```

2. **Activate the virtual environment**:
   - For Command Prompt:
     ```bash
     venv\Scripts\activate
     ```
   - For PowerShell:
     ```bash
     .\venv\Scripts\Activate.ps1
     ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the application**:
   ```bash
   python main.py
   ```

With these instructions, you can set up and run the Task Management Application on a Windows environment manually, without the need for batch scripts.
