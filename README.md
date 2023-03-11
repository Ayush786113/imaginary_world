
# Imaginary World

This is a personal project, a content library for my stories (I am both a developer and an author :) ), I made for my resume.

This backend API serves as a platform for serving data to a frontend application. It provides endpoints for various functionalities such as reading stories and chapters from the database, writing private or public messages or subscription to newsletter.
## Documentation

It is a full stack project consisting of both frontend and backend. The frontend is very roughly created so may not be appealing. The project is open to suggestions for improvements.

The backend is created with Java Spring Boot and Appwrite. The API endpoints are currently hardcoded to return data in a specific format.
## Deployment

The project is not deployed yet because I don't have a server to host the applications - Appwrite, Plausible, Spring Boot, Sveltekit.

The repositories are linked below

- [Frontend](https://github.com/Ayush786113/imaginary_world_sveltekit_frontend/)
- [Backend](https://github.com/Ayush786113/imaginary_world_springboot_backend)
## API Reference

```
Base URL - api.domain.extension
```

#### Get all stories

```http
  GET /stories
```

#### Get single story details

```http
  GET /stories?id=${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of story to fetch |

#### Get single chapter detail

```http
  GET /chapter?id=${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of chapter to fetch |

#### Post comment

```http
  POST /connection
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- 
|
| `name`      | `string` | **Required**. name of the writer |
|
| `email`      | `string` | **Required**. email of the writer |
|
| `message`      | `string` | **Required**. message of the writer |
|
| `private`      | `boolean` | **Optional**. is private message or not **Default - false**|

#### Add subscriber

```http
  POST /subscribe
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- 
|
| `name`      | `string` | **Required**. name of the subscriber |
|
| `email`      | `string` | **Required**. email of the subscriber |

## Tech Stack

**Client:** Sveltekit, PicoCSS

**Server:** Spring Boot

**Database:** Appwrite

**Analytics:** Plausible
## Authors

Ayush
- [Github](https://www.github.com/ayush786113)
- [Instagram](https://www.instagram.com/__pole___star__)
- [Facebook](https://www.facebook.com/ayush.ghosal.3)
## Support

For support, email ayush786113@gmail.com