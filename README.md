# To-Do Terminal Application

This is a simple To-Do application for the terminal, written in Go. The application allows users to add, complete, delete, and list their tasks. The tasks are stored in a JSON file, ensuring persistence across sessions.

## Features

- **Add tasks**: Create new tasks with a description.
- **Complete tasks**: Mark tasks as completed.
- **Delete tasks**: Remove tasks from the list.
- **List tasks**: Display all tasks with their status and timestamps.

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/todo-app.git
    cd todo-app
    ```

2. Build the application:
    ```sh
    go build ./cmd/todo
    ```

## Usage

Run the `todo` command with the appropriate subcommands:

- **Add a new task:**
    ```sh
    ./todo -add "Your task description"
    ```

- **Complete a task:**
    ```sh
    ./todo -complete [task number]
    ```

- **Delete a task:**
    ```sh
    ./todo -del [task number]
    ```

- **List all tasks:**
    ```sh
    ./todo -list
    ```

### Example

```sh
# Adding tasks
./todo -add "Demo analysis"
./todo -add "Presentation"

# Listing tasks
./todo -list

# Completing a task
./todo -complete 2

# Deleting a task
./todo -del 1

# Listing tasks again
./todo -list


