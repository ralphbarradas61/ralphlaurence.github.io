# Ralph Laurence — Arduino Portfolio

## Files
- `index.html` — the whole site
- `media/` — project videos and preview images
- `thumb.jpg` — preview picture when the link is shared
- `firestore.rules` — security rules for Firebase (views, likes, rating, comments)

## Turn on views, likes, rating and comments (Firebase)
1. Go to https://console.firebase.google.com and create a project.
2. Build → Authentication → Get started → Sign-in method → enable **Anonymous**.
3. Build → Firestore Database → Create database (production mode, region asia-southeast1).
4. Firestore → Rules tab → paste everything from `firestore.rules` → Publish.
5. Project settings (gear icon) → Your apps → Web (</>) → register app.
   Copy `apiKey`, `authDomain`, `projectId`, `appId`.
6. Open `index.html`, find `FIREBASE_CONFIG` near the top, paste the 4 values, save, upload again.
7. Authentication → Settings → Authorized domains → add `YOURNAME.github.io`.

Until step 6 is done the site works normally; the views/likes/rating/comments just stay hidden.
