# files-to-firebase-react

# 🚀 Javascript full-stack 🚀

### React / files to firebase react

Upload files to Firebase with React and save URL in MongoDB with Node.

https://github.com/coding-to-music/files-to-firebase-react

https://files-to-firebase-react.vercel.app

https://files-to-firebase-react.herokuapp.com

by CyberWolve https://github.com/cyber-wolve

https://github.com/cyber-wolve/files2firebase

## Environment Values

```java
	apiKey: process.env.REACT_APP_API_KEY,
	authDomain: process.env.REACT_APP_AUTH_DOMAIN,
	projectId: process.env.REACT_APP_PROJECT_ID,
	storageBucket: process.env.REACT_APP_STORAGE_BUCKET,
	messagingSenderId: process.env.REACT_APP_MESSAGING_SENDER_ID,
	appId: process.env.REACT_APP_APP_ID,

	const url = process.env.REACT_APP_API_URL + "/songs"

    await mongoose.connect(process.env.MONGODB_URI, connectionParams);

```

## Firebase setup

/client/src/firebase.js

```java
import { initializeApp } from "firebase/app";
import { getStorage } from "firebase/storage";

const firebaseConfig = {
	apiKey: process.env.REACT_APP_API_KEY,
	authDomain: process.env.REACT_APP_AUTH_DOMAIN,
	projectId: process.env.REACT_APP_PROJECT_ID,
	storageBucket: process.env.REACT_APP_STORAGE_BUCKET,
	messagingSenderId: process.env.REACT_APP_MESSAGING_SENDER_ID,
	appId: process.env.REACT_APP_APP_ID,
};

const app = initializeApp(firebaseConfig);
const storage = getStorage(app, process.env.REACT_APP_BUCKET_URL);
export default storage;
```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/files-to-firebase-react.git
git push -u origin main
```

## Heroku

```java
heroku create files-to-firebase-react

```

## Heroku MongoDB Environment Variables

```java
heroku config:set

heroku config:set JWT_SECRET="secret"

heroku config:set PUBLIC_URL="https://files-to-firebase-react.herokuapp.com"
```

## Push to Heroku

```java
git push heroku

# or

npm run deploy
```
