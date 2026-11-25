# Class 10 Notes — Setup Guide

This is a free-to-start website template. Students can browse and download PDFs without accounts. Only the admin signs in to upload PDFs.

## What you need
- A Supabase account/project (free tier, subject to current plan limits)
- A GitHub account for free static hosting with GitHub Pages

## A. Set up the database and file storage
1. Create a project at https://supabase.com.
2. In **Authentication → Users**, create your admin user with your email and a strong password.
3. Open that user and copy the **User UID**.
4. In `setup.sql`, replace every `ADMIN_USER_UUID` with that UID.
5. Open **SQL Editor**, paste the edited `setup.sql`, and run it.
6. In **Project Settings → API**, copy the Project URL and the `anon` / publishable key.
7. In `index.html`, replace:
   - `YOUR_SUPABASE_PROJECT_URL`
   - `YOUR_SUPABASE_ANON_KEY`
   with your own values.

Do not put a `service_role` or secret key in the website.

## B. Publish the website free
1. Create a GitHub repository named `class10-notes`.
2. Upload `index.html` to the repository root.
3. Open **Settings → Pages**.
4. Under Build and deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then Save.
5. GitHub will show the public website address after deployment.

## C. Use it
- Open your public website address. Students can read and download published PDFs without signing up.
- Click **Admin Login**, sign in using the admin email/password, then upload a PDF.
- PDFs are limited to 20 MB in this starter page. Supabase plan limits and terms may change; check your dashboard before uploading lots of files.

## Important
- Keep your admin password private. Do not share it with students.
- Anyone can view/download the notes, as requested.
- This starter has no custom domain and no automatic backup.
- Only upload notes you created or have permission to distribute.
- If you publish publicly, avoid adding personal phone numbers, home addresses, student records, or private information.
