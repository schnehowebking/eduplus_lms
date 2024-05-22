# Learning Management System with Django

A comprehensive School Management System (LMS) built with the Django web framework. Whether you're developing an LMS for an educational institution or looking to enhance your skills and portfolio, this project is a perfect starting point.

Let's collaborate and enhance this project together!

## Current Features

- **Dashboard:** Displays school demographics and analytics; accessible only to admins.
- **News and Events:** Available to all users.
- **Student Management:** Admins can add, update, and delete student records.
- **Lecturer Management:** Admins can add, update, and delete lecturer records.
- **Course Enrollment:** Students can add or drop courses.
- **Score Submission:** Lecturers can submit scores for attendance, midterm exams, final exams, and assignments.
- **Automatic Calculations:** The system calculates total, average, points, and grades for students.
- **Grade Comments:** Provides comments such as "pass," "fail," or "pass with a warning."
- **Assessment and Grade Pages:** Students can view their assessment results and grades.
- **Academic Management:** Manages sessions/years and semesters, grouping assessments and grades accordingly.
- **Content Upload:** Supports video and documentation uploads for each course.
- **PDF Generation:** Generates PDFs for student registration slips and grade results.
- **Access Control:** Implements page access restrictions.
- **Quiz Management:**
  - Stores quiz results under each user.
  - Randomizes question order.
  - Allows viewing of previous quiz scores on the category page.
  - Shows correct answers after each question or all at once at the end.
  - Supports resuming incomplete quizzes for logged-in users.
  - Limits quizzes to one attempt per user.
  - Categorizes questions and monitors success rates by category.
  - Provides explanations for question results.
  - Sets pass marks.
  - Supports multiple choice, true/false, and essay question types.
  - Displays custom messages for pass or fail outcomes.
  - Adds custom permissions (view_sittings) to view quiz results from users.
  - Includes a marking page for completed quizzes, filterable by quiz or user.

## Contributing

We welcome contributions! To get started, check out the `TODO.md` file for tasks.

## Requirements

Ensure you have the following installed:

- [Python 3.8+](https://www.python.org/downloads/)
- [PostgreSQL](https://www.postgresql.org/download/)
- [Redis](https://redis.io/docs/latest/operate/oss_and_stack/install/install-redis/)

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/schnehowebking/eduplus_lms.git
    ```

2. **Create and activate a Python virtual environment:**

    ```bash
    pip install -r requirements.txt
    ```

3. **Create a `.env` file in the root directory and add the following variables:**

    ```bash
    # Database configuration
    DB_NAME=[YOUR_DB_NAME]
    DB_USER=[YOUR_DB_USER]
    DB_PASSWORD=[YOUR_DB_PASSWORD]
    DB_HOST=localhost
    DB_PORT=[YOUR_POSTGRES_PORT (default is 5432)]

    # Email configuration
    EMAIL_FROM_ADDRESS="Django LMS <youremail@example.com>"
    EMAIL_HOST_USER=[YOUR_EMAIL]
    EMAIL_HOST_PASSWORD=[YOUR_EMAIL_PASSWORD]

    # Other
    DEBUG=True
    SECRET_KEY=[YOUR_SECRET_KEY]
    ```

4. **Apply migrations:**

    ```bash
    python manage.py migrate
    ```

5. **Create a superuser:**

    ```bash
    python manage.py createsuperuser
    ```

6. **Start the development server:**

    ```bash
    python manage.py runserver
    ```

7. **Ensure your Redis server is running:**

    ```bash
    redis-server
    ```

8. **Start the Celery worker:**

    ```bash
    celery -A config.celery worker -l INFO
    ```

9. **Access the application at:** [http://127.0.0.1:8000](http://127.0.0.1:8000)

## References

- Quiz functionalities adapted from: [django_quiz](https://github.com/tomwalker/django_quiz)

## Connect with Me

<div>
<a href="https://www.linkedin.com/in/mdhasibunnabischneho" target="_blank">
<img src=https://img.shields.io/badge/linkedin-%231E77B5.svg?&style=for-the-badge&logo=linkedin&logoColor=white alt=linkedin />
</a>
<a href="https://github.com/schnehowebking" target="_blank">
<img src=https://img.shields.io/badge/github-%2324292e.svg?&style=for-the-badge&logo=github&logoColor=white alt=github />
</a>
<a href="https://stackoverflow.com/users/14780695/schnehowebking" target="_blank">
<img src=https://img.shields.io/badge/stackoverflow-%23F28032.svg?&style=for-the-badge&logo=stackoverflow&logoColor=white alt=stackoverflow />
</a>
<a href="https://www.facebook.com/hunschneho/" target="_blank">
<img src=https://img.shields.io/badge/facebook-%232E87FB.svg?&style=for-the-badge&logo=facebook&logoColor=white alt=facebook />
</a>
</div>

## Support

<a href="https://www.buymeacoffee.com/schnehowebking">
<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="schnehowebking" />
</a>

#### Show your support by starring this project!
