# 🍽️ Crave — Food Ordering Web App

**Crave** is a full-featured food ordering platform (inspired by Swiggy/Zomato) built with pure **HTML, CSS & JavaScript** — no frameworks, no build tools, no backend required. All data is persisted in the browser via `localStorage`.

---

## 🚀 Getting Started

### Prerequisites
- Any modern browser (Chrome, Edge, Firefox)
- No installation, dependencies, or server needed!

### Run the project
Just open the entry file in your browser:

```
landing.html   ← Start here (portal chooser)
```

Or serve it locally for a cleaner experience:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000/landing.html`

---

## 🔑 Demo Accounts

| Portal | Email | Password |
|---|---|---|
| **Admin** | `admin@crave.com` | `admin123` |
| **Restaurant Partner** | `rest@crave.com` | `rest123` |
| **Customer** | Sign up via the Sign Up tab | — |

> Each login screen has a **⚡ One-Click Login** button for quick demo access.

---

## 📁 Project Structure

| File | Description |
|---|---|
| `landing.html` | Landing page — choose your portal |
| `index.html` | Main app — customer ordering + **Admin Dashboard** |
| `index1.html` | **Restaurant Partner Panel** — menu & order management |
| `index2.html` | Lightweight **Quick Food Ordering** portal |
| `README.md` | This file |

---

## ✨ Features

### 🛒 Customer Portal
- 🔍 **Smart search** — restaurants, cuisines & dishes with typo-friendly aliases (e.g. "piza" → 🍕)
- 🏷️ **Category filters** — Breakfast, Biryani, Desserts, Fitness, Party Packs & more
- 🥗 **Veg-only toggle** & sorting (rating, delivery time, price)
- 🎉 **Offers & deals** on restaurant cards
- ❤️ **Favorites** & ⭐ ratings
- 🧾 **Cart** with quantity steppers and itemized bill (delivery fee, GST, savings)
- 📦 **Order history** with one-click **Reorder**
- 📄 Info pages — About, Terms, Privacy, Help Centre, etc.

### 🏪 Restaurant Partner Panel (`index1.html`)
- 📊 Dashboard with stats — orders, revenue, active orders, menu size
- 📦 **Order management** — status flow: `New → Preparing → Ready → Out for delivery → Delivered / Cancelled`
- 🍽️ **Menu editor** — add/edit/delete items, veg/non-veg markers, availability toggle
- ⚙️ **Restaurant profile** editing
- 📈 **Analytics** — 7-day revenue chart & item performance

### 🛡️ Admin Dashboard
- 📊 KPI overview — total orders, revenue, users, restaurants
- 📦 Order management with live status updates
- 🏪 **Add / edit / delete restaurants** (with inline menu editing)
- 👥 Registered users list

### 🧑‍💼 Auth
- Sign up / sign in for customers, restaurants, and admin
- Separate session keys per portal (`crave_session`, `crave_session_restaurant`)
- Form validation with friendly error messages

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript (ES5-compatible) |
| Fonts | Google Fonts — **Inter** |
| Icons | Emoji (zero asset dependencies) |
| Data | `localStorage` (users, sessions, restaurants, menus, orders) |
| Hosting | Static — GitHub Pages / Netlify / Vercel ready |

---

## 🗄️ Data & Storage Keys

| Key | Purpose |
|---|---|
| `crave_users` | Registered accounts (customer, restaurant, admin) |
| `crave_session` / `crave_session_restaurant` | Active sessions |
| `crave_restaurants` | Restaurant catalog |
| `crave_menus` | Per-restaurant menu items |
| `crave_orders` | All orders (shared between portals) |
| `crave_history` | Per-user order history |

> Data is seeded automatically on first load. **Clear your browser's localStorage** (or use DevTools → Application → Local Storage → Clear) to reset the demo.

---

## 📱 Responsive Design

Fully responsive across desktop, tablet, and mobile:
- Sticky headers & filter bars
- Collapsible sidebar (partner panel) on mobile
- Horizontal-scrolling category rails
- Mobile-friendly tables & modals

---

## 🖼️ Screenshots

> Add screenshots of the landing page, customer portal, partner panel, and admin dashboard here:
> ```markdown
> ![Landing](screenshots/landing.png)
> ![Customer Portal](screenshots/customer.png)
> ```

---

## 📌 Roadmap

- [ ] Real backend (Node/Express or Firebase)
- [ ] Payment gateway integration
- [ ] Live delivery tracking
- [ ] Reviews & ratings
- [ ] Dark mode

---

## 🤝 Contributing

1. Fork the repo
2. Create a branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m "Add amazing feature"`)
4. Push (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is for **educational purposes** (SDC Project Review Demo).

---

<p align="center">Made with 🧡 in India</p>
