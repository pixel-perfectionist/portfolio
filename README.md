# you-need-a-dev-like.me

Source for [you-need-a-dev-like.me](https://you-need-a-dev-like.me), the portfolio of Alexander Katrukhin, UX Engineer.

Built with [Svelte](https://svelte.dev), [Vite](https://vitejs.dev) and [Tailwind CSS](https://tailwindcss.com). Deployed to GitHub Pages.

## Run locally

```bash
yarn
yarn dev
```

## Scripts

| Command        | Description                                                        |
| -------------- | ------------------------------------------------------------------ |
| `yarn dev`     | Start the Vite dev server                                          |
| `yarn build`   | Build to `dist/`                                                   |
| `yarn github`  | Production build with the `you-need-a-dev-like.me` base URL        |
| `yarn preview` | Serve the built site locally                                       |
| `yarn format`  | Format the code with Prettier                                      |

## Deployment

Every push to `main` runs [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml). It builds the site with `yarn github` and publishes `dist/` to the `gh-pages` branch.

## Structure

- `src/routes/`: page components (`Portfolio`, `About`)
- `src/lib/`: shared components (header, cards, modal, Vimeo player)
- `src/assets/`: images and the contact card
