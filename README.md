# n8n Form to Email Automation Workflow

This project is an automation workflow built using **n8n**.  
It collects user details from a form, stores the data in **Google Sheets**, checks the user occupation, and sends an automated email through **Gmail**.

## Project Overview

The workflow starts when a user submits a form.  
After submission, the entered data is added to a Google Sheet.  
Then the workflow filters and checks the submitted values using conditional logic. Based on the user occupation, it sends a suitable email message automatically.

This project shows how to connect form submission, spreadsheet storage, condition-based routing, and email automation in one workflow.

## Workflow Steps

1. **On form submission**  
   The workflow is triggered when a user submits the form.

2. **Append row in sheet**  
   The submitted user data is stored in Google Sheets for record keeping.

3. **Filter**  
   The workflow filters the incoming data before further processing.

4. **Switch**  
   A switch condition checks the user's occupation or category.

5. **Send a message / Send a message1**  
   Based on the condition, different email messages are prepared and sent.

6. **Merge**  
   The workflow merges the outputs from different branches.

7. **Send a message2**  
   A final email step is executed after merging the branch results.

## Tools and Services Used

- **n8n**
- **Google Forms / Form Submission Trigger**
- **Google Sheets**
- **Gmail**
- **Conditional Logic (Filter and Switch nodes)**

## Example Use Case

A user submits their details such as:
- Name
- Email
- Occupation

The workflow stores this information in Google Sheets and sends a personalized email based on the occupation selected by the user.

For example:
- If the occupation is **Engineer**, one message can be sent
- If the occupation is **Other**, another message can be sent

## Output

- User data is saved in **Google Sheets**
- Automated email is sent through **Gmail**
- The workflow handles multiple conditions using branch logic

## Features

- Automated form submission handling
- Google Sheets integration
- Condition-based email routing
- Gmail email automation
- Organized workflow with merge logic

## Files to Include in GitHub

- `README.md` – Project documentation
- `workflow.json` – Exported n8n workflow file
- `screenshot.png` – Workflow screenshot

## How to Use

1. Import the workflow JSON file into n8n
2. Connect your Google Sheets account
3. Connect your Gmail account
4. Configure the form trigger
5. Update the filter and switch conditions as needed
6. Execute the workflow
7. Submit the form and verify:
   - data is stored in Google Sheets
   - email is sent through Gmail

## Project Purpose

The aim of this project is to automate user data collection and email communication.  
It reduces manual work by automatically storing submitted details and sending condition-based email responses.

## Conclusion

This project demonstrates a practical workflow automation use case using n8n. It integrates form handling, spreadsheet storage, conditional branching, and email delivery into a single automated pipeline.
