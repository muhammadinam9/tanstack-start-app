# 🌊 Aquarius Learning Portal

An educational learning portal for the Diagnostic Medical Sonography and MRI Technologist programs at **Aquarius Institute of Des Plaines, Illinois**, led by Dr. Tehmina Inam.

## ✨ Features

- **Dashboard** — At-a-glance stats: active students, live courses, pending grades, class average
- **Courses** — Full curriculum for DMS and MRI tracks with schedules and credit hours
- **Assignments** — Submission tracker with drag-and-drop file upload (PDF, DOCX, JPG, PNG · up to 50 MB)
- **Exams & Quizzes** — Scheduled and available assessments with status indicators
- **Study Guides** — Filterable library of PDFs, atlases, video lessons, and ARRT prep materials
- **Grades** — Class averages, trend indicators, and recent submission scores
- **Mobile-responsive** — Full navigation on all screen sizes

## 🛠️ Stack

| Layer | Technology |
|---|---|
| Framework | [TanStack Start](https://tanstack.com/start) (React 19 + file-based routing) |
| Styling | Tailwind CSS v4 with custom OKLCH design system |
| Components | shadcn/ui (Radix UI primitives) |
| Package manager | Bun |
| Deployment | Cloudflare Workers (via Wrangler) |

## 🚀 Getting Started

### Prerequisites
- [Bun](https://bun.sh) v1.0 or higher
- Node.js v18+ (for tooling)

### Local Development

```bash
# Clone the repo
git clone https://github.com/muhammadinam9/quarius-learning-portal.git
cd quarius-learning-portal

# Install dependencies
bun install

# Start dev server
bun run dev
```

Open [http://localhost:3000](http://localhost:3000).

### Build for Production

```bash
bun run build
```

### Deploy to Cloudflare

```bash
bunx wrangler deploy
```

## 📁 Project Structure

```
src/
├── routes/
│   ├── __root.tsx        # Root layout, header, footer, mobile nav
│   ├── index.tsx         # Dashboard
│   ├── courses.tsx       # Course catalog
│   ├── assignments.tsx   # Assignment list + file upload
│   ├── exams.tsx         # Exam schedule
│   ├── study-guides.tsx  # Filterable resource library
│   └── grades.tsx        # Grade tracking
├── components/ui/        # shadcn/ui primitives
├── hooks/
└── styles.css            # Tailwind + custom design tokens
```

## 🎨 Design System

Custom palette built on OKLCH for perceptual uniformity:

| Token | Value | Use |
|---|---|---|
| `--cream` | `#f5f0e8` | Background |
| `--sage` | `#dce5d4` | Secondary surfaces |
| `--teal` | `#2d8a9e` | Accent / interactive |
| `--ink` | `#0c2340` | Primary text |

Typography: **Instrument Serif** (headings) + **Work Sans** (body).

---

© 2025 Aquarius Institute of Des Plaines. All rights reserved.
