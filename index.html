<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>To-Do App</title>

  <style>
    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family: Arial, sans-serif;
    }

    body{
      background:#f3f4f6;
      display:flex;
      justify-content:center;
      align-items:center;
      min-height:100vh;
    }

    .container{
      width:400px;
      background:white;
      padding:25px;
      border-radius:12px;
      box-shadow:0 4px 12px rgba(0,0,0,0.1);
    }

    h1{
      text-align:center;
      margin-bottom:20px;
      color:#333;
    }

    .input-section{
      display:flex;
      gap:10px;
      margin-bottom:20px;
    }

    input{
      flex:1;
      padding:10px;
      border:1px solid #ccc;
      border-radius:6px;
      font-size:16px;
    }

    button{
      padding:10px 15px;
      border:none;
      border-radius:6px;
      cursor:pointer;
      font-size:15px;
    }

    .add-btn{
      background:#2563eb;
      color:white;
    }

    ul{
      list-style:none;
    }

    li{
      display:flex;
      justify-content:space-between;
      align-items:center;
      background:#f9fafb;
      padding:12px;
      margin-bottom:10px;
      border-radius:8px;
    }

    li.completed span{
      text-decoration:line-through;
      color:gray;
    }

    .actions button{
      margin-left:5px;
    }

    .complete-btn{
      background:#16a34a;
      color:white;
    }

    .delete-btn{
      background:#dc2626;
      color:white;
    }

    .filters{
      display:flex;
      justify-content:center;
      gap:10px;
      margin-top:20px;
    }

    .filter-btn{
      background:#e5e7eb;
    }

    .active{
      background:#2563eb;
      color:white;
    }
  </style>
</head>

<body>

  <div class="container">
    <h1>To-Do List</h1>

    <div class="input-section">
      <input type="text" id="taskInput" placeholder="Enter task">
      <button class="add-btn" id="addTask">Add</button>
    </div>

    <ul id="taskList"></ul>

    <div class="filters">
      <button class="filter-btn active" data-filter="all">All</button>
      <button class="filter-btn" data-filter="active">Active</button>
      <button class="filter-btn" data-filter="completed">Completed</button>
    </div>
  </div>

  <script>
    const taskInput = document.getElementById("taskInput");
    const addTaskBtn = document.getElementById("addTask");
    const taskList = document.getElementById("taskList");
    const filterButtons = document.querySelectorAll(".filter-btn");

    let tasks = JSON.parse(localStorage.getItem("tasks")) || [];
    let currentFilter = "all";

    // Save tasks to localStorage
    function saveTasks() {
      localStorage.setItem("tasks", JSON.stringify(tasks));
    }

    // Render tasks
    function renderTasks() {
      taskList.innerHTML = "";

      let filteredTasks = tasks.filter(task => {
        if (currentFilter === "active") return !task.completed;
        if (currentFilter === "completed") return task.completed;
        return true;
      });

      filteredTasks.forEach((task, index) => {
        const li = document.createElement("li");

        if (task.completed) {
          li.classList.add("completed");
        }

        li.innerHTML = `
          <span>${task.text}</span>
          <div class="actions">
            <button class="complete-btn">
              ${task.completed ? "Undo" : "Done"}
            </button>
            <button class="delete-btn">Delete</button>
          </div>
        `;

        // Complete Task
        li.querySelector(".complete-btn").addEventListener("click", () => {
          tasks[index].completed = !tasks[index].completed;
          saveTasks();
          renderTasks();
        });

        // Delete Task
        li.querySelector(".delete-btn").addEventListener("click", () => {
          tasks.splice(index, 1);
          saveTasks();
          renderTasks();
        });

        taskList.appendChild(li);
      });
    }

    // Add task
    addTaskBtn.addEventListener("click", () => {
      const text = taskInput.value.trim();

      if (text === "") {
        alert("Please enter a task");
        return;
      }

      tasks.push({
        text: text,
        completed: false
      });

      saveTasks();
      renderTasks();

      taskInput.value = "";
    });

    // Filter tasks
    filterButtons.forEach(button => {
      button.addEventListener("click", () => {
        document.querySelector(".active").classList.remove("active");
        button.classList.add("active");

        currentFilter = button.dataset.filter;
        renderTasks();
      });
    });

    // Initial render
    renderTasks();
  </script>

</body>
</html>
