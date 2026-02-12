# LEAP Species Approval Page

A standalone GitHub Pages site for editing and approving species submissions from the LEAP Wetland Monitoring app.

## How it works

1. When a lower-level user submits a new species, an approval email is sent to admins.
2. The "Edit and Approve" link in the email points to this hosted page.
3. The page fetches the species request data from the Supabase edge function.
4. The admin can edit the species details and approve or reject the submission.

## Setup

1. Push this repo to GitHub.
2. Enable GitHub Pages in the repo settings (deploy from `main` branch, root `/`).
3. Update the `send-species-approval-request` edge function to use the GitHub Pages URL for the edit link.

## URL Format

```
https://jessicanasica.github.io/leap-species-approval/?id=REQUEST_ID&token=TOKEN
```
