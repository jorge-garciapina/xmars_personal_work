# Activity Feature Requirements
This document outlines the requirements for the “Activity” feature, inspired by Slack, to be implemented in the XMARS application. 
The purpose of the feature is to give the user a feed with all the Workspace activity that might include mentions, threads, reactions to user’s messages and invitations.

![image 1](	/assets/1.png)

## Requirements
-	Users can see a chronological list of recent activities.  
   ![image 2](	/assets/2.png)

-	Users can filter activities by type (mentions, replies to threads, reactions): Using the filter tabs along the top of the notification feed, user can adjust the feed to see specific notifications, or switch to All to see all the latest notifications.
   ![image 3](	/assets/3.png)

-	**Mentions**: messages the user has been mentioned in, with the name of the conversation or thread, the name of the person who mentioned and a preview of the message.
   ![image 4](	/assets/4.png)

-	**Threads**: a list of replies to threads the users follows , or threads the user has been mentioned in.
   ![image 5](	/assets/5.png)

-	**Reactions**: if someone reacts to any of the user’s messages, the message will be shown with all its reactions.
   ![image 6](	/assets/6.png)
     *	Inside the reaction notification, the user can add more reactions to the same message.
        ![image 7](	/assets/7.png)

-	**Apps**: messages from apps, like google calendar invitations or bots inside the application.
   ![image 8](	/assets/8.png)
  
-	**Invitations**: Invitations to collaborate such as channels the user has been added to and canvases that have been shared with the user.
   ![image 9](	/assets/9.png)

-	Users can filter activities by read/unread
   ![image 10](	/assets/10.png)
   ![image 11](	/assets/11.png)

-	**Activity badge notifications**: the Activity icon on Slack will show a numbered or a dot badge for every unread notification.
   ![image 12](	/assets/12.png)
  
## Contents of every notification on the Activity feed
   ![image 13](	/assets/13.png)

Every Item of the Activity feed should contain:
-	Type of activity: the type of activity the item stands for, it can be Mention, Thread reply, Reaction, Invitation.
-	Thread or channel information: information about the channel or thread related to the activity.
-	Time stamp: the time and date when the activity occurred.
-	Message/content: The main content or message of the notification, providing details about the activity.
     *	The message/content might contain the avatar/icon about the user or channel related to the activity.
  
## Interaction
-	When clicking on any of the Activity items, the user is taken directly to the specific channel or thread. Also, the selected item will have a change on its background color to a lighter one
   ![image 14](	/assets/14.png)
-	When hovering over any of the Activity items, action buttons will be displayed.
   ![image 15](	/assets/15.png)
 	
	These Action buttons are:
    * **Save for later**: this will add this notification to the “Later” section. If clicked, a new legend “Saved for later” on the notification will be added and the color of the icon will be changed:
      
      ![icon 1](	/assets/icons/1.png)

      ![image 16](	/assets/16.png)
      
    * **More actions**: this button will open a menu with more options depending on the type of notification.
 
      ![icon 2](	/assets/icons/2.png)
 
     ### Different notifications: 
     1. Reply to thread notification:
     
         ![image 17](	/assets/17.png)
     
        - 	**Remind me about it**: it will open a second menu with some default times and the option to customize the time for the reminder to take place.
    
            ![image 18](	/assets/18.png)
       	
        - 	**Turn off notifications for replies**: it will stop notifications for this specific thread replies. Also, it will change this option to “Get notified about new replies”.

             ![image 19](	/assets/19.png)
       	
        - 	**Open new window**: will create a new window and open the message/thread on it.
    
             ![image 20](	/assets/20.png)
       	
        -  **Open in home**: it will open the message/thread on the home view of the application.
    
             ![image 21](	/assets/21.png)
    
        -   **Copy Link**: will copy the link to the message/thread to the clipboard.
  
     3. Reaction notification:
     
        The options of this menu will behave the same as the ones in “Reply to thread” notifications:
     
         ![image 22](	/assets/22.png)
     
     4. Mention notification:

        The options in this menu will behave the same as the previous ones, except for “Mute channel” that will stop the Mention notifications from this channel.
     
         ![image 23](	/assets/23.png)
        
    *  **Mark as read**: If the notification has not been read, another action button will be displayed. This button will mark as “Read” the notification.
      
      ![icon 3](	/assets/icons/3.png)
