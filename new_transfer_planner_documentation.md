# Transfer Planner Documentation

## Project Description

The goal of this application is to help students understand which completed courses can be transferred from one academic program to another.

---

## Features

- Displays all courses
- Shows whether each course is passed or not
- Allows selection of a target program
- Generates an equivalency table
- Excludes non-passed courses from transfer calculations

---

## Program Information

Current Program:
- Computer Science

Available Target Programs:
1. Computer Engineering
2. Civil Engineering
3. Electrical and Electronics Engineering

---

## Equivalency Algorithm

The application uses a simple keyword-based equivalency system.

Each course from the current program is compared with predefined equivalent courses from the selected target program.

### Rules Used

- Only courses marked as "Yes" are considered transferable.
- Courses marked as "No" are ignored.
- If no matching course exists, the application displays `N/A`.

### Example

| Current Course | Equivalent Course |
|---|---|
| Introduction to Programming | Embedded Programming |
| Calculus I | Engineering Mathematics |
| Database Systems | Information Systems |

### Sample Logic

```javascript
if(course.includes("Programming")){
    equivalent = "Embedded Programming";
}
```

---

# Future Improvements

## Automatic Syllabus Comparison Using AI

A future version of this project could use Artificial Intelligence to automatically compare academic program syllabi.

### Proposed Algorithm

1. Load syllabus documents from universities
2. Extract:
   - Topics
   - Learning outcomes
   - Course descriptions
3. Use Natural Language Processing (NLP) to compare similarity between courses
4. Generate similarity scores
5. Automatically suggest equivalent courses

### Example

If two courses contain:
- similar programming topics
- same learning objectives
- matching practical work

then the system could automatically mark them as equivalent.

---

## Benefits of AI-Based Comparison

- Faster transfer evaluation
- Reduced manual work
- More accurate equivalency detection
- Easier process for students and universities

---

## Conclusion

This project demonstrates a simple transfer planning system and shows how AI could improve academic course equivalency in the future.
