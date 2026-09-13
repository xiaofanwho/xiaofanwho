# ASTC Travel Passport Museum Map

**Live app:** [asct-map.streamlit.app](https://asct-map.streamlit.app/)

An interactive map of every US museum participating in the [ASTC Travel Passport Program](https://www.astc.org/astc-travel-passport-program/).

- Parser & QA scripts: [scripts-bank/astc](https://github.com/xiaofanwho/scripts-bank/tree/main/astc)
- Streamlit map app: [streamlit-apps/asct-map](https://github.com/xiaofanwho/streamlit-apps/tree/main/asct-map)

## What is ASTC?

The Association of Science and Technology Centers (ASTC) runs a Travel Passport Program that lets members of one participating science center or museum get free or discounted admission at hundreds of other member institutions across the US (and internationally). It's a great perk if you have a membership already — but the official directory is a long, static PDF, which makes it hard to answer simple questions like "which of these are near me?" or "which ones are near where I'm traveling next month?"

## What this is for

This project turns that PDF directory into an interactive map so a member can actually explore it: filter by state, search by name, see which locations require proof of residence, and click any museum for its address, phone number, and other details — instead of scrolling through 53 pages of small print.

## Why I made this

As a member myself, I found it genuinely inconvenient to figure out where I could actually visit. The official PDF is long and only sorted by state and museum name, with no way to see what's nearby — and cross-referencing addresses against Google Maps one by one isn't practical for hundreds of locations. Having everything geocoded and plotted on one map makes it far easier to see, at a glance, which museums are worth a visit.

## How it's built and hosted

The app is built with [Streamlit](https://streamlit.io/), a Python framework that turns a plain script into a shareable web app without writing any HTML/JS/CSS by hand. The map itself is rendered with Folium (Leaflet.js under the hood), embedded directly into the Streamlit page. Because Streamlit apps are just Python scripts, the whole thing — data loading, geocoding, filtering, and the map UI — lives in one file, and can be run locally with a single `streamlit run` command or deployed for free on Streamlit Community Cloud for anyone to use from a browser, no install required.
