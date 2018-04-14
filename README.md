# React-Firebase-Hosting-Example
A simple example to show how you can deploy a create-react-app to Firebase Hosting

The deployed app can be seen at https://iprog-firebase-example.firebaseapp.com/

## Steps

1. Create a React project, e.g. with `create-react-app`
2. Make sure that everything runs fine locally
3. Go to Firebase Hosting, go to the console and create a new project
4. Follow the instructions about how to install firebase cli tools given on the website
5. Go back to your repo. Run `firebase login` and make sure you're logged in to
   your Google account.
6. Now run `firebase init`. Select "Hosting" as the option and specify `build` as your public folder (you can have a look at the `firebase.json` file in this repository). You should see some new files in your directory named `.firebaserc` and `firebase.json`.
7. Run `npm run build` or `yarn build` in the root of your repository. You
   should see a new `build` folder (don't commit this one to git).
8. Run `firebase deploy`. Your project should now be hosted just fine.
