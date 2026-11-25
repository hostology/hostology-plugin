---
name: hostology-onboarding
description: Use when a venue user asks to set up their venue in Hostology, asks what is left to do in their venue setup or onboarding checklist, or wants to carry on setting up their venue.
---

# Hostology Onboarding

Walk the user through their venue's setup checklist, one step at a time, until every step is done. The Hostology
venue connector's own guidance governs how each tool is used; this skill only sets the course of the conversation.

## 1. Open

Call `list_venues` to find the venue and where its setup has got to.

## 2. Say where things stand

Tell the user which steps are done and which are still to do, using the plain names in the table below, never the
keys. Say which step comes next.

## 3. Do the tool work first

Take the outstanding steps among `billables`, `enquiry-workflow` and `event-workflow` with the user, one at a time:
the catalogue, pricing and payment terms for billables, then the enquiry and event workflows. When a step's work is
finished, ask the user whether it is done, tick it with `complete_onboarding_steps`, and move on.

## 4. Then the portal steps

Go through the remaining outstanding steps in the table's order. For each one, say what it is and where in the venue
portal it is done, and wait for the user to tell you it is done. Then tick it with `complete_onboarding_steps`. If
the step comes back as an error, tell the user and carry on to the next step.

## 5. Close

Call `list_venues` again. If it shows sample data still present, offer to remove it with `remove_sample_data`.
Then confirm that the venue's setup is complete.

## The steps

| key | plain name | where it is done |
|---|---|---|
| `venue-details` | Add your venue details | Venue Settings -> Venue Details |
| `media-images` | Upload media images | the Media page, opened from this step on the venue Dashboard's setup checklist |
| `billables` | Set up your billables | with the assistant (Billable Items and Pricing in the portal) |
| `documents` | Import your documents | Planning -> Documents |
| `templates` | Build your templates | Templates -> Itineraries |
| `invite-colleagues` | Invite your colleagues | My Team, in the account menu |
| `email-templates` | Build your email templates | Templates -> Email Templates |
| `enquiry-workflow` | Set up an enquiry workflow | with the assistant (Planning -> Workflows in the portal) |
| `connect-inbox` | Connect your inbox | Venue Settings -> Integrations |
| `email-hub` | Configure your Email Hub settings | Venue Settings -> Application Settings |
| `test-enquiry` | Send a test enquiry | send an email to the connected inbox and check it arrives in the Email Hub |
| `itinerary-template` | Create an itinerary template | Templates -> Itineraries |
| `event-workflow` | Set up an event workflow | with the assistant (Planning -> Workflows in the portal) |
| `event-templates` | Assemble event templates | Templates -> Event Templates |
| `suggested-suppliers` | Upload your suggested suppliers | Planning -> Suppliers |
| `test-event` | Add a test event | Events: create one and check it |
