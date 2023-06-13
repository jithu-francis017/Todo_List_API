# TodoLists Django Rest Framework Project

This project is a TodoLists application built using Django Rest Framework. It allows users to manage their tasks by performing CRUD operations (Create, Read, Update, Delete) through a RESTful API.


   The project will be accessible at [https://todo-lists-api-lyp3.onrender.com/]([http://127.0.0.1:8000/](https://todo-lists-api-lyp3.onrender.com/)).

## API Endpoints

The following API endpoints are available for managing tasks:

### 1. Create a Task

- **URL**: ``
- **Method**: POST
- **Parameters**: None
- **Request Body**:

  ```json
  {
    "owner": "<int>"
    "title": "Task Title",
    "description": "Task Description"
  }
  ```

- **Response**:

  - Status: 201 CREATED
  - Body:

    ```json
    {
      "owner": "1"
      "title": "Task Title",
      "description": "Task Description"
    }
    ```

### 2. Get All Tasks

- **URL**: ``
- **Method**: GET
- **Parameters**: None
- **Response**:

  - Status: 200 OK
  - Body:

    ```json
    [
      {
        "owner": "1"
        "title": "Task Title",
        "description": "Task Description"
      },
      ...
    ]
    ```

### 3. View a Task

- **URL**: `/tasks/<int:pk>/`
- **Method**: GET
- **Parameters**:
  - `pk`: The ID of the task
- **Response**:

  - Status: 200 OK
  - Body:

    ```json
    {
      "owner": "1"
      "title": "Task Title",
      "description": "Task Description"
    }
    ```

### 4. Update a Task

- **URL**: `/tasks/<int:pk>/`
- **Method**: PUT/PATCH
- **Parameters**:
  - `pk`: The ID of the task
- **Request Body**:

  ```json
  {
    "owner": "1"
    "title": "Updated Task Title",
    "description": "Updated Task Description"
  }
  ```

- **Response**:

  - Status: 200 OK
  - Body:

    ```json
    {
      "owner": "1"
      "title": "Updated Task Title",
      "description": "Updated Task Description"
    }
    ```

### 5. Delete a Task

- **URL**: `/tasks/<int:pk>/`
- **Method**: DELETE
- **Parameters**:
  - `pk`: The ID of the task
- **Response**:

  - Status: 204 NO CONTENT

## Contribution

Contributions to this project are welcome. If you find any issues or want to suggest improvements, please open an

 issue or submit a pull request to the [repository](https://github.com/jithu-francis017/Todo_List_API).

## License

This project is licensed under the [MIT License](LICENSE).
