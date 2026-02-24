```mermaid
classDiagram
    class SchoolManagementSystem {
        +Student()
        +Teacher()
        +Admin()
    }
    class Student {
        +register()
        +viewGrades()
    }
    class Teacher {
        +assignGrades()
        +manageClasses()
    }
    class Admin {
        +manageUsers()
        +generateReports()
    }
    SchoolManagementSystem --> Student : interacts
    SchoolManagementSystem --> Teacher : interacts
    SchoolManagementSystem --> Admin : interacts
```