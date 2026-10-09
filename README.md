
# Meesho-Clone-yaswanthinfotech

A front-end-only, multi-page e-commerce clone inspired by modern Indian marketplace UX. All shopping state (cart, wishlist, addresses, orders, theme, login) is stored in the browser's localStorage. No backend is required.

> **Disclaimer:** This is an independent educational/demo project. It is **not** the official Meesho website and does not connect to Meesho's APIs, accounts, payments, orders or databases. No real payments or orders are processed.

## Features

### Shopping
- Product search with live suggestions
- Category and subcategory navigation
- Filters: category/subcategory, minimum and maximum price, rating, minimum discount, seller
- Sorting by price, rating, discount and newest
- Product quick view, product details page and image switching
- Wishlist add/remove (persisted in localStorage) and a Favourites page
- Cart with quantity +/− controls, remove, subtotal, MRP discount, delivery and grand total
- Coupon codes: `WELCOME10`, `SAVE100`, `SHOP20`, `FIRST50`

### Checkout and orders
- Saved addresses with selection and deletion
- Checkout summary with UPI, card and Cash on Delivery options
- Demo order placement, orders list and order tracking
- Navigation guards that redirect checkout/payment to the cart when it is empty

### Account
- Login, signup and OTP demo flow (demo OTP: `123456`)
- Profile page and seller onboarding pages

### Home page showcase
- Deals of the day, category promos and trending products
- "Original Brands" logo marquee (pauses on hover)
- Beauty, home & kitchen and trust sections

### UI and motion
- Light/dark theme toggle (saved locally)
- Responsive layout with mobile navigation
- Page entrance, scroll progress, hover effects, animated banners and an animated announcement ticker
- Reduced-motion support via `prefers-reduced-motion`

## Pages

Home, products, categories, search, product details, cart, wishlist, checkout, payment, order success, orders, track order, profile, address, login, signup, OTP, notifications, offers, seller, create seller, help, contact, returns, privacy, terms, about and 404.

## Tech stack

- HTML5, CSS3, JavaScript (vanilla)
- [Bootstrap 5.3](https://getbootstrap.com/) and [Bootstrap Icons](https://icons.getbootstrap.com/) via CDN
- localStorage for demo cart, wishlist, theme, auth and order state
- Product catalogue of 180 items in `data/products.js`

## Project structure

```
MEESHO_V_3.0/
├── index.html            # Home page
├── products.html         # Full catalogue
├── product-details.html  # Single product page
├── cart.html, checkout.html, payment.html, order-success.html
├── *.html                # Other pages (login, orders, seller, help, ...)
├── css/                  # Stylesheets (style, responsive, motion, enhancements)
├── js/                   # Page logic (app, cart, checkout, search, auth, ...)
├── data/products.js      # Product catalogue
└── assets/               # Logos, brand images, product images, banners
```

## Getting started

No build step is needed.

1. Clone or download this repository.
2. Open `index.html` in a modern browser.

An internet connection is needed only for the CDN-hosted Bootstrap and icon files and for remote demo images.

## Notes

- Clearing browser site data resets the demo cart, wishlist, orders and login.
- Coupon codes and the OTP are fixed demo values.
