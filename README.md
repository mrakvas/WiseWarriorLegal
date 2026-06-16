# Wise Warrior — public legal pages

Static **Privacy Policy** and **Support** pages for App Store Connect and in-app links.  
No app source code — safe to keep this repository **public**.

## Why a separate repo?

| Approach | Verdict |
|----------|---------|
| **This repo (public, legal only)** | Recommended — only visitor-facing pages; app + System repos stay private. |
| **Private app repo + GitHub Pages** | Works — Pages site is public while code stays private — but couples legal to the app repo. |
| **Private System repo + Pages** | Same as above; System holds internal docs you do not want public. |

## Publish (one-time)

1. Create a **public** GitHub repo named `WiseWarriorLegal` (or push this folder).
2. **Settings → Pages → Build from branch `main` → folder `/ (root)`**.
3. Wait ~2 minutes. Live base URL:

   `https://mrakvas.github.io/WiseWarriorLegal/`

4. Use in App Store Connect:

   | Field | URL |
   |-------|-----|
   | Privacy Policy | `https://mrakvas.github.io/WiseWarriorLegal/privacy.html` |
   | Support URL | `https://mrakvas.github.io/WiseWarriorLegal/support.html` |
   | Marketing URL | `https://wisewarriorboxing.com/blog-post6` |

5. Mirror URLs in `WiseWarriorTimer/constants/brand-links.ts`.

## Files

- `privacy.html` — Privacy Policy
- `support.html` — Support / contact
- `index.html` — Short index linking both pages

Update the **Effective date** in `privacy.html` when you materially change the policy.
