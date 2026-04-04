# GitHub Pages Deployment Guide

## Option 1: Using GitHub Web Interface (Easiest)

### Steps:
1. **Go to GitHub**: https://github.com
2. **Create New Repository**: 
   - Name: `nirvana-proposal`
   - Public repository
   - Initialize with README (optional)

3. **Upload Files**:
   - Click "Add file" → "Upload files"
   - Drag and drop all files from this folder:
     - `index.html`
     - `Nirvana_SR_Proposal_v4.0_Bilingual_MOST_BEAUTIFUL.pdf`
     - `README.md`
     - `.gitignore`

4. **Enable GitHub Pages**:
   - Go to Repository Settings
   - Scroll to "GitHub Pages" section
   - Source: select `main` branch
   - Folder: `/ (root)`
   - Save

5. **Get Your Link**:
   - Wait 1-2 minutes
   - Your site will be at: `https://[your-username].github.io/nirvana-proposal/`

## Option 2: Using GitHub CLI (Fastest if you have CLI)

### Steps:
```bash
# 1. Login to GitHub CLI
gh auth login

# 2. Create repository
gh repo create nirvana-proposal --public

# 3. Navigate to project folder
cd /path/to/nirvana-proposal

# 4. Initialize git and push
git init
git add .
git commit -m "Add Nirvana SR Proposal v4.0"
git branch -M main
git remote add origin https://github.com/[your-username]/nirvana-proposal.git
git push -u origin main

# 5. Enable GitHub Pages
gh repo edit --enable-pages
```

## Option 3: Using Git Commands (Manual)

### Steps:
```bash
# 1. Create repository on GitHub.com (web interface)

# 2. Clone it locally
git clone https://github.com/[your-username]/nirvana-proposal.git
cd nirvana-proposal

# 3. Copy all files to this folder
cp /path/to/your/files/* .

# 4. Commit and push
git add .
git commit -m "Add Nirvana SR Proposal"
git push origin main

# 5. Enable GitHub Pages via web interface
```

## Testing Your Site
1. **Wait 1-2 minutes** after enabling GitHub Pages
2. **Visit**: `https://[your-username].github.io/nirvana-proposal/`
3. **Test on mobile**: Open the link on your phone
4. **Test download**: Click the PDF download button

## Troubleshooting
- **404 Error**: Wait a few minutes, GitHub Pages needs time to deploy
- **CSS not loading**: Check if all files are uploaded correctly
- **PDF not downloading**: Ensure PDF file is in the repository root

## Share with Shareholders
Once deployed, share this link:
`https://[your-username].github.io/nirvana-proposal/`

They can:
1. View the beautiful HTML presentation
2. Download the complete PDF
3. View on any device

---
*Last updated: April 4, 2026*
