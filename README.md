# [hire.dev] - Interview Questions Template

This is a template repository you can use to create your own questions
set of questions compatible with hire.dev platform.

### What to do?

Simply clone this template, modify questions.yaml and make sure it's valid against the schema.

- Github action will make sure the README.md is regenerated, so that your questions are open source in a nice format
- In case you use hire.dev, please specify this repository in Questions section of your organisation and import the repo.

## Motivation

At hire.dev, we want to make it possible for a teams to manage their set of interview questions on 
GitHub in form of a simple YAML file.

1. We want team members to actively collaborate on a set of questions that are being asked during the interview process.
2. We believe the questions are more relevant when being built continuously and naturally while building stuff instead of when they are prepared just for the sake of interview process. 
3. Possibility to store them in YAML on GitHub gives people an opportunity to collaborate like on any other project. Ask questions, do pull-request reviews, create issues.
4. The setup of this repo allows for this questions to be either just publicly available on GitHub, or be used as part of hire.dev platform.

## Schema

```
questions:
- title: {question_name}
  type: {full_text,single_choice,multi_choice}
  options: # available just for single_choice,multi_choice questions
  - value: {answer_no_1_text}
    correct: true # only 1 correct answer possible for single_choice questions
  - value: {answer_no_2_text}
  hint: # optional hint 
  body: |
    Body of the question in Markdown to briefly describe the question more in detail
    ~~~python
    # You can even provide code snippets
    ~~~
```

## How does hire.dev question repositories work?

```
                                                                                                      
                                                                                                      
                                            +--------------------------------------+                  
+-------------------+                       |                                      |                  
|Questions repository -------------------------------+    hire.dev                 |                  
|no.1               |                       |        |                             |                  
|                   |  hire.dev pulls       |  +-----|-----+                       |                  
|+ questions.yaml   |  data from the repo   |  |           |                       |                  
+-------------------+                       |  |           |                       |                  
                                            |  |           |                       |                  
                                            |  | Company's |                       |                  
                                            |  | question  |    Job Pipeline       |                  
+-------------------+                       |  | database  |    of a specific      |                  
|Questions repository--------------------------|           |    interview          |                  
|no. 2              |                       |  |           |    +-----------------+|                  
|                   |                       |  +-----|-----+    | Introduction    ||                  
|+ questions.yaml   |                       |        |          +-----------------+|                  
+-------------------+                       |        |          +-----------------+|                  
                                            |        +----------- Questions block ||                  
                                            |  A subset of      +-----------------+|                  
                                            |  questions        +-----------------+|                  
                                            |  is chosen for    | Online meeting  ||                  
                                            |  each individual  +-----------------+|                  
                                            |  job type         +-----------------+|                  
                                            |                   | Final block     ||                  
                                            |                   +-----------------+|                  
                                            +--------------------------------------+                  
                                                                                           
```
