# Storify

Storify is a **Cloud Storage Web App** built with [Next.js](https://nextjs.org). It allows users to upload, organize, and share their files seamlessly. The application supports a variety of file types, includes real-time search functionality, and provides a modern, user-friendly interface. Built with scalability and responsiveness in mind, Storify ensures a smooth user experience across devices.

## Features

- **File Upload**: Drag-and-drop or browse files for upload.
- **Real-Time Search**: Quickly find files using a search bar with debounced queries.
- **File Organization**: Categorize files into `Documents`, `Images`, `Media`, and `Others`.
- **Sharing**: Share files with other users via email.
- **Responsive Design**: Optimized for both desktop and mobile devices.
- **Built-in Authentication**: Manage user accounts and permissions securely.
- **Dynamic Sorting and Filtering**: Organize files by type, date, or custom queries.
- **Usage Analytics**: See available storage space and file usage stats.

---

## Getting Started

Follow these steps to get the development server up and running:

### Prerequisites
- Node.js 18.x or higher
- npm, yarn, or pnpm installed globally

### Installation
1. Clone the repository:
   ```bash
   git clone git@github.com:Suenkuen/storify.git
   cd storify
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser to view the app.

---

## Configuration

To connect Storify to your database and cloud storage backend, set up the required environment variables in a `.env.local` file:

```env
NEXT_PUBLIC_APPWRITE_ENDPOINT: The base URL for your Appwrite cloud instance.
NEXT_PUBLIC_APPWRITE_PROJECT: The unique ID of your Appwrite project.
NEXT_PUBLIC_APPWRITE_DATABASE: The ID of your Appwrite database.
NEXT_PUBLIC_APPWRITE_USERS_COLLECTION: The ID of the users' collection in your database.
NEXT_PUBLIC_APPWRITE_FILES_COLLECTION: The ID of the files' collection in your database.
NEXT_PUBLIC_APPWRITE_BUCKET: The storage bucket ID for uploaded files.
NEXT_APPWRITE_KEY: The API key to authenticate server-side requests.
```

Replace placeholders with your backend configuration.

---

## Learn More

- [Next.js Documentation](https://nextjs.org/docs) - Learn more about the framework powering this app.
- [Appwrite Documentation](https://appwrite.io/docs) - Understand the backend architecture.

---

## Deploy on Vercel

You can easily deploy Storify on [Vercel](https://vercel.com). Follow the deployment documentation for more details:

- [Vercel Deployment Guide](https://nextjs.org/docs/app/building-your-application/deploying)
