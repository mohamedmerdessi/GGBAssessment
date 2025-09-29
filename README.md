Welcome! This repository contains the starting point for our coding challenge. We're excited to see how you approach this practical, real-world task.

Project Overview
Your task is to build a full-stack, single-page "Feedback Board" application on top of this template. The application will allow users to submit feedback items and track their status through a simple workflow. The core challenge is to design the backend, create the database schema, and build the UI to interact with it.
Core Requirements
Your implementation should satisfy the following user stories:
As a user, I can submit new feedback with the necessary details (e.g., a title and description).
As a user, I can see a list of all submitted feedback items on a single page.
As a user, I can change the status of a feedback item through a simple workflow (e.g., 'Open' ➡️ 'In Progress' ➡️ 'Done') using buttons on the UI.


Bonus Features (Optional)
If you have extra time and want to showcase more of your skills, consider implementing one of the following creative challenges. These are not required, but are a fantastic way to demonstrate deeper product and technical thinking.

1. The Polished Experience (Design & Usability):
Challenge: This is for candidates who love crafting thoughtful interfaces. Go beyond the basic functional requirements and make the application a pleasure to use by focusing on professional polish. You can use a component library like Shadcn/UI, Material UI, or Chakra UI, or demonstrate your skills with a tool like Tailwind CSS.
Your implementation should achieve the following:
Accessibility (a11y): The application must be fully navigable and usable with only the keyboard. All inputs should have proper labels, and interactive elements should have clear focus states.
Responsiveness: The layout must adapt gracefully to a mobile screen size (e.g., 375px width). No content should be cut off or require horizontal scrolling.
Thoughtful User Feedback: The 'Submit' button on the form should be disabled while the API request is in flight to prevent double submissions. Provide clear loading states, for instance, by showing skeleton loaders while the initial feedback list is being fetched.
What this shows: This demonstrates a deep sense of user empathy and frontend craftsmanship. It shows you can build applications that are not just functional but also robust, accessible, and delightful to use for everyone.

2.The People's Choice (Upvoting & Sorting):
Challenge: Add a feature to "upvote" a feedback item. Then, add a control to the UI that allows the list to be sorted by either "Most Recent" or "Most Upvoted."
What this shows: Your ability to evolve a data model, handle more complex state interactions, and implement backend logic for sorting and querying.

3. Instant Gratification (Optimistic UI):
Challenge: When a user changes the status of an item (e.g., clicks "In Progress"), the UI should update immediately, before the API call to the backend has finished. If the API call fails for any reason, the UI should gracefully revert the item to its original state and perhaps show an error.
What this shows: A deep understanding of modern frontend state management and creating a snappy, responsive user experience. This is a very common and important pattern in production applications.


Technical Specifications
Stack
Framework: Next.js ( You are free to use either the Pages or App Router).
Database: Your choice.
ORM / DB Client: You are free to choose and install any ORM or database client you are comfortable with to connect to PostgreSQL.

Data Model
You are responsible for designing the database schema in PostgreSQL. Your schema must be able to store the necessary information for each feedback item, including its content, its current state in the workflow, and when it was created.

API Endpoints
You will need to create the API endpoints to support the application's functionality. We recommend a RESTful approach.
An endpoint to GET all feedback items.
An endpoint to POST a new feedback item.
This should accept the necessary data to create a new item.
An endpoint to PATCH or PUT an existing feedback item.
This will be used specifically for updating the item's status.

Frontend UI & UX
The entire application should exist on a single page (/).
A Note on Visuals: We are primarily focused on functionality and workflow, not design polish. Please do not spend significant time on styling, animations, or pixel-perfect layouts. A clean, simple, and usable interface is all that’s required to demonstrate the features.

Submission Form:
A simple form for creating a new feedback item.
Submitting the form should call your POST endpoint.

Feedback List:
Display all feedback items fetched from your GET endpoint.
Each item card should clearly display its details and current status.
Crucially, each card must have interactive elements (e.g., buttons) to advance its status. Clicking these should call your update endpoint and the UI for that item should react to the change.

A Note on Using AI Assistants
We recognize that AI tools like GitHub Copilot and Claude are part of modern development. You are welcome to use these tools to help you.
However, our goal is to evaluate your problem-solving and design skills. Therefore:
You must be able to explain any code or schema you submit. We will likely ask you to walk through your solution.

Your Task & Submission Workflow
You have cloned this template repository to your local machine.
Do not work in a fork. Please create a new, private repository on your personal GitHub account.
Implement the required features.
Commit your code frequently with clear, descriptive messages. This helps us understand your thought process.
When you are finished, please invite mohamedmerdessi  as a collaborator to your private repository.

Local Setup Instructions
To ensure we can run your project smoothly, please provide clear setup instructions in this README.
Environment Variables: Create a .env.example file in the root of your project listing all necessary environment variables.

# .env.example
DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DATABASE"
Database Setup: Add instructions below on how to prepare the database. For example, if you use a migration tool, specify the exact command to run.
(Your setup instructions here)
Dependencies: Ensure all required dependencies are listed in package.json. We will run npm install (or yarn install).
Running the App: The application should start with the standard npm run dev command.

What We're Looking For
Functionality: Does the application meet all the requirements and user stories?
Database Design: Is the schema you designed logical, efficient, and appropriate for the requirements?
Code Quality: Is the code clean, well-structured, readable, and maintainable?
API Design: Are the API endpoints logical and well-designed?
Frontend State Management: How effectively does the UI react to data changes?
Problem-Solving: How did you approach the requirements and structure your solution?
