# LineSwap

Buy or sell your spot in a real-world queue.

Long lines at visa centers, clinics and public service offices waste hours. LineSwap turns a place in line into a digital ticket. Anyone can join a queue from their phone, and people who are already in line can sell their spot to someone in a hurry. Payment is in USDC on Solana, and the seller is paid the moment the ticket moves to the buyer.

> **Status: MVP prototype.** This repo contains a clickable user-experience prototype. Venues, wait times, tickets, prices and transactions are all mock data. No wallet connects and no money moves.

## Try it

Open `index.html` in any browser, or visit the GitHub Pages site once it's enabled.

1. Open a queue, for example the visa center.
2. Buy a spot from the list to jump ahead, or join the line to get your own ticket with a QR code.
3. On your ticket, set a price and list it. A mock buyer appears after a few seconds.
4. Check **Wallet** to see the balance and history update.

## How it works (planned)

- **Queue tickets:** each place in line is a ticket with a QR code that the venue scans at the door.
- **Marketplace:** people in line can list their spot at a price they choose; buyers see the position, the expected wait and the time they'd save.
- **Payments:** USDC on Solana. The ticket and the payment swap in one transaction.
- **Fee:** LineSwap keeps 5% of each sale.

## Tech

- Single static HTML file: HTML, CSS and vanilla JavaScript, no build step
- Font: Chakra Petch (Google Fonts)
- Planned: Solana program for ticket transfer and USDC escrow, wallet connection through Solana Wallet Adapter

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. The site appears at `https://<your-username>.github.io/<repo-name>/` within a minute or two.
