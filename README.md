# scriptfu
Various scripts for automation, devops, etc. Feel free to improve upon them, suggest changes, and so on 😉

#### `pflogpy.py`
##### Parse a **Postfix** mail log to summarize daily mail flow.
It produces a report similar to **pflogsumm** that includes:
  - Total messages processed (sent, deferred, bounced)
  - Rejected messages and connection attempts
  - Hourly distribution of mail events (optional)
  - Top senders and recipients

Features:
  - Accepts the date input on the command line in either YYYYMMDD or YYYY-MM-DD format,
    but still relies on the standard Postfix log timestamp format for parsing logs.
  - Option to skip report generation if no mail was processed.
  - Option to send the report via email with both plaintext and HTML parts. The HTML part
    displays the text report using a monospace font.
  - Optional command-line parameter to exclude the "Messages per Hour" section.
