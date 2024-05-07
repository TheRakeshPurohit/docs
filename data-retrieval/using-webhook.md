---
description: Get data right into the application whenever the user imports the spreadsheet
---

# 🪝 Using Webhook

Once the user completes importing the spreadsheet in the widget, the impler starts sending spreadsheet data to the callback URL mentioned in the **project**.

If the callback URL is protected, there is a facility to add **header-based authentication**. To activate it you can mention `authHeaderName` in the **project** and its value to the `import` button as `authHeaderValue` prop.

Data will be sent to the application in chunks, you can mention your desired `chunkSize` in **project**.

Data will be sent to the `callbackURL` in the following format,

<table data-full-width="true"><thead><tr><th width="217.33333333333337">Name</th><th width="487">Description</th></tr></thead><tbody><tr><td>template</td><td><code>CODE</code> of the template</td></tr><tr><td>uploadId</td><td>Upload ID</td></tr><tr><td>data</td><td>Array of data in JSON format</td></tr><tr><td>totalRecords</td><td>Total number of records in uploaded spreadsheet</td></tr><tr><td>totalPages</td><td>Total number of pages the data is divided on</td></tr><tr><td>page</td><td>Current page number</td></tr><tr><td>pageSize</td><td>Size of the data being sent</td></tr><tr><td>extra</td><td>Extra string or JSON if it's being passed to <code>Import</code> button</td></tr></tbody></table>

Have any doubts? Shoot us a message directly on [Discord](https://discord.impler.io).
