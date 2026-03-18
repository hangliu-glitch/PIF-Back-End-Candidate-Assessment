# Backend Software Engineer Take Home Test

In **PayItForward**, we require the back end engineer to be proficient in code development, API design and basic database management, build and deployment. This simple assessment is to access your back end development skills and knowledge. The assignment should take about a day to complete but we allow the submission within a week.  

## Tasks
Your task is to design and implement a **TODO-list server**, where your users can:
* Sign in using any one of: **Gmail, Facebook or GitHub** login. 
* **Add** a TODO item.
* **Delete** a TODO item.
* **List** all TODO items.
* **Mark** a TODO item as completed.

---

## Requirements
* **Language:** Complete the exercise in **Go**. 
* **Scope:** You only need to create the APIs, not the UI / HTML pages.
* **Interface:** The interface should be implemented on **REST API** or **gRPC**.
* **Framework:** You can choose to use any framework you are comfortable with (e.g., Gin, Echo, Go-kit, etc.).
* **Database:** You can use any database or datastore system that can be started standalone.
* **Version Control:** All code shall be committed into a **GitHub** (or equivalent) public repository with proper commit history.
* **Containerization:** The service should be containerized in **Docker** and published to **Docker Hub**.
* **Deployment:** A `docker-compose.yml` file shall be provided to start the docker image along with the database such that we can run it by invoking:
    ```bash
    docker compose up
    ```
* **Verification:** Once the server is running, we should be able to invoke:
    ```bash
    curl -H "Authorization: <any_appropriate_auth_token>" http://host:port/api_path/params1
    ```
    and get an appropriate response object for each of the APIs above (Add/Delete/List/Mark-complete).
* **Testing:** Some unit tests illustrating your testing knowledge is a plus. 

> **Note:** Params can be in RESTful API style, or query parameters. Appropriate authentication tokens can be passed in via Authorization header or as part of the POST body (or input data of any RPC framework that you use, e.g., gRPC).

---

## Evaluation Criteria
* **Code Quality:** Clean, readable, testable, performant, and maintainable.
* **Naming Conventions:** Class and method names should clearly show their intent and responsibility.
* **Scalability:** Your solution should easily accommodate possible future requirement changes.
* **Adaptability:** If you get shortlisted for a second interview, you will be asked to perform minor code changes. You are expected to be able to update and refresh the service.
* **DB Schema Design:** Proper use of indexing and relational design.
* **API Design:** Cleanliness and maturity of the API.

---

## Test Submission 
Provide a URL link to the GitHub project containing the following:

### 1. README
* Instructions for **running** the app.
* Instructions for **testing** the app.
* Instructions for **building** the app.
* **Interface documentation** (API specs).

### 2. Source Code 
* Project must contain all necessary build files/scripts (depending on what build system you choose).
* Scripts and necessary files to build the Docker image of your server.

### 3. Docker Compose File 
* A `docker-compose.yml` for starting the entire service environment.

---

**Please fill up the submission form for review.**

Would you like me to suggest a standard Go project structure for this assignment or help you draft the `docker-compose.yml` template?
