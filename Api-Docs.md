# JSONPlaceholder API Reference 
> **Audience:** Developers | **Doc Type:** Step-by-Step API Guide | **Tools:** Markdown

## Overview 
This guide covers two API endpoints - GET and POST from free source JSONPlaceholder.com

## Base URL
`https://jsonplaceholder.typicode.com`

## EndPoints

1.**GET Method** (Fetches all posts)
### URL
`GET /posts`

#### Sample Response (`200 OK`)
```json
[
  {
    "userId": 1,
    "id": 1,
    "title": "Sample Post Title",
    "body": "Main text content of the blog post."
  }
]
```

### Sample Response Fields
| Field | Type | Description |
| :--- | :--- | :--- |
| `userId` | Integer | Shows which user created post. |
| `id` | Integer | shows the unique id of the post. |
| `title` | String | The title of the blog post. |
| `body` | String | The main text content of the blog post. |

2.**POST** Method (Create new post) 
`POST /posts`

### Sample Request
```bash
curl -X POST https://typicode.com \
  -H "Content-Type: application/json" \
  -d '{"title": "My First Post", "body": "Hello world!", "userId": 1}'
```

### Request Body Parameters
| Field | Type | Description |
| :--- | :--- | :--- |
| `title` | String | The title of the blog post. |
| `body` | String | The main text content of the blog post. |
| `userId` | Integer | Shows which user created post. |

### Sample Response (`201 Created`)
```json
{
  "id": 101,
  "title": "My First Post",
  "body": "Hello world!",
  "userId": 1
}
```
### Sample Response Fields
| Field | Type | Description |
| :--- | :--- | :--- |
| `userId` | Integer | Shows which user created post. |
| `id` | Integer | shows the unique id of the post. |
| `title` | String | The title of the blog post. |
| `body` | String | The main text content of the blog post. |
