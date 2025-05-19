# 🗓️ Dynamic Attendance Skip Planner

A client-side web application designed to help students strategically plan and track their class attendance. Calculate your initial "skip budget" for a semester (based on a 12-week period and an 80% minimum attendance target), and then dynamically update your remaining skippable hours as you use them. Get insights into your current attendance status and optimal ways to use your remaining skip allowance.

link for access: (https://wongkw0731.github.io/Attandace-Calculator/)

<!-- Optional: Add a screenshot or GIF here -->
![image](https://github.com/user-attachments/assets/88e51475-d270-45c4-9df3-ee3364a57017)![image](https://github.com/user-attachments/assets/415ae333-3a93-44e0-9197-7a676f1f9f38)![image](https://github.com/user-attachments/assets/50f1df3a-10a1-4514-93a5-7e38e4a0e6a6)![image](https://github.com/user-attachments/assets/a1748de3-ca32-4df7-ba95-72e0827a3a16)![image](https://github.com/user-attachments/assets/0d908286-cf9c-482b-8b6d-6b2c4041978a)






## ✨ Core Features

*   **📚 Flexible Class Setup:**
    *   Define multiple class types (e.g., Lecture, Lab, Tutorial).
    *   For each class type, specify:
        *   A custom name.
        *   Hours per session (e.g., 2 hours for a lecture).
        *   Number of sessions per week.
    *   Easily add or remove class types.

*   **🧮 Initial Skip Allowance Calculation (Phase 1):**
    *   Calculates total scheduled hours for a 12-week semester based on your class setup.
    *   Determines your **total initial skippable hours budget** (20% of total scheduled hours, aiming for 80% attendance).
    *   Displays:
        *   Total Scheduled Hours.
        *   Minimum Required Attendance Hours.
        *   Your Total Skippable Hours Budget.
    *   Shows the maximum number of individual sessions of *each class type* you could skip if you used your entire budget on that one type.
    *   **Optimal Skipping Combinations:** Suggests various combinations of different class types you could skip to maximally utilize your initial budget.

*   **🔄 Track Skips & Update Allowance (Phase 2):**
    *   After initial calculation, input the number of sessions you've *already skipped* for each class type.
    *   **Recalculates:**
        *   Your **current remaining skippable hours budget**.
        *   Your **current attendance percentage**.
        *   Total hours skipped so far.
        *   Effective hours attended.
    *   **Current Attendance Status:** Clearly indicates if you are "Currently Safe" or on the "Barrier List Warning" (below 80% attendance) with a visual badge.
    *   **Optimal Remaining Skipping Combinations:** Shows how to best use your *remaining* budget.

*   **📊 Insightful Results & Visualizations:**
    *   Clear presentation of semester overview, skippable hours, and attendance status.
    *   Tables for maximum individual session skips.
    *   Lists for optimal multi-class skipping combinations.
    *   Status badges (Safe/Danger) for quick understanding of your current attendance.

*   **⚙️ User-Friendly Interface:**
    *   Clean, modern design with intuitive "stepper" inputs for numerical values.
    *   Responsive layout for different screen sizes.
    *   Clear separation between initial setup and ongoing tracking.
    *   Calculations are performed client-side, providing instant feedback.

## 🚀 How to Use

1.  **Open `index.html`** in your web browser.

2.  **Phase 1: Initial Setup & Calculation**
    *   Click "➕ Add Class Type" to define your classes.
    *   For each class:
        *   Enter a **Class Type Name** (e.g., "Calculus Lecture").
        *   Adjust **Hours per Class Session** using the stepper.
        *   Adjust **Number of Sessions per Week** using the stepper.
    *   Once all class types are defined, click "🧮 Calculate Initial Allowance".
    *   Review your "Semester Attendance Overview", "Total Initial Skippable Hours Budget", "Max Sessions to Skip" (individually), and "Optimal Initial Skipping Combinations".

3.  **Phase 2: Track Your Skips & Update Allowance**
    *   The "Track Your Skips" section will now be active.
    *   For each class type listed, use the stepper to input the **number of sessions you have already skipped**.
    *   Click "🔄 Recalculate Remaining Skips".
    *   Review your:
        *   "Current Attendance Status" (Safe or Barrier List).
        *   "Current Remaining Skippable Budget".
        *   "Optimal Remaining Skipping Combinations" based on your updated budget.

4.  **Repeat Phase 2** throughout the semester as you skip more classes to stay updated. If your class schedule changes, you can modify the initial setup and recalculate from scratch.

## 💻 Technical Highlights

*   **Pure Client-Side Logic:** All calculations and interactions are handled by JavaScript directly in the browser. No backend or internet connection is required after loading the page.
*   **Dynamic DOM Manipulation:** JavaScript is used to dynamically add/remove class input fields and update result sections without page reloads.
*   **Combination Generation:** Implements logic to find and display various combinations of class skips that fit within the allowed budget.
*   **CSS Styling:** Modern CSS with variables for theming (`Poppins` and `Inter` fonts).
*   **No Data Persistence:** This version of the planner is session-based. Data is not saved locally in the browser (e.g., via `localStorage`). You'll need to re-enter your class setup if you close and reopen the page.

## 💡 Potential Future Enhancements

*   [ ] Local storage to save class setups and skipped counts between sessions.
*   [ ] Option to define a custom total number of semester weeks.
*   [ ] Option to set a custom minimum attendance percentage.
*   [ ] More advanced combination filtering or sorting.
*   [ ] Visual calendar integration or planning view.
