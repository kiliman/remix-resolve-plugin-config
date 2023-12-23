# Welcome to Remix + Vite!

The Remix Vite plugin calls `resolvePluginConfig` multiple times per request.

This can be problematic if you're using a custom `routes` config with big route
trees.

## Repro

To reproduce, just clone repo and `npm run dev`. You'll see it output `routes`
multiple times when you load the home page.
