# FormCraft

FormCraft is a web application that allows users to create and publish forms to collect responses from their audience. It is built using modern technologies and comes with a range of features.

## Live app

Check out the live demo of FormCraft deployed on Vercel: [FormCraft Live App](https://form-craft-eta.vercel.app/)

## Video Demo
[demo video link](https://drive.google.com/file/d/1DZTLwiW-TolOpi1El7vE7OiSWeBXj6Ty/view?usp=sharing)

![image](https://github.com/ShivamPatel-India/FormCraft/assets/70719016/6f370c5c-eb2a-450d-bbd8-66b7c770444d)

![image](https://github.com/ShivamPatel-India/FormCraft/assets/70719016/24cf3ddf-ea5a-4f50-9db8-d9e8a996bbcb)

![image](https://github.com/ShivamPatel-India/FormCraft/assets/70719016/e4953f34-0b3d-4a9a-8bb8-2fa098c35362)

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







