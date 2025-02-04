# SEI7 Team Project3 Capstone

## Project Name:  StadiumSpotter-Back End

### Developers & Collaborators Team

### Samia jamal
### Hussain Zuhair
### Kawthar Mahfoodh
### Rajiah A Rasool

## ERD StadiumSpotter

[ERD for Spotter Web Applicatiion](https://lucid.app/lucidchart/fefbef16-ca85-4e4b-9b4c-e50b83b0488d/edit?viewport_loc=221%2C48%2C1822%2C893%2C0_0&invitationId=inv_7358d525-c7c2-474f-99e6-8355a686d312)

<img src="/images/ERD.png" alt="ERD">

## Wireframes
[Wireframe for Spotter Web Applicatiion](https://drive.google.com/file/d/1ATwKRevKVkXsdx-5TLEJpfEL4yoAR78E/view?usp=sharing)


## Link to StadiumSpotter Web Application: 
[Web Application Link](https://github.com/YouKnow74/StadiumSpotter-BE)

### Our Team:


<img src="/images/ourteam.png" alt="Team Seven">



## Requirements

### General Requirements

- Build a web application from scratch, must be your own work.(completed)
- Use MERN Stack framework to build your application.(completed)
- Deploy on any server so application is live on the web. (completed)
- Create a `README.md` file that explains your app to the world.(completed)
- Include ERD of your project idea.(completed)
- Include wireframes or link to wireframes.(completed)
- Include link to your trello board.()
- Users' board and stories.
- Link to your deployed application.

### Readme Requirements
Don't underestimate the value of a well crafted README.md.
The README.md introduces your project to prospective employers and forms their first impression of your work!
Include the following sections within the README.md:
  ☐ App Title: Contains a description of what the app does and optional background info.
  ☐ Screenshot(s): A screenshot of your app's landing page and any other screenshots of interest.
  ☐ Technologies Used: List of the technologies used. 
  ☐ Planned future enhancements for the application.

### Technical Requirements

☐ A working full-stack, single-page application.
☐ Incorporate the technologies of the MERN-stack:
    *MongoDB/Mongoose
    *Express
    *React
    *Node
☐ Have a well-styled interactive front-end.
☐ Communicates with the Express backend via AJAX.
☐ Implement token-based authentication. Including the ability of a user to sign-up, log in & log out.
☐ Implement authorization by restricting CUD data functionality to authenticated users. Also, navigation should respond to the
   login status of the user.
☐ Have a well-scoped feature-set. Full-CRUD data operations are required for atleast 2 resources other than user.

#### Stretch Technical Goals (optional)
-Consume data from a third-party API.
-Implement additional functionality if the user is an admin.
-Utilize multi-user, real-time communications (beware that this is difficult and time consuming - please seek instructor approval).

### Team Requirements

- Every team member must have commits contributing to the project.
- No single student should do a majority of the commits.

### Necessary Deliverables

- Projects are due on Thursday, 04th of Jan, 2024 at 09.30am!
- You have to fill the [Google Sheet] with you name, github link and deployed link.
- A **15~20 minute presentation** in which you answer the following questions:
  - What is the application about?
  - Is there any information you think might help us understand what you built?
  - What were the team members' contributions to the project?
  - Demo of application.
  - What features did you include?
  - Make sure to explain anything "new" (things that we didn't cover in class).
  - Ensure to program MERN Stack application. Do not forget to include authentication part.
  - What was the most difficult part of the project?
  - What was your favorite part to work on?
  - What would you like to add next?

## About the Web Application (StadiumSpotter-Back End):
The Stadium Reservation Application: is a web-based platform that facilitates the process of conducting reservation. It provides two distinct user roles: Admin, reservation customer, each with specific functionalities tailored to their roles.

### Admin User:
As an Admin user, the user has an access authority to a comprehensive reservation categories created by the user. User can add, edit, view details, and delete reservation. Additionally, has a dedicated section to manage reservation, enabling admin team to add, edit, view details and delete reservation made by the users. Furthermore, they can add new item to sport categories to enhance the diversity of available categories of sport type. Existing Sport types are: indoor and outdoor sports.

### Customer as a User:
Customers are users who can create their own reservation and submit reservation request to reservation team. They have the capability to manage their own reservation, as well as review extra facilities provided along with reservation. By selecting their option of reservation, customers can monitor the progress of reservation and stay informed about payment status or the price of reservation. Customers can also select the date of their reservation, enabling them to control the date of the reservation.


#### User resources 

 - User must have a profile.
 - User must be able upload their profile image.
 - User must be able to edit their profile information.
 - User must be able to change the password.
 
#### User Authentication by JSON Web Tokens(WJT)

Authentication by JSON Web Tokens (JWT) is a method of verifying the identity of a user in a web application or API.
- User must be able to sign up.
- User must be able to sign in.
- User must be able to sign out.
- Token Generation: Upon successful authentication, the server generates a JWT.
- The JWT consists of three parts: a header (for signing the token),
                                a payload (information about user:Id, role, expiry time) and signature.
- The server signs the header and payload with a secret key to create the signature.
- Token takes multiple phases such as: issuance, usage and until reach verification process and access control.


### Technical Aspect of StadiumSpotter-Back End application:

# Server.js

This file contains the server-side code for a web application using Node.js and Express.js. It sets up a server to handle incoming requests and configure various functionalities.

## Dependencies

- Let's go through the JSON file and describe each dependency listed under the "dependencies" key:

1. "bcrypt": "^5.1.1"
   - Description: A library for hashing and salting passwords.
   - Version: "^5.1.1" indicates that it requires a version equal to or greater than 5.1.1.

2. "dotenv": "^16.3.1"
   - Description: A zero-dependency module that loads environment variables from a .env file into process.env.
   - Version: "^16.3.1" indicates that it requires a version equal to or greater than 16.3.1.

3. "ejs": "^3.1.9"
   - Description: A simple templating language that lets you generate HTML markup with plain JavaScript.
   - Version: "^3.1.9" indicates that it requires a version equal to or greater than 3.1.9.

4. "express": "^4.18.2"
   - Description: A fast, unopinionated, minimalist web framework for Node.js.
   - Version: "^4.18.2" indicates that it requires a version equal to or greater than 4.18.2.

5. "jsonwebtoken": "^9.0.2"
   - Description: An implementation of JSON Web Tokens (JWT) for generating and verifying tokens.
   - Version: "^9.0.2" indicates that it requires a version equal to or greater than 9.0.2.

6. "mongoose": "^8.0.3"
   - Description: An object modeling tool for MongoDB that provides a straightforward, schema-based solution to model application data.
   - Version: "^8.0.3" indicates that it requires a version equal to or greater than 8.0.3.

These dependencies are essential for the back-end functionality of the StadiumSpotter application. They provide functionalities such as password hashing, environment variable management, HTML templating, web framework capabilities, JWT handling, and MongoDB data modeling. 

## Installation and Setup

1. Clone the project repository.
2. Navigate to the project directory.
3. Install the required dependencies by running the command: `npm install`.
4. Create a `.env` file in the root directory and configure the necessary environment variables. Refer to the `.env.example` file for the required variables.
5. Start the server by running the command: `node server.js`.

## Configuration

- The server listens on the port specified in the `PORT` environment variable.
- Static files, such as CSS, JS, audio, video, and image files, are served from the "public" directory.
- The database configuration is defined in the "db" module located in the "config" directory.

## Routes

The following routes are available:

- `/facility`: Handles requests related to facilities.
- `/reservation`: Handles requests related to reservations.
- `/stadium`: Handles requests related to stadiums.



##control.js file exports functions that handle reservation-related operations such as creating a new reservation, retrieving a list of reservations, deleting a reservation, retrieving a reservation for editing, and updating a reservation. These functions interact with the Reservation model and perform database operations based on the received HTTP requests and send appropriate responses.

##used HTTP methods along with their typical usage:

GET: retrieves a resource or a list of resources (retrieving data, fetching a web page and retrieving a list of items). It should not have any side effects on the server.

POST: submits data to be processed to a specified resource (for example, submitting a form, sending data to be processed). It can create new resources or perform other actions that have side effects on the server.

PUT: updates a resource at a specified URL with the new representation provided in the request (updating an existing resource with a complete replacement representation). It replaces the entire resource with the new data.

These HTTP methods are used in combination with URLs (endpoints) to perform various operations on web resources. The choice of method depends on the desired action and the semantics of the operation you decide to perform on the server.

## Usage

1. Make sure the server is running.
2. Send HTTP requests to the appropriate routes using tools like cURL or a web browser.
3. Check the console log for the message indicating that the server is running on the specified port.










## Useful Resources

- **[Git Team Workflow](https://trello.com/invite/stadiumspotter/ATTIb079db0c886353646c04bf9c6612f24e0062057C)**
- **[MongooseJS documentation](https://mongoosejs.com/docs/index.html)**
-**[Mongoose web application databas link:mongodb+srv://Hussain:2qWcV0dri9YcdbAg@cluster0.j0qrk0d.mongodb.net/StadiumSpotter?       retryWrites=true&w=majority]
     PORT=3011
     SECRET=HelloTeamMembers85452222


