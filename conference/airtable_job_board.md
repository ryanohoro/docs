## Airtable No Code Job Board

Here we use AirTable and some cloud storage to create an elegant and feature-rich user-driven job board.

### Goals:
1. User-driven content
1. Elegant display (vs. Google Sheets)
1. Moderation
1. Notifications
1. No code
1. No cost

### Sample

<img alt="Sample Custom Gallery View" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/diana_example_gallery.png" width="100%">


### Airtable Base Template

**Skip all the setup.** Use this template link, and click "Copy Base" to get started!

[Airtable Job Board Base](https://airtable.com/shrme2KSoGVdsCt1H/tblDRZRchQH7BLJGa/viwSvg8NIIyLab4QI?blocks=hide)

<img alt="Copy Base" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_copy_base.png">

### Airtable View Manual Setup
1. Sign up for [Airtable](https://airtable.com/). This will be our database and form designer/host. The free account tier should work for our needs

1. In your first project, create a Base "Job Board". This is the database we'll work from.
<img alt="Sample Customized Job Board" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_base_create.png" width="100%">
1. Find the Grid View, give the current table a name, "Jobs".
1. Add the relevant field names in the tops of each column of the table, using the "+" sign to add new fields.
    - Company Name (Single Line)
    - Company Logo (Attachment)
    - Role (Single Line)
    - Location (Single Line)
    - Job Link (URL)
    - Type (Single Select)
    - Approved (Single Select)
1. Add some sample data to your table, set the Type field to "Sponsor" on some, The Approved field to "Yes" on some

<img alt="Sample Table Data" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_table_data.png" width="100%">

1. Create a new form, it will auto-populate with all of the fields
1. Add a title and description to your form
1. Customize the fields on your form, set visibility and order

<img alt="Customize Form" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_form_customize.png" width="100%">

1. Create a new Gallery view
1. Customize the Gallery view Cards to have all but the Company Logo and Approved fields displayed, and the cover field set to "fit"

<img alt="Customize Gallery Cards" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_gallery_cards_customize.png" width="100%">


1. If you'd like to moderate the job postings manually, set a filter for Approved is "Yes". When new jobs are posted, review them and set Approved to "Yes" to display them
1. Set the sort field to Company Name to keep things tidy. If you'd like to tag and prioritize sponsored or other types of listings, sort first by Type (Z -> A), then Company Name

### Share Airtable Links

1. Make sharable links for your Form and Gallery views
1. For more accessible browsing, also create a sharable Grid view link
1. Share these links as needed for your event/organization

### Notifications

Get notified when a new job is posted.

#### Free

When setting up the form, enable "Email me at" to get an email every time the form is submitted

<img alt="Email Notifications" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_email.png">

#### Paid Upgrade (Pro)

Use Automation to connect your Airtable to external services like Slack. Use this to enable moderation, or post new jobs to a channel as they are posted, or approved for moderation

When new posts are submitted, send a notification to a moderation channel

<img alt="Automation for New Post" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_new_post.png" width="100%">

<img alt="Automation for New Post" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_slack_demo.png">


When posts have their Approved field updated, send a notification to the public channel

<img alt="Automation for Approval" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_approved.png" width="100%">

### Customizing the Job Board Layout

1. Create an HTML template, or use the sample [HTML Template](https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/jobs.html) to create a custom layout for your Grid view
1. Get the embed code for the Gallery view, and the shareable links for the Grid and Form views, add them to the custom layout
1. Host the custom layout file on AWS S3, Goole Cloud Storage, GitHub Pages, or any other static hosting option



