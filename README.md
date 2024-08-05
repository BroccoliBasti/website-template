# Nuxt 3 Website Template
## Setup

```bash
pnpx nuxi@latest init .

pnpm install -D typescript

pnpx nuxi@latest module add @nuxtjs/tailwindcss

pnpx nuxi@0.10.4 module add shadcn-nuxt
```

## Configure nuxt.config.ts

```
// https://nuxt.com/docs/api/configuration/nuxt-config
export default defineNuxtConfig({
  compatibilityDate: '2024-04-03',
  devtools: { enabled: true },
  modules: ["@nuxtjs/tailwindcss", "shadcn-nuxt"],
  shadcn: {
    prefix: '',
    componentDir: './components/ui'
  }
})
```

## Run the CLI
```bash
pnpx shadcn-vue@0.10.4 init
```

## Add components
```bash
npx shadcn-vue@0.10.4 add <component>
```

```bash
pnpm install
```