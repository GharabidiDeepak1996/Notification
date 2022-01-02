# Send FCM Notifications Using Postman

Step 1 :
Select POST type and enter request endpoint URL as 
https://fcm.googleapis.com/fcm/send

Step 2:
Set Authorization Header and Content-Type.
Authorization: key=<server_key> and Content-Type: application/json
Note: You have to copy Legacy Server Key from Firebase Console > Project Settings > Cloud Messaging

Step 3:
Now Select Body > raw > JSON(application/json) and add following JSON object:
{
  "to" : "<YOUR FCM TOKEN>",
 "notification" : {
   "title": "Title of Your Notification",
   "body" : "Body of Your Notification"
 },
 "data" : {
   "key_1" : "Value for key_1",
   "key_2" : "Value for key_2"
 }
}
