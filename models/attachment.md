#### Attachments (Files, Photos, Videos)

```
{{id}}
{{permalink}}
{{title}}
{{url}}
{{width}}
{{height}}
{{html}}
{{author_name}}
{{author_url}}
{{provider_name}}
{{provider_url}}
{{created_at}}
{{updated_at}}
{{type}}
{{25x25}}
{{50x50}}
{{100x100}}
{{270x360}}
{{640x480}}
{{135x135}}
{{original}}
{{1024x768}}
```

#### RESIZING IMAGES
---

You can resize images to any size like this:

`<img src="/api/resize/{{id}}?size=640x480" />`

`{{id}}` is the id of the photo in question

Want to view the image in your browser first?

Just put the URL in your browser:
`http://sitename.com/api/resize/55?size=640x480&debug=1`

#### IMAGE RESIZING GEOMETRY
---

Sizes are represented in width x height, example: 200x150. When the width and hight is the same you will get a perfectly square image that is resized and cropped to prevent stretching. When the width and height is different, the image will be sized to the maximum width and the hight will be naturally scaled. We will add other resize options soon!


#### NOTES ON IMAGE RESIZING
---

This system resizes and caches the image, so it becomes available in other places. However the first resize operation can be slow (up to a second or two).
