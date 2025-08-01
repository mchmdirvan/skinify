# Skinify

[Skinify](https://skinify.mchmdirvan.com) online store for mobile phone skin products.

## Links

- Frontend Web: <https://skinify.mchmdirvan.com>
- Backend API: <https://skinify-api.mchmdirvan.com>

Repositories:

- General: <https://github.com/mchmdirvan/skinify>
- Backend API: <https://github.com/mchmdirvan/skinify-api>
- Frontend Web: <https://github.com/mchmdirvan/skinify-web>

Inspirations:

- <https://exacoat.com>

## Features

- Home page
  - Hero section
  - Products catalogue
  - Example: <https://exacoat.com>
- Product page
  - Image
  - Name
  - Brand
  - Price
  - Add to cart form: quantity input & add to cart button
- Shopping cart page
  - Product items to buy
    - Image, name, price, quantity, total (price x quantity)
    - Remove item
  - Link: continue shopping, go to products catalogue
  - Link: checkout
- Checkout page
  - Order summary
    - Product items to buy
    - Grand total of all product items to buy
- Place order / transaction is being processed

## UI Designs

- Figma:

### Home Page

<img alt="Home Page" src="./designs/home.jpg" width="400" />

## Entity Relationship Diagram (ERD)

![ERD](./diagrams/erd.svg)

## REST API Endpoints

- Production: `https://skinify.mchmdirvan.com`
- Local: `http://localhost:3000`

| Endpoint         | HTTP     | Description               |
| ---------------- | -------- | ------------------------- |
| `/products`      | `GET`    | Get all products          |
| `/products/:id`  | `GET`    | Get product by id         |
| `/products/seed` | `POST`   | Seed all initial products |
| `/products`      | `POST`   | Add new product           |
| `/products`      | `DELETE` | Delete all products       |
| `/products/:id`  | `DELETE` | Delete product by id      |
| `/products/:id`  | `PUT`    | Update product by id      |

### Product

```json
{
  "id": "uuid",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
```

### Add New Product

````json
{
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
Request Body:

```json
{
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
````

Response Body:

```json
{
  "id": "abc123",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
```
