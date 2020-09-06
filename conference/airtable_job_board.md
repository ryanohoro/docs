## No or Low Code Job Board

Here we use AirTable and some cloud storage to create an elegant and feature-rich user-driven job board.

### Goals:
1. Low code
1. Negligible cost
1. Elegant display options (let's improve on Google Sheets)
1. User-driven content
1. Moderation
1. Monitoring/notifications

Skip all the Airtable view setup and use this template link. Click "Copy Base" to get started!

https://airtable.com/shrme2KSoGVdsCt1H/tblDRZRchQH7BLJGa/viwSvg8NIIyLab4QI?blocks=hide

### Airtable View Setup
1. Sign up for AirTable. This will be our database and form designer/host. The free account tier should work for our needs.
https://airtable.com/
1. In your first project, create a Base "Job Board". This is the database we'll work from.
1. Find the Grid View, give the current table a name, "Jobs".
1. Add the relevant field names in the tops of each column of the table, using the "+" sign to add new fields.
  - Company Name (Single Line)
  - Company Logo (Attachment)
  - Role (Single Line)
  - Location (Single Line)
  - Job Link (URL)
  - Type (Single Select)
  - Approved (Single Select)
1. Create a new form. It will auto-populate with all of the fields
1. Add a title and description to your form
1. Customize the fields on your form, set visibility and order
1. Add some sample data to your table to try out the features, set the Type field to "Sponsor" on some, The Approved field to "Yes" on some
1. Create a new Gallery view
1. Customize the gallery view to have all but the Approved field displayed, set the cover field to "fit"
1. If you'd like to moderate the job postings manually, set a filter for Approved is "Yes". When new jobs are posted, review them and set Approved to "Yes" to display them
1. Set the sort field to Company Name to keep things tidy. If you'd like to tag and prioritize sponsored or other types of listings, sort first by Type (Z -> A), then Company Name
1. Create a Text View for more accessible browsing
1. Make sharable links for your Form and Gallery views
1. For more accessible browsing, also create a sharable Grid view link
1. You're all set! Share these links as needed for your event/organization

### Airtable Notifications

To get notified when a new job is posted, you have two options:

 - Free: When setting up the form, enable "Email me at" to get an email every time the form is submitted
 - Paid Upgrade: Use Automation to connect your Airtable to external services like Slack


### Customizing the Job Board Layout

1. Create an HTML template, or use the sample (/airtable_job_board/jobs.html)[HTML Template] to create a custom layout for your Grid view
1. Get the embed code for the Gallery view, and the shareable links for the Grid and Form views, add them to the custom layout
1. Host the custom layout file on AWS S3, Goole Cloud Storage, GitHub Pages, or any other static hosting option



