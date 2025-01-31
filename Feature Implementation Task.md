# Feature Implementation Task: Print History Table

## Task Overview
You are responsible for implementing a **Material-UI Table** in the existing `PrintHistory.tsx` file. This table should fetch data from the backend API and display the print history in a structured format.

## Requirements
- Use **Material-UI Table** components.
- Fetch print job data from the API and store it in state.
- Display the following columns:
  - **Print Job** (file name)
  - **Lab**
  - **Status**
  - **Material**
- Handle loading states and API errors properly.

## Steps to Complete

### Step 1: Set Up Development Environment and Branch
- Ensure your development environment is properly set up.
- Create a new feature branch before starting work:
  ```sh
  git checkout -b feature/print-history-table
  ```

### Step 2: Verify API Response
Before integrating the API into the frontend, confirm that the backend is returning the expected data.

- API Endpoint: `GET /print-jobs/`
- Test the API using the following cURL command:
  ```sh
  curl -X GET http://localhost:8000/print-jobs/ \
       -H "Content-Type: application/json"
  ```
- Ensure the response matches the expected JSON format:
  ```json
  [
    {
      "id": 1,
      "file": "prototype_arm.stl",
      "lab": "3D Print Hub",
      "material": "PLA",
      "status": "completed",
      "created_at": "2024-01-30T12:34:56Z"
    }
  ]
  ```

### Step 3: Fetch Data in `PrintHistory.tsx`
- Use `useEffect` to fetch the API data.
- Store the response in `useState`.
- Implement error handling for failed requests.

### Step 4: Display Data in a Material-UI Table
- Implement a `Table` with appropriate `TableCell` values.
- Ensure proper alignment and readability.

### Step 5: Test and Validate
- Start the backend and ensure `/print-jobs/` is accessible.
- Verify the table correctly displays fetched data.
- Check pagination, error handling, and UI responsiveness.

### Step 6: Create a Pull Request
- Once the feature is implemented, push the branch to the repository:
  ```sh
  git add .
  git commit -m "Implement Print History Table"
  git push origin feature/print-history-table
  ```
- Open a pull request (PR) for review.
- Address any feedback before merging into the main branch.

## Deliverables
- A working `PrintHistory.tsx` page with a **Material-UI Table** displaying print jobs.
- Fully functional API integration with pagination.
- Proper error handling and loading states.
- A completed pull request ready for review.

## Notes
- Follow best practices for API calls and state management.
- Ensure consistent styling with the existing UI components.
- If authentication is required in the future, implement it accordingly.

---
This document outlines the **expected implementation** for the Print History Table.

