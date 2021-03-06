# Open Shopping List

![](https://i.imgur.com/rbqwXdk.gif)

# Features
- Shows online users, a snackbar tells you when someone connects or disconnects
- Delete and Check swipe animations
- Urgent items: They are on the top always
- Animations when someone else removes, adds or checks an item
- Cozy and Compact layout

# Prerequisites
- **Firebase Project**
  - Sign up at https://firebase.google.com/
  - Add a new project
  - Open your new project
  - Add Android app to the project
    - **Android package name**: com.messedcode.openshoppinglist
    - **App nickname**: Open Shopping List
    - **Debug signing certificate SHA-1**: *LEAVE EMPTY*
  - Download configuration file
  - Move configuration file to `/app/src/google-services.json`
  - click database on the left sidebar
  - Change to RULES tab
  - Replace `.read` and `.write` values to `true`

    ```json
    {
      "rules": {
        ".read": "true",
        ".write": "true"
      }
    }
    ```

# Use Case Goals
Make this application usable in public. (Publishing to Play Store.)

- [ ] Add user authentication
- [ ] Make lists' shareable
- [ ] Copying public lists to your own workspace

# Development Goals
- [ ] Setup proper Proguard
- [ ] Rewrite using MVP
- [ ] Decouple from Firebase
- [ ] Write backend server (NodeJS)
- [ ] Move notifications to backend (right now we are sending them directly from the app which exploits our server key)