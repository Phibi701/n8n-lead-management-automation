# Lead Management Automation with n8n

## Overview
A basic lead management workflow built using n8n, webhooks, conditional logic, and Google Sheets. The workflow captures student enquiries, checks their course interest, and stores the submitted information in a spreadsheet.

## Tools and Technologies
- n8n
- Webhooks
- IF node for conditional routing
- Google Sheets
- JSON data

## Workflow
1. A webhook receives student enquiry details.
2. The Edit Fields node organizes the incoming data.
3. An IF node checks the student's course interest.
4. The appropriate branch sends the enquiry data to Google Sheets.
5. The spreadsheet stores the enquiry details for further review.

## Sample Input
```json
{
  "student_name": "Test Student",
  "email": "student@example.com",
  "course_interest": "Data Science",
  "enquiry_message": "I would like information about the course."
}
```

## Spreadsheet Fields
- student_name
- email
- course_interest
- lead_status
- category
- ai_priority
- summary

## Current Limitations
This is the basic version of the project. The category, priority, and summary fields use predefined placeholder values. AI-based classification is not implemented in this version.

## Security Notes
Credentials, access tokens, and private webhook URLs are not included in this repository.

## Future Improvements
- Add reliable AI-based enquiry classification.
- Add email notifications.
- Improve error handling and input validation.

## Author
MCA student exploring workflow automation and integrations.
