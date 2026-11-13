# Pre-Trade Checklist

A simple web checklist to run through every time I open the charts. **No box, no trade.**

**Live site:** https://pre-trade-hazel.vercel.app

## What it does

The page walks through my trading flow top-down. Each step stays locked until the one before it is complete, so I can't skip ahead.

1. **Direction (Daily / 4H):** pick bullish, bearish, or ranging. Confirm the Daily trend and that the 4H agrees. Ranging means no trade.
2. **4H zone:** a demand or supply zone in my bias direction, with imbalance (FVG) or liquidity, that price has respected. A breaker block in my bias direction also counts.
3. **Lower timeframe:** an LTF demand/supply zone with imbalance and/or liquidity, price testing it, and a CISD confirmation.
4. **My rules:** entry timeframe, whether CISD is required or optional, where the stop goes, and a written invalidation.

When every step is complete, the bottom bar turns green and shows **BUY** or **SELL setup valid**. Then I can log the trade, which resets the board for the next setup.

## Features

- Locking steps that enforce the order of the checklist
- Progress bar and clear go/no-go verdict
- Counters for valid setups logged and resets without trading
- Light and dark themes
- Works on desktop and mobile
- Progress saves in the browser (localStorage), so nothing is lost on refresh

## Tech

A single static `index.html` file with plain HTML, CSS and JavaScript. No build step and no dependencies, apart from the Baloo 2 font from Google Fonts.

## Run it locally

Download or clone the repo and open `index.html` in a browser.

## Deploy

Hosted on [Vercel](https://vercel.com) as a static site. Pushing to `main` redeploys automatically.

## Design

Retro desktop-window style: thick black borders, grey title bars, hard offset shadows, and a dotted halftone background.

## Disclaimer

This is a personal discipline tool, not financial advice.
