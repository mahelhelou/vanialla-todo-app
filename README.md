# Documentation

## About This Project

This project is a simple Todo application built in using vanilla JavaScript and have many features.

The project is a clone of [Ed's Todo List](https://github.com/developedbyed/vanilla-todo), but I added more features, cleaned the code and, of course, wrote a documentation.

If you founded this project helpful, please support me by buying a service I provide on [Fiverr](https://fiverr.com/mahelhelou).

## Todo App Features (Vanilla JavaScript)

- Add a todo
- Delete a todo
- Update a todo
- Filter todos
  - Completed todos
  - Uncompleted todos
- Keep the todo list stored in the `localStorage`

## App HTML Code

- Create a header for the app title
- Create a todo structure
  - Input to add the todo text
  - Button to push the todo input's value
- Create a todo filter (Select)
  - Show all todos (All)
  - Show completed todos
  - Show uncompleted todos
- Create a todo list container
  - Push a todo item inside it
  - Every todo item should have
    - Check icon to mark the todo as completed
    - Delete icon to delete the todo

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Vanilla Todo List</title>
		<link href="https://fonts.googleapis.com/css?family=Poppins&display=swap" rel="stylesheet" />
		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.12.1/css/all.min.css" integrity="sha256-mmgLkCYLUQbXn0B1SRqzHar6dCnv9oZFPEC1g1cwlkk=" crossorigin="anonymous" />
		<link rel="stylesheet" href="./style.css" />
	</head>

	<body>
		<header>
			<h1>Vanilla Todo List</h1>
		</header>
		<form>
			<input type="text" class="todo-input" />
			<button class="todo-button" type="submit">
				<i class="fas fa-plus-square"></i>
			</button>
			<div class="select">
				<select name="todos" class="filter-todo">
					<option value="all">All</option>
					<option value="completed">Completed</option>
					<option value="uncompleted">Uncompleted</option>
				</select>
			</div>
		</form>
		<div class="todo-container">
			<ul class="todo-list"></ul>
		</div>

		<script src="./app.js"></script>
	</body>
</html>
```
