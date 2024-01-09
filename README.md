# FormCraft

FormCraft is a web application that allows users to create and publish forms to collect responses from their audience. It is built using modern technologies and comes with a range of features.

## Live Demo

Check out the live demo of FormCraft deployed on Vercel: [FormCraft Live Demo](https://form-craft-eta.vercel.app/)

## Technologies Used

- Next.js 13 with AppRouter
- Dnd-kit library
- ServerActions
- Typescript
- Tailwind CSS / Shadcn UI
- Vercel PostgreSQL
- Prisma as ORM

## Features

- Responsive design
- Drag and drop form designer
- Layout fields: Title, SubTitle, Spacer, Separator, Paragraph
- Form fields: Text, Number, Select, Date, Checkbox, Textarea
- Easy addition and customization of new fields
- Form preview dialog
- Share form URL
- Form submission and validation
- Form statistics: Visits and Submissions

## Local Setup

Follow these steps to set up FormCraft locally:

```bash
# 1. Install dependencies
npm install

# 2. Set up environment variables. Vercel PostgreSQL is used as database.
echo '
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=#
CLERK_SECRET_KEY=#

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

POSTGRES_PRISMA_URL=#
POSTGRES_URL_NON_POOLING=#
' > .env.local

# Replace the variable values in .env.local with your actual credentials.

# 3. Run the app
npm run dev
