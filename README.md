Ready-made Signup and Login screens with cutom text field inputs using Firebase and GetX. <\br>

### Features- 
1. User state perisitance <\br>
2. Firebase signup, login (using email and password), and sign out using Firebase Auth <\br>
3. Image file upload ( to Firebase Storage) using Image Picker library <\br>
4. Custom user model for Firebase Firestore database <\br>
5. Snackbars indicating the status (error/success) <\br>

### Steps: 


### Changes to make before running it on your device- 
1.  in lib/controller/auth_controllers registerUser function --> await firestore.collection('users'). Change 'users' to your Firestore's collection name. <\br>
2.  in  lib/controller/auth_controllers _uploadToStorage function -->  Reference ref = firebaseStorage.ref().child('profilePics').  Change 'profilePics' to the name you want to store the photos as in your Firebase Storage. <\br>
3. review lib/controller/auth_controllers file diligently and make changes according to the functionalities you require.<\br>
       

#### Note: you can modify the existing code according to your design. <\br>



