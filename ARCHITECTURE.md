<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>School Management System Diagram</title>
</head>
<body>

    <h2>School Management System Class Diagram</h2>

    <pre class="mermaid">
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

            SchoolManagementSystem --> Student : manages
            SchoolManagementSystem --> Teacher : manages
            SchoolManagementSystem --> Admin : manages
    </pre>

    <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
        mermaid.initialize({ startOnLoad: true });
    </script>

</body>
</html>
