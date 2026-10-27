CardVerse Firestore real wallet (read-only)

Upload this index.html to the root of your existing GitHub repository, replacing the old index.html.
It reads users/{signed-in-user-UID}.coins from Cloud Firestore and displays the stored balance.
It does not allow the browser to change coins. Keep Firestore rules restricted to the signed-in owner; never allow public writes to coins.

If the page says wallet document missing, in Firebase Console > Firestore Database > users, confirm a document exists whose document ID exactly matches the signed-in user's Authentication UID, and that it has a numeric coins field (e.g. 500000).
