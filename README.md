query GetAllTasks {
  tasks {
    id
    title
    description
    completed
  }
}

![GetAllTasks Query](..\assets\image1.png)

mutation AddNewTask {
  addTask(title: "Faire le TP5", description: "Terminer la configuration de GraphQL avec Express", completed: false) {
    id
    title
    description
    completed
  }
}

![AddNewTask Mutation](..\assets\image2.png)

mutation CompleteTask {
  completeTask(id: "1") {
    id
    title
    description
    completed
  }
}

![CompleteTask Mutation](..\assets\image3.png)
