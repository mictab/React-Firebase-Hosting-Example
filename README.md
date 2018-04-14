# React-Firebase-Hosting-Example
A simple example to show how you can deploy a create-react-app to Firebase Hosting

The deployed app can be seen at https://iprog-firebase-example.firebaseapp.com/

Please also have a look at `.gitignore` to see things you ideally shouldn't be commiting to Github (e.g. node_modules and build folders).

## Steps

1. Create a React project, e.g. with `create-react-app`
2. Make sure that everything runs fine locally
3. Go to Firebase Hosting, go to the console and create a new project (https://console.firebase.google.com/u/0/)
4. Press `Add project`. Give it a name and select a region. After pressing Continue, you should see a new page.
5. Press Hosting on the sidebar to your left. Then select "Getting Started". Read the instructions.
6. Go back to your repo. Run `firebase login` and make sure you're logged in to
   your Google account.
7. Now run `firebase init`. Select "Hosting" as the option and specify `build` as your public folder (you can have a look at the `firebase.json` file in this repository). You should see some new files in your directory named `.firebaserc` and `firebase.json`.
8. Run `npm run build` or `yarn build` in the root of your repository. You
   should see a new `build` folder (don't commit this one to git).
9. Run `firebase deploy`. Your project should now be hosted just fine.
