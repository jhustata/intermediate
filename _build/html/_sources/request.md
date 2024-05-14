# Data Collection for Prompt Based Programming

## Introduction


The prompt based programming approach is an user-interactive programming approach
that is achieved through Stata's `_request()` option under `display` command. Everytime 
the `_request()` option was called, Stata will pause the current running program/do-file
, print the content in the `display` command, and ask for user input to gather necessary 
information to proceed. Customizing the programs to gather information for key parameters
through this pause-print-request style is called prompt based programming.


The unique information gathering style of prompt-based programming allows programs to:
1) mandatorily request parameters one at a time with instructions 
2) build up check points before executions 
3) allow program to be changed by the user without termination.


These features of prompts may be able to bring various benefits from multiple perspectives 
to help traditional program syntaxes in sitautions like the user is not familiar with 
Stata codes, the user does not know the program well and the instructions are limited, 
or multiple options and long lists need to be specified through syntaxes. The instructed 
parameter intake style requires less user effort to study program syntaxes. 
The introduction of check points, along with the ability to change without termination, 
helps avoid wrong executions thus reduce the costs of error. 


The benefits of prompt based programming apporach may reduce the costs of learning, 
and prevent/fix human error at low costs. In this data collection process, we would like to
gather information about user experience of different programming approaches, and explore
how much the prompt based programming approach may help.


## Main Idea


Through this data collection, piloting users will be given three sets of two programs with 
different programming appraoches (prompt based approach vs. traditional program syntaxes) but
exactly the same functions to achieve the same statistical analytical goals in eahc set. 
These three sets of programs range from simple to very complex. Through the completion of
the analytical goals, user experience like running time and user's subjective opinion about
difficulties of using the two different approach programs will be gathered.


## Program Sets: 


When running the programs, please remember to record the running time displayed in each
program set. If needed, running time may be able to find out through global macros:


Simple Level: `${srt1}` `${srt2}`

Intermediate Level: `${irt1}` `${irt2}`

Complex Level: `${crt1}` `${crt2}`


### Complexity Level - Simple



``` Stata
do "https://raw.githubusercontent.com/Vince-Jin/Prompt/main/prompt_v1.ado"
prompt_v1
```


### Complexity Level - Intermediate


``` Stata
do "https://raw.githubusercontent.com/Vince-Jin/Prompt/main/pilot.ado"
pilot
```


### Complexity Level - Complex


``` Stata
do "https://raw.githubusercontent.com/Vince-Jin/Prompt/main/program753.ado"
program753
```


## User Experience Survey


Please find the excel sheet for user experience information here:
https://docs.google.com/spreadsheets/d/1oQxx83eX7sIIDbyV8frowY8EXuYpRAuudRxnVdfNSQg/edit?usp=sharing

***Please ignore the ID column and use the next available blank row***


### Section 1: Complexity Level - Simple

***Q1:*** Please enter the running time showed for prompt-based programming approach: 

***Q2:*** Please enter the running time showed for traditional program syntax approach: 

***Q3:*** Plesase choose which approach you felt easier to achieve the analytic goal: (1 - Prompt-Based; 2 - Traditional Syntax; 3 - Roughly The Same)

### Section 2: Complexity Level - Intermediate

***Q4:*** Please enter the running time showed for prompt-based programming approach: 

***Q5:*** Please enter the running time showed for traditional program syntax approach: 

***Q6:*** Plesase choose which approach you felt easier to achieve the analytic goal: (1 - Prompt-Based; 2 - Traditional Syntax; 3 - Roughly The Same)

### Section 3: Complexity Level - Complex

***Q7:*** Please enter the running time showed for prompt-based programming approach: 

***Q8:*** Please enter the running time showed for traditional program syntax approach: 

***Q9:*** Plesase choose which approach you felt easier to achieve the analytic goal: (1 - Prompt-Based; 2 - Traditional Syntax; 3 - Roughly The Same)

### Section 4: User Background

***Q10:*** Please indicate how many years you have used Stata: (1 - less than 1 year; 2 - 1 to 3 years; 3 - 3 to 5 years; 4 - more than 5 years)

***Q11:*** Please indicate how you rate your familarity with Stata: (1 - Beginner; 2 - Intermediate; 3 - Advanced; 4 - Expert)

***Q12:*** Please indicate how long you have been used other programming langauge or statistical software (R, Python, C++, Java, HTML, SAS, and etc.): (1 - less than 1 year; 2 - 1 to 3 years; 3 - 3 to 5 years; 4 - more than 5 years)
