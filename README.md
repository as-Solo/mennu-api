
# MENNU-API

This repository is a [json-server](https://github.com/typicode/json-server) created to feed data into the React Application below.

#### [Mennu](https://github.com/as-Solo/mennu/tree/main)

# Server Structure

## Collections

### dishes

```javascript
{
  id,
  nombre,
  image,
  descripcion,
  isGlutenFree,
  isVegan,
  categoria,
  categoriaMenu,
  precio,
  rating,
  menuId   
}
```

### menus

```javascript
 {
   id,
   nombre,
   precio
 }
```

## Used API Endpoints in the App

| HTTP Method | URL                                       | Request Body                 | Description                                                    |
| ----------- | ---------------------------               | ---------------------------- | -------------------------------------------------------------- |
| GET         | `/dishes`                                 |                              | Sends all dishes                                               |
| POST        | `/dishes`                                 | {title, description}         | Creates a new dish                                             |
| GET         | `/dishes/:dishId`                         |                              | Sends all details of a dish                                    |
| GET         | `/dishes?categoria={{categoria}}`         |                              | Dishes by Category                                             |
| GET         | `/dishes?categoriaMenu={{categoriaMenu}}` |                              | Dishes by menuCategory                                         |
| PATCH       | `/dishes/:dishId`                         | {title, description, isFav}  | Edits a dish object                                            |
| DELETE      | `/dishes/:dishId`                         |                              | Deletes a dish object                                          |
| GET         | `/menus`                                  |                              | Sends all menus                                                |
| POST        | `/menus`                                  | {text, gameId}               | Creates a new menu                                             |
| GET         | `/menus/:id`                              | {text, gameId}               | Creates a new menu                                             |
| GET         |`menus/:menuId?_embed=dishes`              | {text, gameId}               | All dishes in a menu                                           |
| DELETE      | `/menus`                                  | {text, gameId}               | Deletes a menu object                                          |   

 
## Links

### Collaborators

[Alejandro S. del Solo](https://github.com/as-Solo)

[Patricia Nieto](https://github.com/PatriNieto)

### Project

[Repository Link Client](https://github.com/as-Solo/mennu)

[Repository Link Server](https://github.com/as-Solo/mennu-api)

[Deploy Link](https://mennu-ih.netlify.app/)


### Slides

[Slides Link](www.your-slides-url-here.com)
