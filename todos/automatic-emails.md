```
STATUS: PROPOSED

PROBLEM
We need a way to send emails when users create different kinds of content through the api (only).

PROPOSAL:
Create a "after-create" template for email. 
If the template exists, then it gets sent. 
If it does not exist, then it does not get sent.

TEMPLATE URL FORMAT:
"email-[kind]-after_create"

Example:
"email-product-after_create"

TAGS:
The post tags will be available within the template.

Additionally, other tags will be available as well:

{{approve_url}} - a url so the user can set the post to active
{{disable_url}} - a url so the user can set the post to be deleted
{{delete_url}} - a url so the user can delete the post
```
