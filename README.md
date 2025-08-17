# Skinify

[Skinify](https://skinify.mchmdirvan.com) - Online store for premium mobile phone skin products.

## 🔗 Links

**Links:**

- Frontend: <https://skinifyy.vercel.app>
- Backend API: <https://skinify-api.onrender.com>

**Repositories:**

- Main: <https://github.com/mchmdirvan/skinify>
- Backend API: <https://github.com/mchmdirvan/skinify-api>
- Frontend Web: <https://github.com/mchmdirvan/skinify-web>

**Inspiration:**

- <https://exacoat.com>

## 🛠️ Architecture & Tech Stack

### Client | Presentation Layer (UI)

- HTML
- CSS
  - Tailwind CSS
  - shadcn/ui
- JavaScript
- TypeScript
- React
- React Router
- Docker

### Server | Application Layer (Business Logic)

- JavaScript
- TypeScript
- Hono
- OpenAPI
- Zod
- Docker

### Data Access Layer (Database)

- Prisma
- PostgreSQL
- Docker

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

![Entity Relationship Diagram](/assets/erd.png)

## 🚀 API Documentation

- Production: `https://skinify-api.mchmdirvan.com`
- Development: `http://localhost:3000`

### REST API Endpoints

| Endpoint        | Method   | Description          |
| --------------- | -------- | -------------------- |
| `/products`     | `GET`    | Get all products     |
| `/products/:id` | `GET`    | Get product by id    |
| `/products`     | `POST`   | Create new product   |
| `/products/:id` | `PUT`    | Update product by id |
| `/products/:id` | `DELETE` | Delete product by id |

### Data Models

**Product Schema:**

```json
{
  "id": "uuid",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "sku": "SKINIFY-IP16P-MTBK-1",
  "brand": "Apple",
  "description": "Skin premium untuk iPhone 15 dengan finishing Matte Black yang elegan. Melindungi dari goresan tanpa menambah ketebalan.",
  "imageUrl": "https://placehold.co/600x600/222/FFF/png?text=Matte+Black",
  "price": 120000,
  "stockQuantity": 100,
  "createdAt": "2023-10-01T12:00:00Z",
  "updatedAt": "2023-10-01T12:00:00Z"
}
```

**Create Product Request:**

```json
{
  "name": "iPhone 15 Matte Black",
  "sku": "SKINIFY-IP16P-MTBK-1",
  "brand": "Apple",
  "description": "Skin premium untuk iPhone 15 dengan finishing Matte Black yang elegan. Melindungi dari goresan tanpa menambah ketebalan.",
  "imageUrl": "https://placehold.co/600x600/222/FFF/png?text=Matte+Black",
  "price": 120000,
  "stockQuantity": 100
}
```

**Create Product Response:**

```json
{
  "id": "uuid",
  "slug": "iphone-15-matte-black",
  "name": "iPhone 15 Matte Black",
  "sku": "SKINIFY-IP16P-MTBK-1",
  "brand": "Apple",
  "description": "Skin premium untuk iPhone 15 dengan finishing Matte Black yang elegan. Melindungi dari goresan tanpa menambah ketebalan.",
  "imageUrl": "https://placehold.co/600x600/222/FFF/png?text=Matte+Black",
  "price": 120000,
  "stockQuantity": 100,
  "createdAt": "2023-10-01T12:00:00Z",
  "updatedAt": "2023-10-01T12:00:00Z"
}
```
