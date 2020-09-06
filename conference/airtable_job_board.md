## Airtable No-Code Job Board

Here we use AirTable and some cloud storage to create an elegant, feature-rich, and user-driven job board.

### Goals:
1. User-driven content
1. Elegant display (vs. Google Sheets)
1. Moderation option
1. Notifications
1. No code
1. No cost

### Sample

<img alt="Sample Custom Gallery View" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/diana_example_gallery.png" width="100%">

### Airtable Base Template

**Skip all the manual setup.** Use this template link, and click "Copy Base" to get started!

[Airtable Job Board Base](https://airtable.com/shrme2KSoGVdsCt1H/tblDRZRchQH7BLJGa/viwSvg8NIIyLab4QI?blocks=hide)

<img alt="Copy Base" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_copy_base.png" width="200px">

### Airtable Manual Setup
1. Sign up for [Airtable](https://airtable.com/) - a SaaS database host and UI designer - with the free account tier.

1. In your first project, create a Base "Job Board" - the database we'll work from.

    <img alt="Sample Customized Job Board" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_base_create.png" width="50%">

1. Find the Grid View, give the current table a name, "Jobs".
1. Add the relevant field names in the tops of each column of the table, using the "+" sign to add new fields.
    - `Company Name` (Single Line)
    - `Company Logo` (Attachment)
    - `Role` (Single Line)
    - `Location` (Single Line)
    - `Job Link` (URL)
    - `Type` (Single Select)
    - `Approved` (Single Select)
1. Add some sample data to your table, set the Type field to "Sponsor" on some, The Approved field to "Yes" on some.

    <img alt="Sample Table Data" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_table_data.png" width="100%">

1. Create a new form, it will auto-populate with all of the fields.
1. Add a title and description to your form.

    <img alt="Customize Form" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_form.png" width="100%">

1. Customize the fields on your form, set visibility, order, and required properties.

    <img alt="Customize Form" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_form_customize.png" width="50%">

1. Create a new Gallery view.
1. Customize the Gallery view Cards to have all but the `Company Logo` and `Approved` fields displayed, and the cover field set to "fit".

    <img alt="Customize Gallery Cards" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_gallery_cards_customize.png" width="50%">

1. If you'd like to moderate the job postings, set a filter for `Approved` **is** "Yes".
    - When new jobs are posted, review them, and manually set `Approved` to "Yes" to allow them to be displayed.
    <img alt="Filter Table" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_table_filter.png" width="60%">
    - You may want to note on the submission form that listings will be moderated, and won't appear immediately.
1. Set the sort field to `Company Name` to keep things tidy.
    - If you'd like to tag and prioritize sponsored or other types of listings, sort first by `Type` (Z -> A), then `Company Name`.
    <img alt="Sort Table" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_table_sort.png" width="60%">

You should have a nice looking, filtered, and sorted Gallery view.

<img alt="Sample Customized Job Board" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_gallery_demo.png" width="50%">

### Share Airtable Links

1. Make shareable links for your Form and Gallery views.
    
    <img alt="Shareable Link" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_form_shareable.png" width="60%">

1. For more accessible browsing, also create a shareable Grid view link.
1. Share these links as needed for your event/organization.

### Notifications

Get notified when a new job is posted.

#### Free

When setting up the form, enable "Email me at" to get an email every time the form is submitted.

<img alt="Email Notifications" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_email.png" width="50%">

#### Paid Upgrade (Pro)

Use Automation to connect your Airtable to external services like Slack. Use this to enable moderation, or post new jobs to a channel as they are posted, or approved for moderation.

When new posts are submitted, send a notification to a moderation channel.

<img alt="Automation for New Post" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_new_post.png" width="100%">

When posts have their `Approved` field updated, send a notification to the public channel.

<img alt="Automation for New Post" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_approved.png" width="100%">

You should see a notification to your preferred channel when either event is triggered.

<img alt="Sample Slack Post" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_automations_slack_demo.png" width="70%">

### Customizing the Job Board Layout

1. Create an HTML template, or use the sample [HTML Template](https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/jobs.html) to create a custom layout for your Grid view.
1. Get the embed code for the Gallery view, and the shareable links for the Grid and Form views, add them to the custom layout where the placeholder links are.

    <img alt="Gallery Embed Code" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_gallery_embed.png" width="30%"><img alt="Gallery Embed Code" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/airtable_gallery_embed_code.png" width="70%">
    <img alt="Gallery Embed Code" src="https://github.com/ryanohoro/docs/raw/main/conference/airtable_job_board/images/custom_html_template.png" width="100%">


1. Host the custom layout file on AWS S3, Google Cloud Storage, GitHub Pages, or any other static hosting option.



