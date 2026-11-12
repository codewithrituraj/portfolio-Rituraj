# Ritu Raj Sanjay — Portfolio

Vite + React + TypeScript portfolio with Framer Motion interactions, editable project data, responsive neon UI, local Rituu assistant, and a mailto contact fallback.

## Run locally

```bash
npm install
npm run dev
```

## Build / preview

```bash
npm run build
npm run preview
```

## Deploy on Vercel

Import this repository into Vercel. Framework preset: **Vite**. Build command: `npm run build`. Output directory: `dist`.

## Configuration

- Edit all portfolio content in `src/data/projects.ts`.
- Add a real `resume.pdf` to `public/` and replace the download handler in `src/main.tsx` if you want a PDF download instead of the generated text resume.
- The contact form opens a validated `mailto:` fallback. To use Formspree or EmailJS, add your public endpoint/key via Vite env variables and replace the submit handler.
- Optional Rituu API upgrade: add `VITE_AI_API_URL` and forward questions from `src/components/Rituu.tsx` to that endpoint. Never place secret API keys in client code.
