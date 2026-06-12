# 🌊 Serene Bay — Setup & Deployment Guide

Welcome to **Serene Bay**, your clean, elegant ocean photography and personal literary journal. This project has a built-in interactive visual content editor (WYSIWYG CMS). You can update your photography links, text formats, and titles live on your website inside your web browser. 

Follow this manual step-by-step to get your website up on the internet completely free using GitHub and Vercel.

---

## 🛠️ Step 1: Create a Free GitHub Account
GitHub is an online hosting system that holds your code files securely.
1. Open your web browser and go to [https://github.com](https://github.com).
2. Click **Sign up** in the top-right corner.
3. Fill out your email, establish a secure password, choose a unique username, and complete the verification step.

---

## 📁 Step 2: Upload Your Website Files to GitHub
You don't need any special developer software to upload your files; you can do it right inside your web browser.
1. Once logged into GitHub, look at the top right of the page and click the **`+` (Plus)** icon, then select **New repository**.
2. Set up your repository with these exact configurations:
   * **Repository name:** Type `serene-bay`
   * **Public/Private:** Select **Public**
   * Leave everything else unchecked/as-is.
3. Scroll to the bottom and click the green **Create repository** button.
4. You will see a setup screen. Look for the link that says: **"uploading an existing file"**. Click it.
5. Open your local computer file folder where you saved `index.html` and `README.md`. 
6. Drag both files directly into your web browser box to load them.
7. Scroll down to the bottom of the page and click the green **Commit changes** button. Your files are now safely stored online!

---

## 🚀 Step 3: Publish Live to Vercel
Vercel turns your code files on GitHub into a live web address accessible by anyone across the world.
1. Open a new browser tab and navigate to [https://vercel.com](https://vercel.com).
2. Click **Sign Up** in the upper-right corner.
3. Select **Continue with GitHub**. A pop-up box will appear asking to authorize Vercel; click **Authorize Vercel**.
4. Once you are inside your new dashboard, click the blue button labeled **Add New...** and select **Project**.
5. You will see a section titled *"Import Git Repository"*. Find your `serene-bay` project repository in that list and click the **Import** button right next to it.
6. A configurations page will load. **Do not change any settings here**. The default options are perfectly set up for this project.
7. Click the **Deploy** button.
8. Wait roughly 30 seconds while Vercel compiles the web assets. Once done, confetti will hit the screen, and you will see a preview thumbnail layout of your site!

---

## 📝 Step 4: Access and Manage Your Content
1. Click on the image thumbnail display inside Vercel to launch your new web page address (e.g., `https://serene-bay.vercel.app`).
2. Click the dark button labeled **Open CMS Panel** in the top right header navigation bar.
3. Modify the article title text, change the image address placeholder link (using high-quality images from sites like Unsplash), alter the categories, and use the visual editor text block to type or format your deep reflections.
4. Click **Apply and Save Changes**. The site updates instantly without changing code!

*Note: This sleek template uses `localStorage` architecture, keeping your written words saved directly within your browser profile cache.*
