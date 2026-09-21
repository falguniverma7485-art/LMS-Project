# LMS Assignment & Progress Module

## Overview

This project contains the frontend module for Assignment Management, Student Progress Tracking, and Teacher-side Assignment Evaluation in a Learning Management System (LMS).

The module is built using only HTML and CSS. It does not use JavaScript, a backend, a database, or real authentication.

## Module Structure

```text
LMS_Assignment_Connected/
│
├── HTML/
│   ├── assignment.html
│   ├── assignment-details.html
│   ├── submission.html
│   ├── progress.html
│   ├── teacher-login.html
│   ├── teacher-dashboard.html
│   ├── teacher-assignments.html
│   ├── student-submissions.html
│   └── evaluation.html
│
├── CSS/
│   └── style.css
│
└── README.txt
```

## Student-side Pages

### assignment.html
Assignment dashboard containing:
- Total assignments
- Submitted assignments
- Pending assignments
- Overdue assignments
- Assignment list
- Course and instructor details
- Due dates
- Marks
- Links to assignment details

### assignment-details.html
Displays assignment-specific details for:
- HTML Assignment
- CSS Flexbox Assignment

Each assignment contains:
- Course
- Instructor
- Due date
- Maximum marks
- Description
- Instructions
- Submission status
- Evaluation status
- Teacher feedback

The same page uses URL fragments to display the selected assignment:

```text
assignment-details.html#html
assignment-details.html#css
```

### submission.html
Student assignment submission page containing:
- Student name
- Assignment name
- File upload
- Comments
- Due date
- Submit and cancel controls

### progress.html
Student progress page containing:
- Overall progress
- Completed assignments
- Pending assignments
- Average marks
- Course-wise progress bars

## Teacher-side Pages

### teacher-login.html
Frontend teacher login form with:
- Teacher email
- Password
- Login button

The login is a frontend-only form and does not perform real authentication.

### teacher-dashboard.html
Teacher dashboard containing:
- Total assignments
- Total students
- Pending evaluations
- Evaluated submissions
- Assignment management access

### teacher-assignments.html
Teacher assignment list containing:
- Assignment name
- Course
- Due date
- Number of submissions
- Pending evaluations
- Maximum marks
- Link to student submissions

### student-submissions.html
Displays submitted student assignments with:
- Student name
- Submission date
- Evaluation status
- Marks
- Evaluation action

### evaluation.html
Teacher evaluation page containing:
- Student name
- Submitted file
- Marks field
- Feedback field
- Submit evaluation control
- Back to submissions link

## Main Flows

### Student Flow

```text
Assignments
    ↓
Assignment Details
    ↓
Submission
    ↓
Progress
```

### Teacher Flow

```text
Teacher Login
    ↓
Teacher Dashboard
    ↓
Teacher Assignments
    ↓
Student Submissions
    ↓
Evaluation
```

## Technology

- HTML5
- CSS3

No JavaScript is used in this module.

## Styling

The module uses a shared stylesheet:

```text
CSS/style.css
```

The design follows a common LMS visual style with:
- Poppins font
- Light lavender background
- Purple and indigo primary colors
- White rounded cards
- Soft shadows
- Consistent buttons and form fields
- Responsive layout
- Rounded corners

## Important Limitation

This is a frontend-only implementation.

The following are static UI elements and do not persist data:

- Teacher login
- Assignment submissions
- Marks
- Teacher feedback
- Student progress
- Evaluation results

Backend, database, and real authentication can be integrated in a later phase.

## Running the Project

Open any HTML file from the `HTML` folder in a browser or use VS Code Live Server.

For the best navigation experience, start with:

```text
HTML/assignment.html
```

Teacher-side testing can start with:

```text
HTML/teacher-login.html
```
