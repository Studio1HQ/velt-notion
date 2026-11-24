<div align="center">

<img src="https://raw.githubusercontent.com/Studio1HQ/Studio1HQ/main/assets/banners/velt-notion.webp" alt="Notion-Style Editor with Velt: A Notion-style document editor starter with Velt comments and presence" width="100%" />

<br />
<br />

# Notion-Style Editor with Velt

### A Notion-style document editor starter with Velt comments and presence

A Next.js starter for a Notion-style editor with nested documents, a Tiptap editor, cover and image uploads with EdgeStore, and Velt comments, presence and a sidebar.

<br />

[![Built by Studio1](https://img.shields.io/badge/Built_by_Studio1-f97316?style=for-the-badge&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAxNjAgMTYwIiBmaWxsPSJub25lIj48cGF0aCBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTAgMzVDMCAxNi42ODA3IDE0LjA3NDQgMS42NDg0NCAzMiAwLjEyNjk1M1YxNDFINTEuMDUyM0M1Mi40MzA4IDEzNy4zNDQgNTQuNzQ0NiAxMzMuNjg5IDU3Ljk5MzggMTMwLjAzM0M2MS4xNDQ2IDEyNi41MDggNjQuNjg5MiAxMjMuNDQgNjguNjI3NyAxMjAuODI5QzcyLjU2NjIgMTE4LjM0OSA3Ni4zNTY5IDExNi43ODIgODAgMTE2LjEyOVY4Ni43NTQ0Qzc1LjQ3MDggODcuOTI5MiA3MS4zODQ2IDg5LjY5MTkgNjcuNzQxNSA5Mi4wNDE1QzY0IDk0LjUyMjUgNjAuNzUwOCA5Ny40NiA1Ny45OTM4IDEwMC44NTRDNTYuNTM0NSAxMDIuNzIgNTUuMjU0NSAxMDQuNjU5IDU0LjE1MzkgMTA2LjY3MVYwSDEyNUMxNDQuMzMgMCAxNjAgMTUuNjY5OSAxNjAgMzVWMTI1QzE2MCAxNDQuMzMgMTQ0LjMzIDE2MCAxMjUgMTYwSDEyNFYxOEgxMDQuOTQ4QzEwMy41NjkgMjEuNjgxNiAxMDEuMjU1IDI1LjM2MjggOTguMDA2MiAyOS4wNDQ0Qzk0Ljg1NTQgMzIuNTk0MiA5MS4zMTA4IDM1LjY4NDEgODcuMzcyMyAzOC4zMTRDODMuNDMzOCA0MC44MTIgNzkuNjQzMSA0Mi4zODk2IDc2IDQzLjA0NzRWNzIuNjMwNEM4MC41MjkyIDcxLjQ0NzMgODQuNjE1NCA2OS42NzI0IDg4LjI1ODUgNjcuMzA1N0M5MiA2NC44MDc2IDk1LjI0OTIgNjEuODQ5MSA5OC4wMDYyIDU4LjQzMDdDOTkuNDY1NSA1Ni41NTEzIDEwMC43NDUgNTQuNTk4NiAxMDEuODQ2IDUyLjU3MjNWMTYwSDM1QzE1LjY3IDE2MCAwIDE0NC4zMyAwIDEyNVYzNVoiIGZpbGw9IiNmZmZmZmYiLz48L3N2Zz4K)](https://studio1hq.com)
[![Built with Velt](https://img.shields.io/badge/Built_with_Velt-141414?style=for-the-badge)](https://velt.dev)
[![Live demo](https://img.shields.io/badge/Live_demo-1c1917?style=for-the-badge&logo=vercel&logoColor=white)](https://notion-velt.vercel.app)

[Velt docs](https://docs.velt.dev) &nbsp;·&nbsp; [Velt](https://velt.dev) &nbsp;·&nbsp; [More examples](https://github.com/Studio1HQ) &nbsp;·&nbsp; [studio1hq.com](https://studio1hq.com)

</div>

<br />

## Overview

This is a minimal Notion-style editor starter built with Next.js, scaffolded in Cursor. It has a document tree, a rich text editor with a slash menu, cover images and file uploads. [Velt](https://velt.dev) adds comments, presence and a comments sidebar.

Use it as a base for collaborative, document-based apps. It is intentionally small so you can extend it.

## Features

- **Velt comments**: `VeltComments` with `@veltdev/tiptap-velt-comments` in the editor and bubble menu, plus a `VeltCommentsSidebar` and `VeltSidebarButton`.
- **Presence**: `VeltPresence` shows active users.
- **User identity**: `useIdentify` maps the signed-in user to a Velt user, and Velt dark mode follows the app theme.
- **Notion-style editor**: Tiptap and BlockNote editor components, slash commands and a bubble menu.
- **Documents**: Document list, search command, trash, publish, icon picker and cover image, kept in a persisted Zustand store.
- **File uploads**: Image dropzone using EdgeStore.
- **Light and dark mode**: Theme toggle with `next-themes`.

## Tech stack

| Layer | Tool |
| --- | --- |
| Framework | [Next.js](https://nextjs.org) (App Router), [React](https://react.dev), TypeScript |
| Collaboration | [Velt](https://velt.dev) (`@veltdev/react`, `@veltdev/tiptap-velt-comments`) |
| Editor | [Tiptap](https://tiptap.dev), [BlockNote](https://www.blocknotejs.org) |
| UI | [Tailwind CSS](https://tailwindcss.com), [shadcn/ui](https://ui.shadcn.com) |
| State | [Zustand](https://zustand-demo.pmnd.rs) |
| File uploads | [EdgeStore](https://edgestore.dev) |
| Packaging | [pnpm](https://pnpm.io) |
| Deployment | [Vercel](https://vercel.com) |

## Getting started

### Prerequisites

- Node.js 18 or later
- pnpm
- A Velt API key from the [Velt console](https://console.velt.dev)
- An EdgeStore project if you want file uploads

### Installation

```bash
git clone https://github.com/Studio1HQ/velt-notion.git
cd velt-notion
pnpm install
```

### Environment variables

Create a `.env.local` file in the project root.

| Variable | Description |
| --- | --- |
| `NEXT_PUBLIC_VELT_KEY` | Your Velt API key, passed to `VeltProvider`. |
| EdgeStore keys | Credentials for your EdgeStore project, needed for uploads through `app/api/edgestore`. See the EdgeStore docs for the variable names. |

### Run

```bash
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000). Other scripts: `pnpm build`, `pnpm start`, `pnpm lint`.

## How it works

```text
app/velt-provider.tsx        VeltWrapper: VeltProvider, user identity, VeltComments, sidebar
app/(main)/                  documents UI and routes
app/(marketing)/, (public)/  landing and public pages
app/sign-in/                 sign-in page
app/api/edgestore/           EdgeStore upload route
components/                  editor, new-editor, bubble-menu, toolbar, cover, search, modals
lib/auth.ts, auth-store.ts   mock auth stored in localStorage
lib/document-store.ts        persisted Zustand document store
```

Sign-in is a mock: any email and password creates a local user with a generated ID, and the Velt user is built from it. Replace `lib/auth.ts` with a real auth provider before production use.

## Resources

- [Live demo](https://notion-velt.vercel.app): the deployed app.
- [Velt documentation](https://docs.velt.dev): SDK guides.
- [Velt](https://velt.dev): product site.
- [EdgeStore documentation](https://edgestore.dev/docs): file uploads.

<br />

---

<div align="center">

<a href="https://studio1hq.com">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Studio1HQ/website/main/brand/studio1-logo-on-dark.svg" />
    <img src="https://raw.githubusercontent.com/Studio1HQ/website/main/brand/studio1-logo-on-light.svg" alt="Studio1" width="160" />
  </picture>
</a>

Built by **[Studio1](https://studio1hq.com)**, the technical content and DevRel partner for devtool teams. Made with [Velt](https://velt.dev).<br />
Browse more open-source examples at [github.com/Studio1HQ](https://github.com/Studio1HQ).

[![Website](https://img.shields.io/badge/studio1hq.com-0b0807?style=for-the-badge&logo=googlechrome&logoColor=white)](https://studio1hq.com)
[![Book a call](https://img.shields.io/badge/Book_a_strategy_call-f97316?style=for-the-badge&logo=googlecalendar&logoColor=white)](https://cal.com/studio1/collab)
[![X](https://img.shields.io/badge/%40Studio1HQ-141414?style=for-the-badge&logo=x&logoColor=white)](https://x.com/Studio1HQ)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0a66c2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/company/studio1hq/)

<sub><a href="https://studio1hq.com">studio1hq.com</a> · Technical content, docs, video and DevRel for devtools</sub>

</div>
