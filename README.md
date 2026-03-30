query GetAllTasks {
  tasks {
    id
    title
    description
    completed
  }
}


mutation AddNewTask {
  addTask(title: "Faire le TP5", description: "Terminer la configuration de GraphQL avec Express", completed: false) {
    id
    title
    description
    completed
  }
}


mutation CompleteTask {
  completeTask(id: "1") {
    id
    title
    description
    completed
  }
}