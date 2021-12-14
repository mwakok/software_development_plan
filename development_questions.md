# Software Development Plan

A Software Development Plan can help provide a framework to understand your research software. It acts as a basis for software design, development, and maintenance, and can guide your software engineering decisions. This document contains a list of questions that can help a researcher to scope the requirements for developing (complex) research software with longer project lifetimes. 

The sections and questions are based on the multiple [references](resources.md).


## 1. Project Introduction
_Brief introduction of the project to provide insight into the purpose behind the software development plan, and the objective you are trying to achieve._

### 1.1 Project goal

- What is the purpose of your software?
- What research question will your software answer?
- What will be the name of your software?
    - Is this name unique and meaningful, and not in violation with any existing trademarks held by others?

### 1.2 Definitions, acronyms, and abbreviations
_Please list all definitions, acronyms, and abbreviations_


### 1.3 References
The documents listed below were either used to create this document or are referenced in it:
- [TU Delft - Software Policy Guidelines](https://doi.org/10.5281/zenodo.4629662)
- [The Software Sustainability Institute - Checklist for a Software Management Plan](https://doi.org/10.5281/zenodo.2159713)



## 2. Project Overview
_This is where you summarize aspects of the project that will be undertaken and need to be considered during the development. Here you will want to list out your UI/UX requirements, software requirements specifications, and principal research output._


### 2.1 Project description
_Please give a description of the proposed software._

- What are the software requirements?
    - UI/UX requirements
    - Deployment
    - ...

- What are the project deliverables?
- What needs are fulfilled by using the software?


### 2.2 Research impact
_Decribe how your software can impact your field of research._

- Will the software help your users, or yourself, to conduct research more easily? Produce results more rapidly? Produce results to a higher degree of accuracy or a finer level of detail? Exploit the power of super-computers?
- Will it help your users, or yourself, to further research by enabling research that cannot be done at present?
- Will your software, in some form, implement a novel solution to a research problem?
- What are the limitations of similar research software that already exists? How will your software be better?
- What are the foreseen benefits for each type of user?

### 2.3 How will you measure your software's contribution to research?
- What evidence do your funders and other stakeholders expect you to present to show that your software has contributed to research?
- Will you measure who has downloaded your software?
- Will you measure who has used your software?
- Will you gather information on publications that describe research which your software has helped to enable, including those by other researchers?
- Do you intend to have a recommended reference or citation for your software?

### 2.4 How will your software relate to other research objects?
- Which published research objects relate to your research software?
- Are there published papers that describe the research that your software will enable?
- Will your software extend or depend upon other research software?
- Will your software consume data sets or invoke online services?
- Will you publish papers about the research you have done to which your software has contributed?
- Will you publish any data sets produced by your software?


### 2.5 Users and use cases
_It is important to design your software with the users and particular use cases in mind. This paragraph discusses the user requirements._

- Who are the intended users of your software?
    - Is there user type or are there many?
    - Is your software for those new to the research field, for experts, or for the general public?

- How will each user type interact with the software?
    - Do users need to install, configure, or change the software?
    - What system requirements (OS, web browser, compiler, programming language) does a user need? Are these common?
    - What knowledge do users need to use the software?
    - What does each user type need to know in order to use the software?

- Will you invite (outside) developers to contribute to the software?
    - How can external developers contribute to the software?
    - Will you provide contributing guidelines?
    - Will your software accept plugins?

- How will you support those who use the software?
    - What level of support will you offer, if any?
    - For how long will you provide support?
    - How will users ask for help?
    - How do you manage issues?
    - Will you publish a record of issues?


## 3. Project Organization
_This part is critical for defining how the project will be structured, how communication among team members will work, and what the general flow of the project will look like._


### 3.1 Development team
- Who is the project lead?
- Who is part of the development team?
- How will team members join and leave the project?
- What do new team members need to know before joining the project?
- How do developers receive credit for their contribution?


### 3.2 Roles and responsibilities
- What are the responsibilities of the involved team members?
- How are the involved team members held accountable for their responsibilities?


### 3.3 Communication plan
_Ensuring clear communication is important in developing software, especially whith remote developers._

- Which communication channels will be used during the project?
- How will team members have access to software development documentation?
- How will software development decisions be recorded and shared?
- How often will team members report on their progress?


## 4. Software development process
_This section describes the software you will develop._

### 4.1 Software Requirements

- What stack will the software depend upon?
     - Is this stack common in your research domain? 
- What third-party libraries are used?
    - What licenses do these libraries carry?


### 4.2 Software Architecture
_If your software depends on external services, accepts plugins, or is build from multiple modules, it can be useful to create a diagram describing how the various components interact. A straightforward model to follow is the [C4 model](https://c4model.com/), which separates the software architecture into 4 conceptual levels._

- Will the software extend or depend upon other research software?

- What functional modules will the software contain?
    - Will the software rely on plugins?
    - Can the modules be abstracted into layers?

- In what order should these modules be developed?
    - Can you identify which modules are mandatory and optional?
    - Can you draw the evolution of the addition of modules?
    - Can you estimate the development duration of each module?

- How do the modules depend on each other?
- How do these modules interact?
    - Describe the API calls

- What computer hardware resources are required for the development environment?
- What computer hardware resources are required for the production environment?
- What resources are needed to deploy the software?
    - Is this requirement constant?
    - Is the deployment scalable?

- Will the software need to access system information?

### 4.3 Software availability
_This paragraph describes possible considerations for releasing your research software._

- Will you release your software at all?
- Will you release binaries, libraries or packages?
- Will you release your source code? Do your funders, or other stakeholders, require you to release your source code?
- Under what kind of license will you make your software available?
    - Please check the TU Delft's [Software Policy Guidelines](https://doi.org/10.5281/zenodo.4629662)
- How will users find and access your software?
- Will users have to register to access or use your software?
- Will your software be accessed as an online service or via a web portal?
- Will you charge users a fee to access or use your software? What will the revenue generated by these fees be used for?


### 4.4 Long-term availability
_Describe how you will ensure the long-term availability of your software._

- Will you deposit releases of your software into a digital repository?
- What digital repositories are appropriate for you to use?
- Has your funder or publisher recommended or mandated a digital repository to use?
- Does the digital repository give you a unique persistent digital identifier for your deposit?
- Can the digital repository accommodate the size of your deposit?
- Are the policies of the digital repository acceptable to you?
- Is the longevity of the digital repository acceptable to you?


### 4.5 Data pipeline
_Paragraph on the usage of data by the software. Most of these points will also be covered by the Data Management Plan._

- What data will the software need access to?
- How much data will be processed?
- Where is the data stored?
- Are there any security or privacy risks associated with the data?
- Will you publish any data produced by the software?


### 4.6 Software quality standards
_This paragraph shall describe or reference the standards to be followed for software requirements, design, code, test cases, test procedures, and test results._

- Will the software be accompanied by a testing framework?
- Which tools will developers need to develop the software?
- Will test, build, and release rely on Continuous Integration?
- Will the developers need to follow specific formatting, linting, or other code quality checks?

- How long do you expect to maintain the software?
    - What measures will be taken during the project to ensure the (long-term) sustainability of the software?

### 4.7 Documentation
_Software documentation comes in various forms with various purposes._

- How will you provide user documentation?
- How will you provide developer documentation?
    - Will you generate an API reference list?
- Will you provide use examples?
- Will you provide tutorials?
- Will you provide audio or video explanations?

## 5. Project Management
_This paragraph defines the various plans you will follow for managing risks, timelines, budgeting, and so on._


### 5.1 Scheduling
The software development process consists of four major steps:

1. Planning
1. Implementing
1. Testing
1. Deployment and Maintenance

**Suggestion:** organize the software development as work packages in a Gantt chart

- What deadlines need to be taken into account?

### 5.2 Risks
- Do the developers have the required digital competences to develop your research software?
    - If not, how will they acquire these competences?
    - Does training impact the software development timeline?


- Sufficient developers
