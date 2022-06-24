Ready-made Signup and Login screens with cutom text field inputs using Firebase and GetX. 

### Features- 
1. User state perisitance 
2. Firebase signup, login (using email and password), and sign out using Firebase Auth </br>
3. Image file upload ( to Firebase Storage) using Image Picker library 
4. Custom user model for Firebase Firestore database 
5. Snackbars indicating the status (error/success) 

### Steps: 
Setup your Firebase project with your Flutter projet's bundle id and downlaod the services.json file and then move it to it project/android/app directory.
Go to the Authentication tab and enable email password sign in.
create a database in Firestore and edit the rules (allow read, write; ) after it is set up, or any other custom rule.


### Changes to make before running it on your device- 
1.  in lib/controller/auth_controllers registerUser function --> await firestore.collection('users'). Change 'users' to your Firestore's collection name. 
2.  in  lib/controller/auth_controllers _uploadToStorage function -->  Reference ref = firebaseStorage.ref().child('profilePics').  Change 'profilePics' to the name you want to store the photos as in your Firebase Storage. 
3. review lib/controller/auth_controllers file diligently and make changes according to the functionalities you require. <\br>
       
      
![signup](https://user-images.githubusercontent.com/71487701/175515977-555284fb-e69f-4313-9667-2a18c31893ff.png)

![login](https://user-images.githubusercontent.com/71487701/175515994-993d2dab-119a-4fcf-acf6-40bb6288be46.png)

#### Note: 
1. you can modify the existing code according to your design. 
2. classpath and other configuration have already been set up inside android/app/build.gradle file and google services dependency has been added to the project level build.gradle file.
3. min sdk versio is set to 19. <\br>
![1](https://user-images.githubusercontent.com/71487701/175516061-3e1872ae-1176-4c66-8916-fa95554592b5.png)
![2](https://user-images.githubusercontent.com/71487701/175516064-0e1c66ee-db9e-438e-912d-ec50f6092d4a.png)
![3](https://user-images.githubusercontent.com/71487701/175516066-22736e27-1fd9-4620-ae21-0956e8314511.png)





