# An Android application to buy and sell used books. 

## Following is the list of features: 

###### Implemented barcode scanner 
   - Made use of react-native-barcodescanner.

   - Added custom code to disable camera after scanning the first instance of barcode.

   - Without the custom code, the external package continues to push new scenes on to the navigation stack as long as the camera is pointed at the barcode.

   - User also has the option to key in ISBN in case the book's barcode is damaged.

###### Implemented native camera
   - Used an external package called react-native-camera.

   - This is the second feature that makes use of mobile platform.
   
###### Used an external API to upload images:
   - We made use of the following post API provided by Imgur to upload the images: https://api.imgur.com/3/image 
   
   - This allowed us to save space in our database.
   
###### Kept user input to a minimum while uploading new books:
   - User just needs to scan the barcode of the book and enter the price.
      
   - All other details of the book are fetched from the following google API: https://www.googleapis.com/books/v1/volumes?q=<ISBN>
   
###### Multiple user support: 
   - Each user can upload new books 
   - Each user can add books posted by other users to his interest list 
   - User has his own personalized upload list and interest list 

###### Edit content:
   - User can edit the price of the book
   
###### Delete content:
   - User can delete the books uploaded by him 

###### Search by title

###### Local user authentication

__Argument of execution:__

We believe we have come up with a decent android application which has all the above mentioned features. The project is well structured and is divided into several modules for ease of maintaineance (modules are: assets, components, images, screens, services, styles). 

For styling, we made use of NativeBase and also custom components as deemed necessary. 

10 APIs have been implemented on server and these APIs are responsible for communication between client and database. 

Also, we faced a scenario where we had to pass a scene itself as a prop to the next scene so that data can be passed back from the new scene to the old scene when the new scene is popped from navigation stack. Had fun implementing this feature. 

## Screenshots ##

###### Login 

<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/login.jpeg" alt="Login" width="250" height="400"/>

###### Explore 
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/explore.jpeg" alt="Login" width="250" height="400"/>

###### Drawer
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/drawer.jpeg" alt="Login" width="250" height="400"/>

###### My Uploads 
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/my_uploads.jpeg" alt="My Uploads" width="250" height="400"/>

###### My Interests
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/my_interests.jpeg" alt="My Interests" width="250" height="400"/>

###### Book details
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/book_details.jpeg" alt="Book details" width="250" height="400"/>

###### Search feature 
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/search_feature.jpeg" alt="Search" width="250" height="400"/>

###### Barcode scanner
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/barcode_s.jpeg" alt="Barcode Scanner" width="250" height="400"/>

###### Image upload
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/img_upload.jpeg" alt="Login" width="250" height="400"/>

###### Auto populate book details
<img src="https://github.com/umn-5117-f16/module-4-group-project-webcrows/blob/master/auto_populate_book_details.jpeg" alt="Login" width="250" height="400"/>
