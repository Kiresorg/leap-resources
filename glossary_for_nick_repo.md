# Leap Project Glossary

*Terms used in the Leap Project README, with plain-English definitions.*

**Acceptance criteria:** The specific, testable conditions a piece of work must meet before the customer accepts it as finished.

**Agile:** A way of running software projects in short, repeated cycles, delivering working pieces often and adjusting the plan based on feedback.

**Analysis and design pack:** The set of documents and diagrams a team produces to describe what will be built and how its parts fit together.

**Analytics:** Examining data to find patterns, totals and trends that help people make decisions.

**Angular:** A tool from Google for building the screens of a web application (the part users see and click in a web browser).

**API (Application Programming Interface):** A defined way for one piece of software to request data or actions from another, such as a trading screen asking a server (a computer that provides a service to others) to place an order.

**API contract:** The written agreement describing exactly which requests an API accepts and which responses it returns, so separate teams can build each side independently.

**Architecture (software architecture):** The overall structure of a system: its major parts, what each one is responsible for, and how they connect.

**Artefact:** Any document, diagram, model or file produced during a project, such as a requirements document or a test plan.

**Auth service:** The part of the system that confirms who a user is (authentication) and what they are allowed to do (authorization).

**AWS (Amazon Web Services):** Amazon's cloud service, which rents out computers, storage and other computing resources over the internet.

**Backlog:** The prioritized list of all the work a team intends to do on its product, usually written as user stories.

**Board (task board):** A shared display, usually in a tool such as JIRA, that shows each piece of work as a card moving through columns such as To Do, In Progress and Done.

**BR-18 extension:** An optional extra feature that each team proposes and builds itself, described in business requirement number 18 of the project specification.

**BRD (Business Requirements Document):** A document that describes what a business needs a system to do and why, written in business language rather than technical terms.

**Business analysis:** The work of understanding what a business needs, defining the problem clearly, and describing what a solution must do.

**Business requirements spec (BRS):** The document handed out at kickoff that describes what the trading platform must do and the standard it must meet, without saying how to build it (spec is short for specification).

**Cadence:** The regular rhythm at which recurring activities happen, such as a weekly review.

**Candidate architecture:** A first, proposed design for a system's structure, put forward for discussion before it is agreed.

**Capstone:** The final project of a training program, in which participants apply everything they have learned.

**CI/CD (Continuous Integration and Continuous Delivery):** An automated process that combines each developer's code changes, tests them, and prepares them for release, many times a day.

**Cloud:** Computing power, storage and software rented over the internet from a provider such as Amazon, instead of run on an organization's own machines.

**Cloud deployment:** Installing and running a finished application on cloud computers so people can use it over the internet.

**Confluence:** A shared team website, made by the company Atlassian, used to write, organize and publish project documents.

**Customer:** In this project, an instructor who plays the business that commissioned the trading platform, whom the team must consult and satisfy.

**Customer engagement:** Meeting and communicating with the customer to understand their needs and agree on what to build.

**Data dictionary:** A reference document listing every data field in a system, with its meaning, format and allowed values.

**Data model:** A description of what information a system stores and how the pieces relate, such as each order belonging to one account.

**Data systems:** The databases (organized stores of data) and related tools a business uses to store, organize and retrieve its information.

**Defect log:** A running record of the problems (defects, often called bugs) found during testing, with the details and current status of each.

**Deployment:** Installing a version of the software where people can use it.

**Deployment automation:** Using scripts and tools to install software the same way every time, with no manual steps.

**Design thinking:** A problem-solving approach that starts by understanding the people who will use a product, then tests ideas with them quickly and repeatedly.

**DevSecOps:** Building security checks into every stage of creating and running software, rather than adding them at the end.

**Docker:** A tool that packages an application together with everything it needs to run into a single unit (a container), so it runs the same way on any computer.

**Domain:** The area of business a system serves, such as trading, together with that area's rules and vocabulary.

**Domain engine:** The core code that carries out a business's rules, such as checking whether a client has enough cash to place an order.

**Domain model:** A diagram or description of the main things a business deals with (such as accounts, orders and instruments) and how they relate.

**EDA (Exploratory Data Analysis):** Looking through a set of data with summaries and charts to understand what it contains before drawing conclusions.

**Elicitation:** The analyst's work of drawing out requirements from stakeholders through interviews, workshops and observation.

**ETL (Extract, Transform, Load):** A process that pulls data out of one system, cleans or reshapes it, and loads it into another, often a database used for reporting.

**Event backbone:** A central messaging system that carries notices of things that have happened (events), such as "order filled," from the parts of a system that produce them to the parts that need to react.

**Event-driven architecture:** A system design in which the parts communicate by publishing and reacting to events, rather than by calling each other directly.

**GenAI (Generative AI):** Artificial intelligence that creates new text, code or images in response to instructions, such as GitHub Copilot.

**Git:** A tool that records every change to a project's files, so a team can work on them together, see who changed what, and return to earlier versions.

**Go/no-go recommendation:** The analysts' evidence-based advice on whether a system is ready to release (go) or not (no-go).

**Handoff:** The point where one person or group passes finished work to another, such as analysts giving engineers a screen specification to build from.

**HTML/CSS:** The two basic languages of web pages: HTML defines a page's content and structure, and CSS defines how it looks.

**IaC (Infrastructure as Code):** Setting up servers and networks by writing configuration files that a tool carries out, instead of configuring each one by hand.

**IAM (Identity and Access Management):** The rules and tools that control who can sign in to a system and what each person is allowed to do.

**Java:** A widely used programming language for building large business applications.

**JIRA:** A work-tracking tool, made by the company Atlassian, in which teams record and manage tasks, user stories and defects.

**JS (JavaScript):** The programming language that runs inside web browsers to make pages interactive.

**JWT (JSON Web Token):** A small, digitally signed piece of data that proves who a user is and is sent with each request after they sign in (JSON is a common text format for data).

**Kafka:** Software that moves large streams of messages (events) between systems reliably and in the order they occurred.

**Kickoff:** The first day of the project, when teams receive the business requirements spec and present an initial plan.

**MyBatis:** A Java tool that connects program code to a database by linking the code to the database queries (requests for data) it runs.

**NestJS:** A framework (a ready-made structure that programmers fill in) for building server applications with Node.js and TypeScript.

**Node (Node.js):** Software that runs JavaScript on a server rather than inside a web browser.

**NoSQL:** A family of databases that store data in forms other than the rows and columns of traditional tables.

**OOAD (Object-Oriented Analysis and Design):** Analyzing and designing a system as a set of objects (things that hold data and behavior, such as an Order) that work together.

**OpenAPI:** A standard format for writing an API contract, which tools can read to produce documentation and test pages automatically.

**OWASP (Open Worldwide Application Security Project):** A nonprofit organization best known for its list of the ten most critical security risks in web applications.

**pandas:** A Python library (a collection of ready-made code) for loading, cleaning and analyzing tables of data.

**Permission matrix (role and permission matrix):** A table showing which types of user can see or do which things in a system.

**Pipeline:** An automated series of steps that builds, tests and releases software each time its code changes.

**Postgres (PostgreSQL):** A free, widely used database that stores data in linked tables and is queried with SQL.

**Postman:** A tool for sending requests to an API and viewing its responses, used to test or explore an API without writing code.

**Process model:** A diagram showing the steps of a business activity, who does each step, and in what order.

**Product thinking:** Deciding what to build by focusing on the problem it solves for users and the value it delivers, rather than on features for their own sake.

**Production code:** The code of the real system that will be released to users, as opposed to tests or experiments.

**Python:** A programming language popular for data analysis and automation because it is easy to read.

**README:** The introductory file in a code repository (a project's shared folder of files, kept with Git) that explains what the project is and how to use it.

**Refactoring:** Restructuring existing code to make it clearer or easier to maintain, without changing what it does.

**Refined backlog:** A backlog whose items have been clarified, split into small pieces, estimated and prioritized so they are ready to work on.

**REST (Representational State Transfer):** A common style of web API in which programs request data or actions using web addresses and standard commands such as GET and POST.

**Risk list:** A list of things that could go wrong on a project, with how likely and serious each one is and what the team will do about it.

**Schema (database schema):** The definition of a database's structure: its tables, the columns in each table, and how the tables link to each other.

**Screen specification:** A document describing each screen of an application: what it shows, what users can do on it, and how it behaves in different situations.

**Secure Code Warrior:** An online training platform that teaches developers to write secure code through hands-on coding challenges.

**Service:** A separately running piece of software that handles one area of a system, such as placing trades or signing users in, and that other parts use through its API.

**Showcase:** A presentation in which a team demonstrates its finished work to an audience.

**Sign off:** To formally approve a piece of work as complete and acceptable.

**SOLID:** Five principles for designing object-oriented code (code organized around objects) so that it is easier to change and extend.

**Sprint:** A short, fixed period of work, often one or two weeks, at the end of which the team delivers and reviews a working piece of the product.

**Spring Boot:** A popular Java framework (a ready-made structure that programmers fill in) for quickly building services and APIs.

**SQL (Structured Query Language):** The standard language for reading and changing data in relational databases (databases that store data in linked tables).

**Stakeholder:** Anyone with an interest in or influence over a project, such as the sponsor who funds it, the people who will use it, or the compliance team.

**Stakeholder demo:** A live demonstration of work in progress to stakeholders, tailored to what each of them cares about.

**Stakeholder panel:** A group of people playing the project's business stakeholders, who hear a team's presentation and question it.

**Stand-up:** A short daily team meeting, often held standing, in which each member says what they did, what they will do next, and what is blocking them.

**State model:** A diagram showing the stages something passes through, such as an order going from new to filled or rejected, and what causes each change.

**Systems analyst (SA):** A person who works between the business and the engineers, turning business needs into clear, testable requirements and checking that what is built meets them.

**Systems literacy:** A working understanding of how an organization's systems fit together and exchange data, without needing to build them.

**TDD (Test-Driven Development):** A way of programming in which the developer writes an automated test first, then writes the code that makes the test pass.

**Test case:** A single scripted check, with set inputs, steps and an expected result, used to confirm that one requirement works.

**Test data:** Prepared or made-up data used to test a system, such as sample accounts and orders.

**Test pack:** A team's complete set of test cases for a system, kept together so they can be run against each new version (also called a test suite).

**Touchpoint (TP1 to TP4):** One of four scheduled progress reviews of a team's project, held on the Fridays of Weeks 3, 6, 8 and 10.

**Traceability audit:** A check that every requirement can be followed through to the design, code and tests that cover it, so nothing is missed.

**Track:** One of the program's two parallel training paths: Software Engineering or Systems Analyst.

**Trade REST API:** The team's API, built in the REST style, that the rest of the system uses to place and view trades.

**Trading platform:** Software that lets clients buy and sell investments, such as company shares, and see what they own.

**TypeScript:** A version of JavaScript that adds type checking (rules about what kind of data each value may hold) to catch mistakes before the code runs.

**UAT (User Acceptance Testing):** The final stage of testing, in which real or representative users confirm the system does what the business needs before it goes live.

**UAT plan:** A document setting out how UAT will run: who tests, which scenarios they test, and the conditions for starting and finishing.

**UI (User Interface):** The screens, buttons and forms a person uses to work with an application.

**UML (Unified Modeling Language):** A standard set of diagram types for describing the structure and behavior of a software system.

**User story:** A short description of a feature from the user's point of view, usually in the form "As a [type of user], I want [goal], so that [benefit]."

**UX (User Experience):** How easy, efficient and pleasant it is for a person to use a product as a whole.

**Ways of working:** The rules a team agrees on for working together, such as meeting times, how decisions are recorded, and when work counts as done.

**Wireframe:** A simple sketch of a screen's layout that shows where things go, without colors or final design.

**Zero trust:** A security approach in which no user or device is trusted automatically, so every request must prove who it comes from and that it is allowed.
