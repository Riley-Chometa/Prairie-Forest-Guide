# Prairie Forest Guide
## Overview
Prairie Forest Guide is a mobile application developed during a year-long projects class at Saskatchewan Polytechnic for a local non-profit here in Saskatoon called Friends of the Saskatoon Afforestation Aread Inc. (FSAAI). It allows users to view “digital signs” placed at specific locations on a map when they are nearby. An admin panel web app enables FSAAI to manage and place these signs. Initially designed as a native app, it was later transitioned to a progressive web app (PWA) due to concerns around Xamarin deprecation and the lack of Apple devices for testing.

## Native App Version
### Features
- **Interactive Map:** The applications main page is a map where the user will be able to see their current location and nearby digital signs.
- **Digital Signs:** Digital signs contain a title, a short description of the topic, an image, and a button that links out to a webpage for the end user to "learn more" if the would like to know more about the subject in the sign.
- **Events:** FSAAI can list upcoming events occuring in their parks for end users to see in a separate tab in the application itself.
- **Feedback Survey:** The application contains a feedback survey that useres can fill out to rate their experience in the app, in their parks, and leave any specific feedback they have as a comment at the end of the survey.
- **Admin Panel:** FSAAI can manage the digital signs and events from the admin panel, as well as view statistics and comments from their feedback survey.

### Tech Stack
- **Xamarin:** For cross-device native application development on both Android and IOS.
- **Microsoft .Net Core MVC:** For development of the Backend API and Admin panel.
- **Google Maps API:** For the map interface and tools needed to implement the main feature of the application.

### Challenges and Solutions
After completion of the projects class the kind people at FSAAI obtained grant money to hire us on as contract developers to complete development of a few more features. During that time we ran into some challeneges associated with both continuing development of the current application and releasing it to the public.
- **Xamarin Deprecation:** During out development of the application as part of our project we started to notice a worrying trend of many already deprecated functions and outdated documentation as well as concerns around support for Xamarin in the future. Contributing to our decision to rework the project.
- **Testing Limitations:** The team lacked Apple devices, making it difficult to test the iOS version or even have it released for use on Apple devices at all.
- **Solution:** Transitioning to a Progressive Web App (PWA) allowed us to mitigate these issues and lean up our original code. Though we couldn't officially test the application on an Apple device still or the Safari browser, we felt it was the best compromise that would allow for more users to access the application while also streamlining the development process so we decided to port the application over to Angular js using Ionic for native UI elements on the frontend of the application.
This experience taught me to thoroughly evaluate the tools we choose and to prefer more popular solutions that are likely to be supported for the foreseeable future.

## Progressive Web App Version
### Features
In addition to porting the application to a Progressive Web App (PWA), the following features were added to the application as part of our contract on top of [the previously mentioned features](#native-app-version).
- **Sign Filtering:** After the original projects end, we were hired on to continue work on the project, one of those features was the ability for end users to set a custom filter for what type of signs they wish to see. The signs all get a Category given to them and users can decide if they want to see a certain category or not if they're more interested in certain subjects then others.
