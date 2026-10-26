# CardVerse Firebase Login Starter

## Included
- Mobile-friendly CardVerse page with six game cards.
- Firebase email/password sign-up, sign-in, sign-out and password-reset UI.
- 500,000 virtual coins shown as a demo display only.

## Required setup before login works
1. Open Firebase Console → Project settings (gear) → General → Your apps → CardVerse web app.
2. Select SDK setup/configuration → Config and copy the complete `firebaseConfig` object.
3. In `index.html`, replace the placeholder `apiKey`, `storageBucket`, and `appId` with the exact values from Firebase. Do not guess these values.
4. Commit `index.html` to GitHub and wait for GitHub Pages to redeploy.
5. Confirm Firebase Authentication → Sign-in method → Email/Password is enabled.
6. Firebase Authentication → Settings → Authorized domains: ensure `nk7108715-source.github.io` is listed; add it if needed.

## Limitations and safety
- Online multiplayer, persistent private rooms, live voice chat, and a secure wallet are not implemented.
- The 500,000 coins are only a UI display, not stored as a real balance.
- Firestore rules currently deny all reads/writes. Keep them closed until secure rules are configured. Never use public `allow read, write: if true` rules.
- Never place Firebase Admin SDK keys or service-account credentials in this HTML.
- Virtual coins only; no cash-out or real-money wagering.
