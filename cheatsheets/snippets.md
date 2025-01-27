## SNIPPETS

#### Introduction
Snippets are small pieces of text that you can create in  the snippets area of the admin. Once you create a snippet, you can include it in the template like so:

`{% snippet 'name' %}`

Additionally, you can include any kind of content you create like blogs etc by doing this: `{% snippet 'id:123-3453465-242423' %}`

Where `"123-3453465-242423"` is the id of a blog, product, or any other piece of content in your admin. The second form only pulls out the content area of your post.


#### GETTING THE ID
---
Extract the ID of a piece of content you are editing.  For example, if the URL in your admin area looks like this while you're editing the content:

`https://app.travelagencytribes.com/admin/content/update/31bdz659-a1bf-4775-9f86-61dd4d342e91`

To display the content you'd use this:
`{% snippet 'id:31bdz659-a1bf-4775-9f86-61dd4d342e91' %}`
