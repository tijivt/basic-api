Rest Api design and implementation using lumen
---------------------------------------------------

Steps to execute the api are:-

1.Download the git directory
2.Need php 7.3 above.
3.Copy the project to a directory
4.Go to the directory and install composer
5.Create database and configure it in.env  file.
6.Start the devlopement server using php artisan serve
7.Migrate the tables using the command- php artisan migrate
8.Execute th api end points with help of any one of http client(postman,insomnia etc).
The different api end points are:-

Login
url-api/login,method-post,request parameters-email,password

Register
url-api/register,method-post,request parameters-name,email,password

Get All Articles
url-api/articles,method-get

Get One Artcle based on Id
url-api/articles/{id},method-get(id is article id)

Authorized api end points
-------------------------

Create a  New Article
url-api/articles,method-post,request parameters-name,email,password,api_token

Update an Article
url-api/articles/{id},method-put,request parameters-api_token(id is article id)

Delete an Article
url-api/articles/{id},method-delete,method-put,request parameters-api_token(id is article id)
