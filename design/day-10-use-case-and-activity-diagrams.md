# Use Cases and Activity Diagrams
## Functional vs Non-functional Specifications 
- Functional: E.g. Able to login, able to view stuff, etc.
- Non-functional: E.g. Program taking too long to query, login process too long resulting in timeouts 
- Usually get users to sign off (to compare the specifications with the delivered system)
- Need precise diction to make sure there are no mistakes in understanding the requirements

## Functional Requirements
- Able to estimate cost, time and resources to develop the system 
- Estimates prior that will depend on the amount of info available 
- Updated estimates to be given as planning goes on 

## Deliverables
- User Requirement Specifications 
  - Functional Requirements 
    - Use Case Model with details 
    - Screen Designs and Flows (paper design - screens & reports)
  - Non Functional Requirements 
    - Performance (system response time)
    - Volume (no. of users, data, future growth)
    - Security (user roles & tasks)
    - Reliability (recovery time, down time)
    - Usability
  - Glossary

## User Stories Extended
- User stories meant to simulate the requirements of the people using the system 
- Need to also include the system's perspective
  - Timer (Scheduler)
  - External and existing system
  - Sensors
  - Counters (e.g. tour booking should be closed if the quota has been met with a counter)

## Current Systems 
- Some potential reasons for investigating the current system 
  - Old functionalities might be necessary
  - Data must be migrated
  - Tech documentation may provide more details of processing algorithms
  - Defects of old system must be avoided
  - May need to retain some parts of the old system

## User Case Models 
- Need to have secure software design and coding habits 
- Actors will initiate the events 
- If the event points to the actor, then it means the system will periodically trigger the actor 
- Keep it to system scope, don't bother creating flows for features that your system isn't handling 
  - E.g. user receives email (the user will read their own email on whatever server they use)

### Find Actor and Use Cases
- Actors should be a unique role 
- Staff can have more than 1 role (e.g. library user and a librarian)
- Multiple groups of staff playing same role
  - E.g. library users who are registered as a public member vs Library users who are the university teaching staff

## Activity Diagrams 
- Ignore exceptions 
- Activity tables no longer used
- Work on tour booking system for workshop

## Interviewing Skills (Requirement Gathering)
- Anthrographic - Studying of human science? 

### Background Reading 
- Advantages
  - Better understand the organisation
  - Better prepare for types of fact finding 
  - Documentation of existing system can help to identify limitations/requirements for functionality of new system
- Disadvantages 
  - Outdated materials
  - Written may not be the actual current practice 

### Observation 
- See what really happens, not what people say happen 
- Includes: 
  - How people carry out processes 
  - What happens to docs 
  - Obtaining quantitative data as a baseline for improvements 
  - Following a process through end-to-end
- Advantages:
  - First-hand experience on how the system operates
  - High level of validity on data
  - Verifies info from other sources 
- Disadvantages
  - People may behave differently, distorting findings 
  - Requires training and skill 
  - Logistical problems for staff who work shifts 
  - Ethical problems with personal data

### Document Sampling
- See info requirements that people need 
- Advantages: 
  - For gathering quantitative data 
- Disadvantages: 
  - Not helpful if system is going to change drastically 

### Questionnaires 
- Likert Scale (Research process for creating a survey)
- Odd scale (5 checkboxes) reduces the chance of a question resulting in a 50-50 response
- Advantages: 
  - Economical way of gathering info from large number of people 
  - Effective way of gathering info from geographically dispersed people 
  - Well designed questionnaire can be analysed by a computer 
- Disadvantages 
  - Good questionnaires are difficult to design
  - No auto way of following up or probing more deeply
  - Postal questionnaire suffer from low response rates 

### Participatory Design 
- User Centred Design (in Scrum - User is the product owner)

### Focus Group 
- To justify weird trends that is found in surveys 
- Some people pick the same people that was part of the survey as a representative
- Some people pick a different person to get more perspectives 
- Or just have a mix of the 2

### Interviews
- Advantages 
  - Can adaptively respond to what was being said (to get more information)
- Disadvantages 
  - Time consuming and costly 
  - Notes must be written up or tapes transcribed after the interview 
  - Facts can be biased 
  - Interviewees can provide conflicting info


## Questionnaire Design
```
--> Basic Info 
--> Classification Info
--> Indentifcation Info 
--> Opening Questions to get respondents interest 
--> Begin with open questions 
--> Begin with simple questions
--> Place difficult or embarassing or personal questions well down the body of the questionnaire 
```

## Minimizing Questionnaire Errors 
- Cannot remember requested info 
- May be motivated to answer incorrectly to provide a better personal image 
- May not understand what's being asked 
- May not know the answer 
- Determine amount of time a respondent can reasonably devote to a questionnaire 
- Don't ask embarrassing or loaded question 
- Explain difficult questions and use simple vocab
- Don't ask for info that the respondent wouldn't know 
- Avoid suggesting a response ("You do read a newspaper everyday, don't you?")
- Anticipate the context of the responses 
- Cushion questions that may seem unreasonable to the respondent
- Avoid talking down or otherwise insulting the intelligence of the respondent

