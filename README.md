# 📰 WackyFlip-Newsfeed

**Dynamic News & Announcement System for Wacky Flip**

`WackyFlip-Newsfeed` powers the **real-time news cards**, **tournament announcements**, and **featured updates** displayed across [wackyflip.com](https://wackyflip.com) and in-game home screens. Designed for speed and flexibility, it ensures players always see the latest events, patch notes, and promotions.

---

## 🎯 Features

| Feature                 | Description                                                          |
| ----------------------- | -------------------------------------------------------------------- |
| 📰 Dynamic News Cards   | Serve rich, clickable update tiles with images, titles, and links    |
| 🏆 Tournament Alerts    | Automatically push event schedules, results, and live status         |
| 📅 Scheduled Publishing | Schedule announcements ahead of time                                 |
| 🔄 Auto-Refresh         | Fetches new updates without page reloads                             |
| 🌍 Localization Support | Multi-language content based on `WackyFlip-Locale`                   |
| 📲 Responsive Layout    | Optimized for desktop, mobile, and in-game views                     |
| 🔗 Deep Linking         | Send users directly to tournaments, blog posts, or store pages       |
| 🔔 Optional Push Link   | Integrates with `WackyFlip-Push` to notify players of important news |

---

## 🛠 Tech Stack

* **Frontend:** React + TailwindCSS / Next.js
* **Backend API:** Node.js + Express / Serverless Functions
* **Database:** MongoDB / PostgreSQL (content storage & scheduling)
* **CDN:** WackyFlip-CDN for hosting images and media assets
* **Integrations:** `WackyFlip-CMS`, `WackyFlip-Locale`, `WackyFlip-Tournaments`

---

## 📁 Repository Structure

```
WackyFlip-Newsfeed/
├── components/
│   ├── NewsCard.tsx
│   ├── TournamentAnnouncement.tsx
│   ├── FeaturedUpdate.tsx
│   └── NewsTicker.tsx
├── pages/
│   └── api/
│       ├── get-latest-news.ts
│       └── schedule-news.ts
├── utils/
│   └── fetchNews.ts
├── styles/
└── README.md
```

---

## 🚀 Getting Started

1. Clone the repository:

```bash
git clone https://github.com/wackyflipgame/WackyFlip-Newsfeed.git
cd WackyFlip-Newsfeed
npm install
```

2. Set environment variables in `.env.local`:

```
NEWSFEED_DB_URI=your-database-uri
CDN_BASE_URL=https://cdn.wackyflip.com
```

3. Run the dev server:

```bash
npm run dev
```

4. Example usage:

```tsx
import NewsFeed from '@/components/NewsFeed';

<NewsFeed limit={5} filter="tournaments" />
```

---

## 📬 Contribution Guidelines

* Keep news content **short and engaging** for quick scanning
* Always provide **alt text** for images for accessibility
* Tag updates correctly for filtering (`tournament`, `patch`, `promo`, etc.)
* Use scheduled publishing for **time-sensitive announcements**

---

## 🔗 Related Repositories

* [`WackyFlip-Blog`](https://github.com/wackyflipgame/WackyFlip-Blog) – Full-length articles, patch notes, and dev diaries
* [`WackyFlip-Tournaments`](https://github.com/wackyflipgame/WackyFlip-Tournaments) – Backend for competitive events
* [`WackyFlip-Push`](https://github.com/wackyflipgame/WackyFlip-Push) – Push notifications for news alerts

---

## 📜 License

MIT © 2025 Wacky Flip Studios
