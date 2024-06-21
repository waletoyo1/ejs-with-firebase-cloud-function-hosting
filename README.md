# ejs-with-firebase-cloud-function-hosting
Using ejs with firebase cloud function &amp; hosting to serve dynamic website


1. Create a folder called templates under functions/lib directory
2. Place your ejs file inside the templates directory
3. Crerate your typsecript function in the src folder and make it possible to access a unique variable/handle from firestore
4. Deploy your cloud function
5. Place this in your firebase.json file under hosting:   "rewrites": [
      {
        "source": "/:handle",
        "function": "handleUserRequest"
      }
    ]

6. handleUserRequest is the cloud function that was deployed above
7. Visit your url e.g xyz.com/handle to show your dynamic website
