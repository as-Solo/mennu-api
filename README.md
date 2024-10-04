
# MENNU-API

Este repositorio fue creado con [json-server](https://github.com/typicode/json-server) para compartir datos con la API MENNU (link mas adeánte).

Esta API proporciona datos sobre menús y platos para la aplicación de restaurante Mennu, donde se puede consultar, crear, editar y eliminar información sobre los menús y sus platos.

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
| POST        | `/dishes`                                 | {nombre, categoria, categoriaMenu,image, precio, rating}         | Creates a new dish                                             |
| GET         | `/dishes/:dishId`                         |                              | Sends all details of a dish                                    |
| GET         | `/dishes?categoria={{categoria}}`         |     {categoria}              | Dishes by Category                                             |
| GET         | `/dishes?categoriaMenu={{categoriaMenu}}` |       {categoriaMenu}        | Dishes by menuCategory                                         |
| PATCH       | `/dishes/:dishId`                         | opcional{id,nombre,image,descripcion,isGlutenFree,isVegan,categoria,categoriaMenu,precio,rating,menuId   }  | Edits a dish object                                            |
| DELETE      | `/dishes/:dishId`                         |    {dishId}                     | Deletes a dish object                                          |
| GET         | `/menus`                                  |                              | Sends all menus                                                |
| POST        | `/menus`                                  | {nombre, precio}               | Creates a new menu                                             |
| GET         | `/menus/:id`                              | {id}               | Get a menu by Id                                             |
| GET         |`menus?nombre = {{nombre}}`              | { nombre}               | Menu by name                                           |
| GET         |`menus/:menuId?_embed=dishes`              | { menuId}               | All dishes in a menu                                           |
| DELETE      | `menus/:Id`                                |                          | Deletes a menu object                                          |   

 
## Links

### Collaborators

[Alejandro S. del Solo](https://github.com/as-Solo)

[Patricia Nieto](https://github.com/PatriNieto)

### Project

[MENNU](https://github.com/as-Solo/mennu)

[MENNU-APPI](https://github.com/as-Solo/mennu-api)

[MENNU-IH](https://mennu-ih.netlify.app/)


### Slides

[Slides Link](www.your-slides-url-here.com)
