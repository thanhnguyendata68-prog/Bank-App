# Banking App - Dev Notes

## 🛠️ Setup & Configuration Log

### Step 1: Initialize Next.js Project

Initialize the application directly in the current directoty with TypeScript, Tailwind CSS, and ESLint:
```bash 
npx create-next-app@latest banking-app --typescript --tailwind --eslint

### Step 2: Initialize shadcn/ui
Configure components and styling for the project:

npx shadcn@latest init

choose Radix UI, NOVA

### Step 3: Create tailwind.config.ts
This project uses Tailwind CSS to build the user interface

### Step 4: Create types/index.d.ts
Ts: enforce strict type checking and define global types for user authentication flows, Net.js routing paramenters, and payment system integration

### Step 5 : Downlaod tailwind-merge and query-string zod

npm install clsx tailwind-merge query-string zod

UI & Utilities: Combines clsx and tailwind-merge to resolve dynamic class conflicts, along with query-string and zod for input data validation and sanitization.

### Step 6 : Create constants folder and index.ts
Contain the static constant: list of sidebar, routes, mockup test data

### Step 7 : Create api/layout.tsx
Root Application Layout (configured with Google Fonts, SEO, Metadata, and forcred dynamic SSR)

- Create page.tsx that main dashboard page (displays balance, financial charts, and recent transactions)

- Create the layout.tsx inside (root) folder in app that shared layout for main pages (includes Sidebar, Navbar, and main content)

### Step 8: Create (auth)
sign-in # User login page
sign-up # Account registration page

---------------------------------
Get error first time about 
Warning: Module not found: Can't resolve 'tailwindcss-animate'

Solve : npm install tailwindcss-animate