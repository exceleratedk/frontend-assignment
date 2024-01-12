## Getting Started

First, run the development server:

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

## The assignment

The assignment is to create a simple web application for inputting and displaying your work experience. The application should have two pages, one for inputting the data and one for displaying it. The following fields should be included:

- Company name
- Position title
- Employment type (full-time, part-time, etc.)
- Location type (remote, on-site, etc.)
- Start date
- End date (optional)
- Industry
- Description

The application should persist the data in some capacity (i.e. the data should not be lost when the application is closed or the page is refreshed). This can be achieved by using a database, local storage, or any other method of your choosing.

The industry field should be a dropdown with a dynamic list of options. The list of options should be fetched from the Excelerate API on this endpoint `https://api.staging.excelerate.dk/industries`. The list should ideally be fetched on the server side and passed to the client. The list should be sorted alphabetically.

## This template

You should use this repository as a starting point for your solution. It's a simple [Next.js](https://nextjs.org/docs/getting-started) application bootstrapped with `create-next-app`. It includes TypeScript, [Tailwind CSS](https://tailwindcss.com/docs), and [shadcn/ui](https://ui.shadcn.com/). Additionally, it uses [React Hook Form](https://react-hook-form.com/) and [Zod](https://zod.dev/) for form validation. 

Hints:
- For creating a list of form items (e.g. the list of work experience items), you can use the `useFieldArray` hook from React Hook Form. See [here](https://react-hook-form.com/api/usefieldarray) for more information.
- You can use [React Query](https://tanstack.com/query/latest/) for fetching data from the API. See [here](https://tanstack.com/query/v4/docs/react/guides/ssr#using-nextjs) for more information about fetching server side.