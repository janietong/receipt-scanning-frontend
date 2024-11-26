This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
# receipt-scanning-frontend
This Receipt Scanning App enables users to upload a receipt image and extracts key details including the vendor name, line items (name and price of purchased items), and the total amount. The frontend is built with **Next.js** and styled using Tailwind CSS, while the backend is powered by **Flask** and integrates **OpenAI's GPT-based API** for OCR functionality. The app is designed to process standard image formats (JPG, PNG) and provide a user-friendly JSON output of the extracted data.

To set up the project, clone the repository and install dependencies for both the frontend (`npm install`) and backend (`pip install flask flask-cors openai`). For the backend, add your OpenAI API key in a `.env` file. Start the servers with `npm run dev` for the frontend and `python main.py` for the backend. The frontend will run on `localhost:3000`, and the backend will be available on `localhost:5000`. For deployment, the frontend can be hosted on Vercel and the backend on Render, with the appropriate API keys and URLs configured.

I chose OpenAI's GPT-based API for its advanced text extraction capabilities, enabling precise formatting and accurate parsing of structured data. However, the app assumes receipts are clear, high-quality images in English, and backend performance may be impacted by large image uploads due to base64 encoding. This app is a powerful tool for automating receipt data processing while providing a seamless user experience.
