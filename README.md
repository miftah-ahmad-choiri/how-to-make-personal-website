# 🎓 Create an Academic Website with AcademicPages on GitHub Pages

## Table of Contents

- [🎓 Create an Academic Website with AcademicPages on GitHub Pages](#-create-an-academic-website-with-academicpages-on-github-pages)
  - [Table of Contents](#table-of-contents)
  - [📌 1. Fork the AcademicPages Repository](#-1-fork-the-academicpages-repository)
  - [📌 2. Rename the Repository](#-2-rename-the-repository)
  - [📌 3. Enable GitHub Pages](#-3-enable-github-pages)
  - [📌 4. Clone the Repository Locally](#-4-clone-the-repository-locally)
  - [📌 5. Install Jekyll Locally (Optional)](#-5-install-jekyll-locally-optional)
    - [🔹 Windows](#-windows)
    - [🔹 macOS / Linux](#-macos--linux)
    - [Run Jekyll Locally](#run-jekyll-locally)
  - [📌 6. Customize Your Site](#-6-customize-your-site)
    - [📝 Edit `_config.yml`](#-edit-_configyml)
    - [📄 Edit Pages](#-edit-pages)
    - [✏️ Adding Blog Posts](#️-adding-blog-posts)
  - [📌 7. Commit and Push Changes to GitHub](#-7-commit-and-push-changes-to-github)
  - [📌 8. Set a Custom Domain (Optional)](#-8-set-a-custom-domain-optional)
  - [🔄 Updating the AcademicPages Template](#-updating-the-academicpages-template)
  - [🎯 Troubleshooting](#-troubleshooting)
    - [❌ Website Not Showing?](#-website-not-showing)
    - [❌ Jekyll Errors Locally?](#-jekyll-errors-locally)
  - [📚 More Resources](#-more-resources)

--------------------------------------------------------------------------------
## 📌 1. Fork the AcademicPages Repository
- Go to the **[AcademicPages GitHub repository](https://github.com/academicpages/academicpages.github.io)**.
- Click **Fork** (top right corner) to create a copy in your GitHub account.

## 📌 2. Rename the Repository
- Go to **Settings** → Rename the repository to **`miftah-ahmad-choiri.github.io`** (replace `miftah-ahmad-choiri` with your GitHub username).
- This is required for GitHub Pages to host the website.

## 📌 3. Enable GitHub Pages
- Navigate to **Settings** → **Pages**.
- Under **Source**, select **main** branch and save.
- Your website will be available at **https://miftah-ahmad-choiri.github.io** in a few minutes.

## 📌 4. Clone the Repository Locally
Open a terminal or command prompt and run:

```bash
git clone https://github.com/username/username.github.io
cd username.github.io
```

## 📌 5. Install Jekyll Locally (Optional)
If you want to test the website locally before pushing changes:

### 🔹 Windows
- Install Ruby via [RubyInstaller](https://rubyinstaller.org/)
- Install Bundler and Jekyll:

```bash
gem install jekyll bundler
```

### 🔹 macOS / Linux
- Install Ruby and Jekyll:

```bash
brew install ruby
gem install jekyll bundler
```

### Run Jekyll Locally
```bash
bundle exec jekyll serve
```
Visit `http://localhost:4000` to preview.

## 📌 6. Customize Your Site
### 📝 Edit `_config.yml`
Modify `_config.yml` to change:
- **Site title, author, email, and social links**.

```yaml
title: "Your Name"
author: "Your Name"
email: "your-email@example.com"
github_username: "your-github"
linkedin_username: "your-linkedin"
```

### 📄 Edit Pages
Modify the Markdown files in the repository:
- `index.md` → Home Page
- `_pages/cv.md` → CV Page
- `_pages/publications.md` → Publications Page
- `_pages/blog.md` → Blog Page

### ✏️ Adding Blog Posts
Create Markdown files inside `_posts/`:

```markdown
---
title: "My First Blog Post"
date: 2025-02-02
author: "Your Name"
---
Welcome to my first blog post!
```

## 📌 7. Commit and Push Changes to GitHub
```bash
git add .
git commit -m "Customized AcademicPages site"
git push origin main
```

## 📌 8. Set a Custom Domain (Optional)
1. Buy a domain (e.g., from Namecheap).
2. Add a `CNAME` file in the repository with your domain name.
3. Configure **DNS records** to point to GitHub Pages.

## 🔄 Updating the AcademicPages Template
If the original **AcademicPages** repository updates, sync your fork:
```bash
git remote add upstream https://github.com/academicpages/academicpages.github.io
git fetch upstream
git merge upstream/main
git push origin main
```

---

## 🎯 Troubleshooting
### ❌ Website Not Showing?
- Check **Settings → Pages** in GitHub.
- Ensure **main branch** is selected as the source.

### ❌ Jekyll Errors Locally?
- Run `bundle install` before `bundle exec jekyll serve`.
- Ensure you have the correct Ruby and Bundler versions.

---

## 📚 More Resources
- 🔹 [AcademicPages GitHub](https://github.com/academicpages/academicpages.github.io)
- 🔹 [GitHub Pages Docs](https://docs.github.com/en/pages)
- 🔹 [Jekyll Docs](https://jekyllrb.com/)

🚀 **Enjoy your academic website!** 🎉

---

✅ Now you can **copy and paste** this directly into a Markdown file (`README.md`) or into your GitHub repository! Let me know if you need any improvements! 🚀