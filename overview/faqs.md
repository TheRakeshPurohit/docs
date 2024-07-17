---
description: Find answers to most common questions our users have while using Impler
---

# 👥 FAQs

<details>

<summary>How to get TemplateId, ProjectId, and Access Token?</summary>

1. Open the Import description and go to the Snippet portion of the Import.
2. Open the last item of the accordion, where you will find the necessary keys.

<img src="../.gitbook/assets/image (5) (1).png" alt="Steps to get ProjectId, TemplateId and AccessToken for the Import" data-size="original">

</details>

<details>

<summary>While making call to my API, do I need to provide our own authorization header value?</summary>

Yes, you need to provide your authorization header value, which you can provide from the front end.

</details>

<details>

<summary>If I use Axios in my custom validator, will it pass the cookies from my logged-in user to my server, or is the validator call being made from Impler's servers?</summary>

No, logged-in user cookies won't be passed to your server. Validator calls are being made from Impler's servers.

</details>

<details>

<summary>Is there any way to access user uploaded file?</summary>

Yes, Impler provides a REST API endpoint to fetch a user-uploaded file. Here is CURL,

```
curl --location --request GET 'https://api.impler.io/v1/upload/:uploadId/files/original' \
--header 'accesskey: <ACCESS_TOKEN>'
```

You can get `:uploadId` using `Upload Complete` event and `ACCESS_TOKEN` will be available from the Settings panel.

API will send a file with headers `Content-Type` and `Content-Disposition` as values for file type and filename respectively.

</details>

Still, have any doubts? Please shoot us a message directly on [Discord](https://discord.impler.io).
