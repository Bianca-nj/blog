# Blog API 

A RESTful backend API built with Laravel for managing blog posts. This project allows users to create, read, update, and delete blog content, and is tested using Postman to simulate real-world API interactions.

##  Features

* Create blog posts
* Retrieve all posts or a single post
* Update existing posts
* Delete posts
* RESTful API structure
* Tested using Postman


##  Tech Stack

* **Backend:** Laravel (PHP)
* **Database:** MySQL
* **API Testing:** Postman


##  Installation

1. Clone the repository:

```
git clone https://github.com/Bianca-nj/blog.git
cd blog-api
```

2. Install dependencies:

```
composer install
```

3. Setup environment:

```
cp .env.example .env
```

4. Generate application key:

```
php artisan key:generate
```

5. Run migrations:

```
php artisan migrate
```

6. Start the server:
```
php artisan serve
```

##  API Endpoints

###  Get all posts

```
GET /api/posts
```

### Get a single post

```
GET /api/posts/{id}
```

### Create a post

```
POST /api/posts
```

### Update a post

```
PUT /api/posts/{id}
```

### Delete a post

```
DELETE /api/posts/{id}
```

## Example Request Body (POST/PUT)

```json id="px3w9v"
{
  "title": "My First Blog Post",
  "content": "This is the content of the blog post."
}
```

##  Testing with Postman

This API was tested using Postman:
* Send requests to the endpoints above
* Use JSON body for POST and PUT requests
* Verify responses and status codes
