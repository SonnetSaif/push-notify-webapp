# Push-Notify-WebApp

A web application for receiving push notifications using **Firebase Cloud Messaging (FCM)**. Demonstrates handling notifications in both **foreground** and **background** states.

---

## Features

- **Foreground Notifications**: Handle and display notifications when the app is open.
- **Background Notifications**: Automatically display notifications when the app is in the background or closed.
- **Firebase Integration**: Uses Firebase Cloud Messaging for push notifications.
- **Service Worker**: Implements a service worker to handle background messages.
- 
---

## Prerequisites

- Firebase project with Cloud Messaging enabled.
- A **VAPID key** from the Firebase Console.
- A modern web browser that supports service workers (e.g., Chrome, Firefox, Edge).

---

## Setup

1. **Add Firebase Configuration**:
   - Replace the Firebase credentials in `main.js` and `firebase-messaging-sw.js` with your project’s configuration.

2. **Add VAPID Key**:
   - Replace `YOUR_VAPID_KEY` in `main.js` with your Firebase VAPID key.

3. **Deploy the App**:
   - Host the app on a web server (e.g., Firebase Hosting, Netlify, or static hosting).

---

## How It Works

1. **Foreground Messages**:
   - Handled via `onMessage` in `main.js` when the app is open.

2. **Background Messages**:
   - Handled by the service worker (`firebase-messaging-sw.js`) using `onBackgroundMessage`.

---

## Usage

1. Open the app in a browser.
2. Allow notifications when prompted.
3. Send test notifications via the Firebase Console or a backend.
4. Verify notifications in both app states.

---

## Contributing

Contributions welcome! Open an issue or submit a PR for improvements.

---

## License

MIT License. See [LICENSE](LICENSE).

---

## Acknowledgments

- [Firebase Documentation](https://firebase.google.com/docs)
- [MDN Service Workers Guide](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API)
