# ✨Vibe Planner✨
An AI-powered task management system for [Cursor](https://cursor.sh/) that seamlessly integrates into both new and existing projects.

**Why a new planning system?** Most planning frameworks I've tried start with a new project and integrate poorly into existing solutions. When generating PRD, they poorly reflect the existing codebase and visual consistency across the entire application.

**Vibe Planner is feature-centric**, with every new assignment starting as a new feature described through an **FRD (Feature Requirements Document)**.

## Workflow ➡️➡️➡️
Here's the step-by-step process using the `.mdc` files in this repository:

### 1️⃣ Create a Froduct Requirement Document (FRD)

In Cursor's Agent chat, initiate FRD creation:

    
    Use @create-frd.mdc
    Here's the feature I want to build: [Describe your feature in detail]
    Reference these files to help you: [Optional: @file1.py @file2.ts]
    

### 2️⃣ Generate Your Task List from the FRD

In Cursor's Agent chat, use the FRD to create tasks:

    
    Now take @O1-My-Feature.md and create tasks using @create-tasks.mdc
    

### 3️⃣ Examine Your Task List

You'll now have a well-structured task list, often with tasks and sub-tasks. Take time to review the generated task list carefully and make any necessary adjustments or refinements to ensure it aligns with your specific requirements and project goals.

### 4️⃣ Instruct the AI to Work Through Tasks (and Mark Completion)

In Cursor's Agent chat, tell the AI to start with the first task (e.g., `1.1`):

    
    Please start on task 1.1 and use @process-task-list.mdc
    

### 5️⃣ Review, Approve, and Progress ✅

As the AI completes each task, you review the changes.
*   If the changes are good, simply reply with "yes" (or a similar affirmative) to instruct the AI to mark the task complete and move to the next one.
*   If changes are needed, provide feedback to the AI to correct the current task before moving on.

You'll see a satisfying list of completed items grow, providing a clear visual of your feature coming to life!

## ✨ To Do
1. Create constraints and guidelines from codebase
2. Create visual guidelines to ensure visual consistency across the entire application
3. Log the time spent on tasks
