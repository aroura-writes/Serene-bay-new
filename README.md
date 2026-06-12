# 🌊 Serene Bay — Studio Installation Manual

This setup features a public frontend portfolio journal (`index.html`) and an entirely isolated custom workspace editor (`editor.html`). 

By connecting a free cloud database tier with Supabase, your text formatting and photo updates persist globally. Anyone across the internet will immediately see what you publish from your dashboard!

---

## ☁️ Step 1: Initialize Your Free Database (Supabase)
Don't worry, there is no code involved here. It is entirely configuration via buttons.
1. Open your browser and create an account at [https://supabase.com](https://supabase.com) by choosing **Sign Up with GitHub**.
2. Inside your main panel overview, click **New Project**.
3. Set your project parameters:
   * **Name:** `serene-bay-db`
   * **Database Password:** Enter any secure password (make sure to write it down!)
   * **Region:** Select the area physically closest to you.
   * **Pricing Plan:** Select the **Free Tier** ($0/month).
4. Click **Create New Project** and allow 1-2 minutes for the cloud servers to initialize.

---

## 🗄️ Step 2: Establish the Post Structure
Your database needs to understand how to organize your titles, text, and images.
1. In the left-hand column sidebar of your Supabase page, click on the **SQL Editor** icon (it resembles a small box with terminal characters `>_`).
2. Click **New Query** at the top left of the screen.
3. Clear out any sample text and copy-paste this precise table blueprint into the code window box:

```sql
create table posts (
  id bigint generated always as identity primary key,
  title text,
  category text,
  image_url text,
  caption text,
  body_html text,
  date_string text
);

-- Turn off data lock rules so your simple dashboard can write data safely
alter table posts enable row level security;
create policy "Allow public access" on posts for select using (true);
create policy "Allow public modifications" on posts for insert with check (true);
