---
name: becky-client-config
description: Becky's saved settings for this account. Becky reads this every time she runs.
metadata:
  type: project
---

# Becky config

Becky fills this in during the first-run wizard. After that she reads it every time and never asks again. Edit by hand only if something changes (new designer email, switched account, expired token, etc.).

## Account
- **Instagram username**: <@theirhandle>
- **Instagram user ID**: <numeric - if pipeboard or graph>

## Instagram access
- **Method**: <pipeboard | apify | graph>
- **Apify token**: <only if method is apify>
- **Graph API token**: <only if method is graph - long-lived, expires ~60 days>

## Delivery
- **Email recipients**: <them@theirdomain.com, designer@theirdomain.com>
- **Transcripts**: <on | off>
- **Doc delivery**: <google-doc | local-file>
- **Email delivery**: <gmail | none>

## Schedule
- **Runs**: <every 30 days - 1st of each month, ~9am - set via /schedule>

## Notes
<Anything Becky learns about this account that future-Becky should know.>
