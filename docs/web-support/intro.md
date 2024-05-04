---
sidebar_position: 1
---

# Livestream Pre-Configuration Documentation

> Prior Access Needed:
>
> - Bitwarden Password Vault
> - Slack
> - Restream Dashboard — login creds via Bitwarden
> - Metro Sanity Studio CMS — login creds via Bitwarden

## 1. Download Bulletins

1. Find and download the bulletins — you can usually find these in the
   `#web-support-rotation` Slack Channel, where Donny usually sends the “Final
   Draft” on Saturdays. If you can’t find them there, ping Paul.

## 2. Configure Restream for FB and YT descriptions

1. Go to https://app.restream.io/channel — (login credentials can be found in
   Bitwarden).
1. Navigate to the "Channels" page (the url ending should be /channel)
   1. If coming from the homepage, it's the link “Set up for OBS, Zoom, etc.“
1. **Click 'Update Titles'** to open text box modals.
   1. _NEW FOR 2024_ — Just update the Date in the title; no further changes
      need to be made! ![Restream image](/img/docs/web-support/01_restream.png)

```

TITLE INPUT:

Metro's Sunday Service — March xx, 20xx — 11:30 AM



DESCRIPTION BODY INPUT:


Metro exists with the hope to "renew, retrain, and rebuild" the surrounding areas of Philadelphia, PA—through Christ-centered worship, genuine community, incarnational ministry, and radical generosity. To learn more about us, please visit us at https://metrophilly.org.

» For resources to this video: https://metrophilly.org/live
» For our children's program: https://metrophilly.org/kids
» For tithes and donations: https://metrophilly.org/give
» View our latest links: https://metrophilly.org/links
» To let us know you'd like to get connected, text METRO to the number 94000

Stay connected with us:
» Website » https://metrophilly.org
» Facebook » https://facebook.com/metroeastfalls
» Instagram » https://instagram.com/metroeastfalls
» Youtube » https://mtro.cc/youtube
» X » https://x.com/metroeastfalls


```

4.  Submit form by clicking "Update all"

![Restream image](/img/docs/web-support/02_restream.png)

5.  NEW FOR 2024 — Update the time in the title for Metro Intrastream from 11:30
    to 9:30 by going into “Edit Settings”.

## 3. Configure Sanity CMS for the site’s Sermon and Sunday Service Event

### Uploading into Website

> New for 2024: LivestreamEvent has been deprecated in favor of Sermon and
> SundayServiceEvent! Read the descriptions of the new fields carefully!

1. Go to Metro’s Sanity Studio dashboard:
   https://metrochurch.sanity.studio/desk/

2. Configure a Sermon sanity document

   1. Click the “🎤 Sermon” content folder
   2. Click the + (plus sign) icon to create a new Sermon
      1. Protip – you can just ‘duplicate’ the latest sermon by clicking into
         the latest, clicking the 🔽 arrow (next to the large gray “Publish”
         button), and clicking “Duplicate”.
   3. Use the previously downloaded bulletins to match the info here.
      1. Note: Make sure to leave all “Media Paths” blank here!
   4. Click “Publish” to save your changes

3. Configure a Sunday Service Event sanity document
   1. Click the “⛪️ Sunday Service Event” content folder
   2. Click the + (plus sign) icon to create a new Sunday Service Event
      1. Protip – you can just ‘duplicate’ the latest sermon by clicking into
         the latest, clicking the 🔽 arrow (next to the large gray “Publish”
         button), and clicking “Duplicate”.
   3. Link the previously created Sermon document as a Sermon reference here
   4. Upload the downloaded bulletins here, making sure to match the correct
      bulletins to the correct services.
      1. Note: Make sure to leave the “Livestream Youtube ID” blank here.
   5. Click “Publish” to save your changes
4. Final checks: Make sure that there aren’t any “edits pencils” or “saving
   spinners” on any of the documents!

## 4. Deploy to Prod

1. In the main nav bar, click into the “Deploy” dashboard section, and hit the
   big green Deploy button to kick off a Vercel build

## 5. Shift the Trello card to the “In Review” column

And that’s it!
