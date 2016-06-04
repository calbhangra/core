# Goals
To develop a full-featured team management application.

The app should:
- make common team tasks **easier**, not harder; else *no one* will use it
- be fully responsive as it will mostly be used on mobile devices
- eliminate the need to login to the Cal Bhangra google account unless absolutely necessary
- utilize new technologies such as ServiceWorkers & WebWorkers to make the user experience better
- emulate a native app experience as close as possible be using "pinned web app" features
    - [Andriod](https://developer.chrome.com/multidevice/android/installtohomescreen)  
    - [iOS](https://developer.apple.com/library/ios/documentation/AppleApplications/Reference/SafariWebContent/ConfiguringWebApplications/ConfiguringWebApplications.html)
    - [Draft W3C Spec](https://w3c-webmob.github.io/installable-webapps/)
    - [Google Progressive Web Apps](https://developers.google.com/web/progressive-web-apps/)
- follow Google's web development [best practices](https://developers.google.com/web/#follow-best-practices)
- have an automatic deployment process from commit to test to actual deployment to server
- follow best practices and have tests, aim to keep code coverage about 95%

## Feature List
- allow for management of gigs
    - any user should be able to "create" a gig
    - all users should be able to respond yes or no to whether they can do the gig
    - owner of the gig should be able to send push notifications to users who have not responded
    - non team members should be 
    - **Discuss:** integrate with Venmo for automatic payments?
- integrate with Google Drive to allow for scoped sharing of files
    - user should be able to upload file and then share with a subset or all of the team members
    - user should be able to adjust sharing details after the fact
    - user should be able to view all of their files as well as ones shared with them
    - admin by default can view all files
- integrate with YouTube to allow uploads and viewing of private videos
    - user should be able to upload videos and limit the viewing audience; 
        - this can be achieved by uploading a private video and only showing the link to users the owner specifics, however should a malicious user copy the link, nothing can be done.
        - if better method is possible, go that route
    - **Discuss:** Should revoking be a feature? If someone copies the link, can't really revoke
    - user should be able to view all videos they've uploaded as well as those shared with them
- integrate with GroupMe *Low Priority*
    - this a "nice to have" feature since GroupMe has a web as well as phone apps
    - user should be able to view and respond to messages
- integrate with the formations application
    - any user should be able to create formations
    - all users should be able to view formations
    - a formation should be scoped to any given set & mix
    - a formation can be in any of three stages: idea, testing, final
        - idea can be created by anyone on the team, and its just that, an idea for a formation
        - a formation can be moved into testing by a captain, this means the formation isn't final, but is a candidate to become final
        - a formation can then be moved from testing to final, this means the formation is mostly set in stone for a given set
- create platform for sharing songs
    - idea is that more people will share songs, our mixes will become better
    - any person can share a song
    - songs can be tagged by user to allow for easy searching
        - example: jugni, intro, ending, etc.
