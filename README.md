
# -- Advanced Grading Console

*Submitted as part of the CodeForge V1 Challenge at BITS Pilani.*

## Overview

The Advanced Grading Console is a browser-based tool that helps
instructors upload student marks, review course data, adjust grade
boundaries, analyze class performance, and download grading reports.

## Bug Fixes (check bug log report)

-   Fixed course selection issues when uploading a new Excel workbook by
    refreshing the available course options.
-   Fixed grading timer behavior so it starts correctly and resets when
    a new file or course is selected.
-   Added checks for missing fields, invalid marks, malformed files, and
    duplicate student-course records.
-   Supports uploading one Excel workbook at a time, and extracts unique
    number of courses from the file for the drop down
-   More bugs were fixed that can be found in the report.

## New Features

-   Added an Excel preview and validation summary so instructors can
    review data before grading.
-   Added marks distribution and grade distribution charts, where an
    instructor can see, how many students fall in a grade range
-   Added a searchable student table with BITS ID search, grade filters,
    and top-five and bottom-five views.
-   Improved editable grade boundaries with validation.

## Data Validation and Cleaning Logic

-   Added file validation to reject uploads with fewer or more than 3 columns.
-   Added warnings for missing values and marks outside the valid range (0–100), highlighting affected rows and excluding them from import if the user proceeds.
-   Added automatic rounding of decimal marks to the nearest whole number, with a notification informing the user that the data was tidied up.
-   Added validation checks to accept files that meet all criteria without warnings or modifications.
-   You can use grading_test_data to test the tool on all scenarios. It contains a file for reach data validation and cleaning scenario to test how tool responds.

## UI Experience

-   Redesigned the interface with a clearer upload process and a more
    organized grading dashboard.
-   Improved upload feedback, workbook preview, and validation messages.
-   Used consistent typography, spacing, subtle borders, and restrained
    purple accents for a cleaner look inspired from BITS Pilani Logo
-   Improved responsiveness for smaller screens and added clearer
    interaction and focus states.

## Basic Usage

1.  Enter the instructor name.
2.  Upload a single `.xlsx` workbook containing student BITS IDs, course
    names, and total marks.
3.  Review the workbook preview and validation summary.
4.  Continue to the grading dashboard and select a course.
5.  Review the charts and student table, and adjust grade boundaries if
    needed.
6.  Download the grading report as a CSV file.
>>>>>>> f9627c7 (updated ui and features)
