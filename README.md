# Microsoft Candidate Evaluation Program

This is a simple C program that simulates a candidate evaluation process for a job at Microsoft. It takes various inputs from the user, including personal details, academic information, and internship experience, then evaluates whether the candidate qualifies for an interview based on predefined criteria. Afterward, the candidate's performance in an interview is assessed based on various parameters, and they are assigned a role and salary package.

## Features

- Takes input from the candidate including:
  - Name
  - CGPA
  - Number of credits
  - Certifications
  - Referrals
  - Years of experience
  - Internships
- Determines if the candidate qualifies for an interview based on certain eligibility criteria.
- After qualifying for an interview, the candidate is asked to input marks for various hiring parameters:
  - Technical knowledge
  - Coding skills
  - Innovation
  - Personality
  - Communication skills
- Based on the total marks from the interview, and years of experience, the program assigns a role and salary:
  - Project Manager (30 LPA)
  - Assistant Manager (25 LPA)
  - Software Engineer (20 LPA)
  - Software Developer (15 LPA)
  - Junior Software Engineer (10 LPA)
  - Intern Software Engineer (5 LPA)
  - Rejected (if below certain criteria)

## How to Run the Program

### Requirements
- A C compiler (e.g., GCC or Clang)
- A terminal or command line interface

### Steps to run:
1. Clone the repository or download the `candidate_evaluation.c` file.
   
   ```bash
   git clone https://github.com/your-username/microsoft-candidate-evaluation.git
   ```

2. Open the terminal and navigate to the directory where the file is located.

3. Compile the program:

   ```bash
   gcc candidate_evaluation.c -o candidate_evaluation
   ```

4. Run the compiled program:

   ```bash
   ./candidate_evaluation
   ```

5. Follow the on-screen prompts to enter the candidate's details and interview evaluation parameters.

## Example Output

```
Enter your name: 
JohnDoe
Enter cgpa: 
8.7
Enter number of credits: 
6
Enter number of certifications: 
3
Enter number of referals: 
2
Enter number of years of experience: 
5
Enter number of internships: 
2

NAME: JohnDoe 
CGPA: 8.700000 
CREDITS: 6 
CERTIFICATIONS: 3 
REFERALS: 2 
YEARS OF EXPERIENCE: 5 
NUMBER OF INTERNSHIPS: 2 

THE CANDIDATE IS ACCEPTED FOR AN INTERVIEW IN MICROSOFT
IN THE INTERVIEW CANDIDATE WILL BE GIVEN MARKS OUT OF 10 FOR EVERY HIRING PARAMETER

Enter marks for technical knowledge: 
8
Enter marks for coding skills: 
7
Enter marks for innovation: 
8
Enter marks for personality: 
7
Enter marks for communication skills: 
8

TECHNICAL KNOWLEDGE: 8 
CODING SKILLS: 7 
INNOVATION: 8 
PERSONALITY: 7 
COMMUNICATION SKILLS: 8 
total marks= 38 
CANDIDATE HAS BEEN HIRED AS ASSISTANT MANAGER
CANDIDATE WILL RECEIVE PACKAGE OF 25 LPA
```

## Program Logic

1. **Eligibility Check**: 
   - A candidate is eligible for an interview if:
     - CGPA is >= 8.5
     - Credits are >= 5
     - Certifications are >= 2
     - Referrals are >= 1
     - Internships are >= 1

2. **Interview Evaluation**: 
   - Candidates who pass the eligibility check will be asked to provide marks for the following interview parameters:
     - Technical knowledge
     - Coding skills
     - Innovation
     - Personality
     - Communication skills
   - Total marks are calculated by summing the individual marks for these parameters.

3. **Role Assignment**:
   - Based on the total marks and years of experience, the program assigns one of the following roles:
     - Project Manager (30 LPA)
     - Assistant Manager (25 LPA)
     - Software Engineer (20 LPA)
     - Software Developer (15 LPA)
     - Junior Software Engineer (10 LPA)
     - Intern Software Engineer (5 LPA)

## Contributions

If you would like to contribute to this project, feel free to fork the repository, make changes, and create a pull request. All contributions are welcome!


### Key Sections Explained:
- **Features**: This section describes what the program does at a high level.
- **How to Run the Program**: Instructions on how to download, compile, and run the program.
- **Example Output**: A sample of what the user will see when they run the program.
- **Program Logic**: Explains the decision-making process behind eligibility and role assignments.
- **Contributions**: Invites others to contribute to the project.
- **License**: Includes licensing information. You can replace it with a more specific license if needed.


