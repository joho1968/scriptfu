# scriptfu
Various scripts for automation, devops, etc. Feel free to improve upon them, suggest changes, and so on 😉

| Script        | Description |
| ------------- | ----------- |
| [pflogpy.py](https://github.com/joho1968/scriptfu/blob/main/pflogpy.py)<br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/><br/>| Parse a **Postfix** mail log to summarize daily mail flow<br/><br/>Produces a report similar to **pflogsumm** that includes: Total messages processed (sent, deferred, bounced), Rejected messages and connection attempts, Hourly distribution of mail events (optional), Top senders and recipients<br/><br/>Features:<br/><br/><ul><li>Accepts the date input on the command line in either YYYYMMDD or YYYY-MM-DD format, but still relies on the standard Postfix log timestamp format for parsing logs.</li><li>Option to skip report generation if no mail was processed.</li><li>Option to send the report via email with both plaintext and HTML parts. The HTML part displays the text report using a monospace font.</li><li>Optional command-line parameter to exclude the "Messages per Hour" section.</li><li>Show file differences that haven't been staged</li>|
