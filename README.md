# 🎮 StreamFlow

> The streaming platform built for everyone — especially where others don't pay.

[![Live Demo](https://img.shields.io/badge/Live-streamflow--delta.vercel.app-660033?style=for-the-badge)](https://streamflow-delta.vercel.app)
[![Next.js](https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js)](https://nextjs.org)
[![Supabase](https://img.shields.io/badge/Supabase-Database-green?style=for-the-badge&logo=supabase)](https://supabase.com)
[![Stripe](https://img.shields.io/badge/Stripe-Payments-blue?style=for-the-badge&logo=stripe)](https://stripe.com)

---

## 🌍 The Problem

Twitch and Kick do not pay creators in Kenya, Nigeria, Ghana and many other African countries. Thousands of talented streamers create content every day but cannot earn a single dollar from their work.

**StreamFlow fixes that.**

---

## ✨ What is StreamFlow?

StreamFlow is a live streaming platform that allows creators anywhere in the world to stream, build an audience and get paid — including in countries where other platforms don't support payouts.

### Key Features

- 🎥 **Live streaming** — Stream using OBS or any RTMP software
- 💬 **Real-time chat** — Live chat powered by Supabase Realtime
- 💳 **Stripe payments** — Tips and subscriptions in USD
- 📱 **M-Pesa payments** — Tips and subscriptions in KES via Intasend
- 📊 **Creator dashboard** — Track earnings, viewers and stream settings
- 🌍 **Global payouts** — Creators in Kenya, Nigeria, Ghana + 40 countries
- 📱 **Mobile responsive** — Works beautifully on all devices

---

## 💰 Revenue Model

| Payment Type | Creator | Platform |
|---|---|---|
| Tips (Stripe) | 70% | 30% |
| Tips (M-Pesa) | 70% | 30% |
| Subscriptions (Stripe $7.99/mo) | 50% | 50% |
| Subscriptions (M-Pesa KES 1,000/mo) | 50% | 50% |

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | Next.js 16, TypeScript, Tailwind CSS |
| **Backend** | Next.js API Routes |
| **Database** | Supabase (PostgreSQL) |
| **Auth** | Supabase Auth |
| **Realtime** | Supabase Realtime |
| **Video** | Mux (live streaming + VOD) |
| **Payments (USD)** | Stripe Checkout + Stripe Connect |
| **Payments (KES)** | Intasend M-Pesa STK Push |
| **Hosting** | Vercel |

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+
- A Supabase account
- A Stripe account
- An Intasend account (for M-Pesa)
- A Mux account (for video streaming)

### Installation

**1. Clone the repository**
```bash
git clone https://github.com/chris-maingi/streamflow.git
cd streamflow
```

**2. Install dependencies**
```bash
npm install
```

**3. Set up environment variables**
```bash
cp .env.example .env.local
```
Fill in your keys in `.env.local`

**4. Set up Supabase database**

Run the SQL from `supabase/schema.sql` in your Supabase SQL Editor.

**5. Run the development server**
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the app.

---

## 🗄 Database Schema
profiles        — User profiles and creator info
streams         — Stream settings and live status
chat_messages   — Real-time chat messages
subscriptions   — Active subscriber records
tips            — One-time tip payment records

## 🌐 Live Demo

Visit the live platform: **[streamflow-delta.vercel.app](https://streamflow-delta.vercel.app)**

- Sign up as a creator
- Get your stream key
- Stream using OBS
- Accept tips and subscriptions from viewers worldwide

---

## 📱 Supported Payment Methods

### Stripe (Global)
- Visa, Mastercard, American Express
- Available worldwide
- Payouts to 40+ countries

### M-Pesa (Kenya & East Africa)
- STK Push directly to viewer's phone
- Available in Kenya
- Payouts via Intasend

---

## 🗺 Roadmap

- [ ] Mux video player integration
- [ ] Stripe Connect creator payouts
- [ ] Intasend M-Pesa creator payouts
- [ ] Creator profile pages
- [ ] Expo mobile app (iOS & Android)
- [ ] Stream categories and discovery
- [ ] Clip creation from VODs
- [ ] Multi-language support (Swahili, Yoruba, Twi)

---

## 🤝 Contributing

StreamFlow is built to help African creators earn. If you want to contribute:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 👨‍💻 Built By

**Christopher Maingi** — Built for the African creator community 🇰🇪

---

## 📄 License

MIT License — free to use and modify.

---

*StreamFlow — Stream anywhere. Earn everywhere.* 🌍
