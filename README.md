# KRUTIK CYBER EXPERT — Free PDF Website (GitHub Pages)

Yeh site 100% phone se chalti hai — koi computer ya terminal nahi chahiye.
Sirf GitHub.com ka browser version (ya GitHub app) use karna hai.

---

## Step 1 — GitHub account banao
1. https://github.com par jao, account nahi hai to "Sign up" karo (free hai).

## Step 2 — Naya repository banao
1. Upar right me **+** icon → **New repository**
2. Repository name: `krutik-cyber-expert` (ya jo naam chaho)
3. **Public** select karo (Pages sirf public repo par free chalta hai)
4. **Create repository** dabao

## Step 3 — Files upload karo
1. Repository ke andar **Add file → Upload files** dabao
2. In 3 files ko upload karo:
   - `index.html`
   - `pdfs.json`
   - `README.md` (optional)
3. Ek folder banao naam `pdfs` aur usme apni PDF files daalo
   (upload karte waqt filename ke aage `pdfs/` type karke bhi folder bana sakte ho, e.g. `pdfs/hacking-basics.pdf`)
4. Neeche **Commit changes** dabao

## Step 4 — GitHub Pages ON karo
1. Repository ke **Settings** tab me jao
2. Left side me **Pages** par click karo
3. **Branch**: `main` select karo, folder `/ (root)`, **Save** dabao
4. 1-2 min baad upar ek link milega, jaisa:
   `https://<tumhara-username>.github.io/krutik-cyber-expert/`
5. Yehi tumhari **live website ka link** hai — isse kisi ko bhi bhej sakte ho.

---

## Naya PDF add kaise karein (har baar)

1. `pdfs` folder me jao → **Add file → Upload files** → apni PDF daalo → Commit
2. Root me `pdfs.json` file khol kar **pencil (edit) icon** dabao
3. Array me ek naya entry jodo, aise:

```json
{
  "title": "Ethical Hacking Basics",
  "description": "Beginner level notes for the course",
  "category": "Ethical Hacking",
  "filename": "hacking-basics.pdf",
  "size": 512000,
  "uploadDate": "2026-08-11"
}
```

- `filename` bilkul wahi naam hona chahiye jo PDF ka hai (jo `pdfs/` folder me daala)
- `size` PDF ki size hai bytes me (approx daal do, koi dikkat nahi agar exact na ho)
- `uploadDate` aaj ki date `YYYY-MM-DD` format me

4. Comma (`,`) laga kar naya entry list me jodo (pehla example entry chaho to hata do)
5. Neeche **Commit changes** dabao

Website apne aap 1-2 minute me update ho jayegi (GitHub Pages ko refresh hone me thoda time lagta hai).

## PDF hatana ho to
1. `pdfs.json` se uska entry delete karo → Commit
2. `pdfs` folder me jaake us file ko bhi delete kar do (teen-dot menu → Delete file)

---

**Note:** Is version me koi password-wala live "admin panel" nahi hai — upload/delete GitHub ki website se hi hota hai. Agar baad me live admin panel chahiye (jisme website ke andar se hi upload ho jaye), to bata dena — uske liye GitHub token wala advanced version bana denge.
