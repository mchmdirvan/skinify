# Skinify

[Skinify](https://skinify.mchmdirvan.com) - Online store for premium mobile phone skin products.

## 🔗 Links

**Links:**

- Frontend: <https://skinify.mchmdirvan.com>
- Backend API: <https://skinify-api.mchmdirvan.com>

**Repositories:**

- Main: <https://github.com/mchmdirvan/skinify>
- Backend API: <https://github.com/mchmdirvan/skinify-api>
- Frontend Web: <https://github.com/mchmdirvan/skinify-web>

**Inspiration:**

- <https://exacoat.com>

## ✨ Features

### Core Pages

- **Home Page**
  - Hero section with featured products
  - Product catalogue with search/filter
  - Brand showcase
- **Product Details**
  - High-quality product images
  - Product specifications (name, brand, price)
  - Add to cart functionality with quantity selector
- **Shopping Cart**
  - Item management (view, update quantity, remove)
  - Price calculations and totals
  - Continue shopping or proceed to checkout
- **Checkout**
  - Order summary with itemized list
  - Grand total calculation
  - Order processing workflow

## 🎨 UI Designs

**Figma Design:**

### Home Page

<img alt="Home Page Design" src="./designs/home.jpg" width="400" />

## 📊 Database Schema

![Entity Relationship Diagram](./diagrams/erd.svg)

## 🚀 API Documentation

**Base URLs:**

- Production: `https://skinify-api.mchmdirvan.com`
- Development: `http://localhost:3000`

### Endpoints

| Endpoint         | Method   | Description           |
| ---------------- | -------- | --------------------- |
| `/products`      | `GET`    | Get all products      |
| `/products/:id`  | `GET`    | Get product by id     |
| `/products/seed` | `POST`   | Seed initial products |
| `/products`      | `POST`   | Create new product    |
| `/products/:id`  | `PUT`    | Update product by id  |
| `/products/:id`  | `DELETE` | Delete product by id  |
| `/products`      | `DELETE` | Delete all products   |

### Data Models

**Product Schema:**

```json
{
  "id": "uuid",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
```

**Create Product Request:**

```json
{
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
```

**Create Product Response:**

```json
{
  "id": "abc123",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "price": 120000,
  "brand": "Apple"
}
```

## 🛠️ Tech Stack

- **Frontend:** [Add your frontend technology]
- **Backend:** [Add your backend technology]
- **Database:** [Add your database]
- **Deployment:** [Add deployment platform]
