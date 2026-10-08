# MeguriPass
![MeguriPass logo](assets/logo.png)

Theme park digital stamp rally turning visits into collectible Solana NFTs.

## Overview

MeguriPass lets amusement parks and event venues run digital stamp rallies. Visitors scan QR codes at attractions to mint low-cost compressed NFT stamps on Solana. Completing a full set unlocks a token-gated fan community and real-world rewards, blending Japan's beloved stamp rally culture with Web3 collectibles.

## Problem

Traditional paper stamp rallies have no lasting value, no community connection, and limited engagement data for venues. Once the paper is thrown away, the memory and the relationship with the visitor disappear too.

## Solution

MeguriPass replaces paper stamps with cheap, instant compressed NFTs tied to QR check-ins. Each stamp becomes a persistent, ownable collectible, and completing a set unlocks a token-gated community and rewards, creating a lasting connection between venues and visitors.

## Features (MVP)

- QR code check-in at each attraction mints a compressed NFT stamp
- Progress tracker UI showing collected vs remaining stamps
- Completing full set unlocks token-gated Discord/LINE community
- Leaderboard ranking top collectors with seasonal rewards
- Simple venue dashboard to create and manage stamp campaigns

## Tech Stack

- Anchor (Solana program framework)
- Metaplex Bubblegum (compressed NFTs)
- Next.js (frontend)
- Phantom Wallet Adapter
- Supabase (backend/session/QR logic)
- QR code scanning (Web)

## How It Works

```
[Visitor] --scans QR--> [Next.js Web App]
                              |
                      verifies check-in
                              |
                        [Supabase]
                              |
                 triggers mint request
                              |
            [Anchor Program + Bubblegum]
                              |
                   compressed NFT stamp
                              |
                     [Visitor's Wallet]
```

Once all stamps in a campaign are collected, the app checks wallet holdings and grants access to a token-gated Discord or LINE community, plus any configured rewards.

## Roadmap

- Pilot with one real amusement park or local event
- Add merchandise redemption marketplace for completed sets
- Build shared multi-venue loyalty network standard

## Pitch

- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team

- Name / Role — [GitHub](#) / [Twitter](#)
- Name / Role — [GitHub](#) / [Twitter](#)
- Name / Role — [GitHub](#) / [Twitter](#)

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)


## Prototype

Live prototype: https://ainajpn.github.io/meguripass/

The source is [docs/index.html](docs/index.html) (served with GitHub Pages from the /docs folder). All data is simulated.
