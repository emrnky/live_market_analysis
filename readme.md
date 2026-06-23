<div align="center">
  <img src="icon.svg" alt="PoE Market Signal icon" width="64" height="64" />

  <h1>PoE Market Signal</h1>
  <p>Machine learning driven market signals for Path of Exile 2 trading.</p>
</div>

---
<div align="center">
  <a href="http://www.poemarketsignal.com/">
    <img src="https://i.giphy.com/xS02DRItBt7aM.webp" alt="Website Link" width="500" height="300" valign="center" />
    <p>
    Visit the website
    </p>
  </a>
</div>

---

[![Support on Gumroad](https://img.shields.io/badge/Support-Buy%20me%20a%20coffee-c9a84c?style=for-the-badge)](https://emrnky.gumroad.com/)

## Overview

PoE Market Signal is a web dashboard that reads Path of Exile 2 market data and turns it into a simple call on each item: buy, sell, or hold. The goal is to help traders spot opportunities in a large, fast moving economy without manually tracking thousands of listings.

A model is trained on historical price and volume data and produces a probability distribution over the three outcomes for every tracked item. The dashboard takes the highest probability outcome and presents it as a signal, along with a confidence score so users can judge how strong that call is.

## Features

- Buy, sell, and hold signals for items across all tracked categories
- Confidence score showing how strongly the model favors its own call
- Live price, trade volume, and seven day percent change per item
- Sortable, filterable table with per signal filtering (buy / sell / hold)
- Category browser with icons, collapsible into a mobile friendly menu
- Direct links from each item to its corresponding PoE2 Wiki page
- Light and dark themes with persistent user preference
- No account or login required

## How it works

1. Market data is collected and stored in a Supabase backend.
2. A machine learning model processes recent price and volume history for each item and outputs buy / hold / sell probabilities.
3. The highest probability becomes the displayed signal; the value of that probability becomes the displayed confidence.
4. The frontend (this repository) queries Supabase directly from the browser and renders the results, refreshing on each new prediction cycle.

Tables are currently refreshed every 24 hours.

## Contributing

Issues and pull requests are welcome. If you spot incorrect signals, broken item links, or rendering bugs, please open an issue with as much detail as you can (item name, category, screenshot if relevant).

## Support

If this tool saves you time or currency, consider supporting the project:

[![Support on Gumroad](https://img.shields.io/badge/Support-Buy%20me%20a%20coffee-c9a84c?style=for-the-badge)](https://emrnky.gumroad.com/)


## Disclaimer

PoE Market Signal is an independent, community built tool. It is not affiliated with, endorsed by, or sponsored by Grinding Gear Games. Path of Exile and Path of Exile 2 are trademarks of Grinding Gear Games. All predictions and signals are generated automatically and are provided for informational purposes only; they are not financial or trading advice, and no outcome is guaranteed. Use at your own discretion.



