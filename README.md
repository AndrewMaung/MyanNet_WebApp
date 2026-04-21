# MyanNet - Burmese Digit Recognition

A lightweight CNN with TensorFlow.js for real-time Burmese digit recognition. Live demo with drawing pad and camera input.

**Test Accuracy:** 99.49% | **Model Size:** 24.18 KB | **Parameters:** 10,634

## Quick Start - Deploy to Vercel

### Method 1: GitHub (Recommended)

1. **Initialize Git repository:**
   ```powershell
   git init
   git add .
   git commit -m "Initial commit: MyanNet deployment"
   ```

2. **Push to GitHub:**
   - Create a new repository on [github.com](https://github.com/new)
   - Copy the remote URL
   - Run:
     ```powershell
     git remote add origin https://github.com/YOUR-USERNAME/REPO-NAME.git
     git branch -M main
     git push -u origin main
     ```

3. **Deploy on Vercel:**
   - Go to [vercel.com/new](https://vercel.com/new)
   - Import your GitHub repository
   - Click **Deploy**
   - Your app will be live in ~1 minute!

---

### Method 2: Vercel CLI (Fastest)

1. **Install Vercel CLI:**
   ```powershell
   npm install -g vercel
   ```

2. **Deploy:**
   ```powershell
   vercel
   ```
   - Link to your Vercel account
   - Accept defaults
   - Done! Your URL will appear in the terminal

---

### Method 3: Drag & Drop

- Visit [vercel.com](https://vercel.com)
- Drag and drop the entire folder onto the dashboard
- Instant deployment

---

## Local Testing

```powershell
python -m http.server 8000
```
Open `http://localhost:8000` in your browser.

---

## Architecture

- **Block 1:** Conv2D(64,3×3) + BN + ReLU + MaxPool
- **Block 2:** DWConv(3×3) + BN + PW(1×1,64) + BN + MaxPool
- **Head:** GAP → Dropout(0.194) → Dense(64) → Softmax(10)

---

## Model Info

- **Framework:** TensorFlow.js (browser-based)
- **Weights:** Real trained weights (base64 embedded)
- **No server required** — runs entirely in your browser
- **Works offline** after initial page load

---

## Features

✅ **Live Drawing Pad** — Draw digits and get instant predictions  
✅ **Camera Input** — Real-time digit detection  
✅ **Research Details** — Architecture, results, cross-validation  
✅ **Edge Deployment** — Optimized for embedded systems  
✅ **Mobile Friendly** — Responsive design  

---

## Citation

IEEE Research Demo · BHDD Dataset · Marwadi University · 2026
