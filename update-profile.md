## UPDATE USER PROFILES & USER PHOTOS

To Update a user profile, create a template with a form called "/account".
Only the current user is allowed to update their profile.

#### Form Action
---
The only form action permitted for update an account is "/account"

#### Allowed Fields
---

User attributes allowed are:

* email
* name
* gender ("m" or "f")
* about (textarea)
* url
* social_twitter (twitter url)
* social_facebook (facebook url)
* social_google (google+ url)
* dob (date of birth - in any reasonable format)
* location
* is_private (boolean)
* newsletter ("1"-enabled, 0 or nil - disabled)
* hide (boolean, profile is not listed in user listings)


#### Example form
---
```
<form method="POST" action="/account">
<label>Email</label>
<input type="email" name="email" value="{{current_user.email}}" />
<label>Name</label>
<input type="text" name="name" value="{{current_user.name}}" />
...
<input type="submit" value="Update Profile" />
</form>
```

#### UPDATING USER PHOTOS
---
You need a separate form to update user templates. It should be named `"/account/photo"`. Only one field is required
attachments[]

#### Example Form
---
```<form method="POST" action"/account/photo">
  <label>Upload a new profile photo</label>
  <input type="file" name="attachments[]" />
  
  <input type="submit" value="Upload photo" />
</form>
```
