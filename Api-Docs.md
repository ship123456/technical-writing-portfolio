# JSONPlaceholder API Reference 

## Overview 
This guide covers  two API end points - GET and POST from free source JSONPlaceholder.com

## Base URL
`https://jsonplaceholder.typicode.com`

## End Points

1.GET Method (Fetches all posts)
### URL
`GET /posts`

### Sample Request
`curl -X GET https://typicode.com`

### Sample Response( 200 - success) 


| Field | Type | Description |
| :--- | :--- | :--- |
| `userId` | Integer | Shows which user created post. |
| `id` | Integer | shows the unique id of the post. |
| `title` | String | The title of the blog post. |
| `body` | String | The main text content of the blog post. |

2.POST Method (Create new post) 
`POST /posts`


