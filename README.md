# e-plantShopping — Paradise Nursery

A shopping cart application for an online plant shop, built with React, Redux Toolkit and Vite.

## Features

- **Landing page** with a "Get Started" button that opens the product listing.
- **Navigation bar** with links to the landing page, the plants listing and the shopping cart, plus a live cart-quantity badge.
- **Product listing** grouped into three categories (Air Purifying, Aromatic Fragrant and Insect Repellent plants). Each card shows an image, name, description, price and an **Add to Cart** button (disabled once the plant is in the cart).
- **Shopping cart** showing a card per plant with thumbnail, unit price, subtotal, **+ / −** quantity buttons and **Delete**, plus the total cart amount.
- **Continue Shopping** and **Checkout** buttons (Checkout shows a "Coming Soon" message).

## Tech and concepts

- React function components, props and composition
- `useState` for toggling the landing page, product list and cart views
- Redux Toolkit (`CartSlice.jsx`) with `addItem`, `removeItem` and `updateQuantity` actions; `useSelector` / `useDispatch` in the components

## Project structure

```
src/
  App.jsx          Landing page and view switching
  App.css          Styles
  AboutUs.jsx      About section on the landing page
  ProductList.jsx  Navbar, plant categories and product cards
  CartItem.jsx     Cart page
  CartSlice.jsx    Redux slice for the cart
  store.js         Redux store
  main.jsx         Entry point
```

## Run locally

```bash
npm install
npm run dev
```

Build for production with `npm run build` (output in `dist/`).
