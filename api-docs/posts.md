# Travel Agency Tribes

#### GETTING STARTED

To access the API, please send an email to support@travelagencytribes.com to request your key.

---

#### AUTHENTICATION
Every API Request must be having a parameter `apiKey` to that was obtained from TAT Support Team. Also if you are trying to return a single post, a `postkey` must be passed along with you `apikey`

---

#### Endpoints
1. Returns posts based on the entered parameters
 `/tatpostapi/v1/data`

2. Returns a single post based on the unique identifier specified. `/tatpostapi/v1/single`

---

#### Parameters
|Parameter|Type|Required|Notes|
|--|--|--|--|
|`apiKey`|String|Yes|It's used to authenticate your request and can be obtained form TAT Support.
|`page`|String|No|This is used for the pagination of posts, this is the next post id for the start of the next page of results, you will recieve this from your first successfull query..|
|`teamname`|String|No|When this is specified, the API will return posts that match your query from this team, only if you are authorized to view them.|
|`row`|String|No|This is the amount of records you want returned per row. If not specified the API will return 100 records per query|
|`postkey`|String|Yes|This is the unique identifier for a post.|
|`posttype`|String|No|This is the type of post you wish to have returned by the API. See the end of document for a list of post types. If not specified the API will return all posts of all types. Post types are mentioned below. 


#### Post Types

These are the post types that can be passed to the API.

`question, video, photo, blog, product, testimonial, offer, place, tip, user_post, lead`

---

### Request Examples

Base URL : `https://api2.gttwl.net/tatpostapi/v1/data`

#### Get All Posts

`<BASE_URL>?apikey=<API_KEY>&page=1&posttype=testimonial&row=50`


#### Get All Posts (By Team)
`<BASE_URL>?apikey=<API_KEY>&page=1&posttype=lead&teamname=My Travel Agency&row=70`


#### Get a Post (By Post Key)

`<BASE_URL>/single?apikey=""&postkey=sk4eo3l2neoir`

---

### Response Examples

#### Get All posts

```
  "status": "",
  "message": " ",
  "data":{
  "posts": [
   {
    "postkey": " ",
    "title": " ",
    "id": " ",
    "created_at": " ",
    "content": " ",
    "author_email": " ",
    "author": " ",
    "photo_attachments": [],
    "agency": " ",
    "posttype": "",
    }
    ],
    "pagination": {
    {
    last_id_on_page: "",
    next_page_id: ""
    },
    "more": " "
    "count": " "
    },
  "content_type": "json"
 }
``` 

---

#### Get a Post (By Post Key)

```{
  "status": "",
  "message":" ",
  "data":{
           "postkey": " ",
           "title": " ",
           "id": " ",
           "created_at": " ",
           "content": " ",
           "author_email": " ",
           "author": " ",
           "photo_attachments": [],
           "agency": " ",
           "posttype": " ",
          },
  "content_type": "json"
  }
```
  
