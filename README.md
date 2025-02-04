# Playlist Functionality Testing - Quinn App
![Quinn App](https://a57.foxnews.com/static.foxbusiness.com/foxbusiness.com/content/uploads/2022/01/720/405/quinn-erotic-app-05.jpeg?ve=1&tl=1)

## Overview

This repository contains the results of a comprehensive testing assignment conducted for the **Quinn app**. The app includes a key feature—the "playlist functionality"—which allows users to create and manage audio playlists by adding, removing, and reordering stories. The primary goal of this project was to evaluate this functionality across both **iOS** and **web platforms**, highlighting potential issues with core functionality, UX, and performance under various network conditions.

## Company: Quinn App
For more information, visit their official website: [http://tryquinn.com/](http://tryquinn.com/)

Quinn  is an audio-based storytelling platform that offers a diverse collection of immersive, intimate, and ASMR-style content. Focused on audio-first experiences, Quinn provides a safe and private space for users to explore sensual storytelling, roleplays, and relaxation audios. The platform is driven by user-generated and professionally curated content, making it a unique alternative to traditional adult media.

## Project Scope

The project focused on manual testing of the **playlist functionality** within the Quinn app, including:

- **Core Functionality Testing**: Testing the basic functionality of creating, adding, and managing playlists.
- **User Experience (UX) Validation**: Ensuring that the user interface and user experience were smooth and intuitive.
- **Edge Case Testing**: Identifying any edge cases, such as very large playlists or uncommon inputs.
- **Cross-Platform Testing**: Testing the functionality on both **iOS** and **web platforms** (Chrome & Safari browsers).
- **Performance Testing**: Observing performance under varying network conditions and offline mode.

## Tools Used

To explore different testing scenarios, I used the following tools:

- **Postman** – For API testing and sending `POST` requests to validate playlist manipulation.
- **Chrome DevTools** – To inspect network activity, debug UI issues, and analyze API responses.
- **Loom** – For recording and sharing video evidence of bugs and UI behaviors.
- **Google Docs** – To document test cases and findings in an organized format.
- **Safari Web Inspector** – For debugging and testing playlist functionality in Safari.
- **Network Throttling (DevTools)** – To simulate different network conditions, such as slow 3G.
- **iOS Testing (Physical Device & Simulator)** – To manually test app behavior on iPhones.

## What Was Expected of Me

The task was to test the following features of the Quinn app:

- **Creating Playlists**: Creating new playlists and verifying their behavior.
- **Adding Stories**: Adding single and multiple stories to playlists and ensuring proper updates.
- **Reordering and Removing Stories**: Testing the ability to reorder and remove stories.
- **Classifying Playlists**: Verifying the privacy settings of playlists (public vs. private).
- **Favoriting Stories/Playlists**: Ensuring users could favorite stories and playlists without issues.
- **Changing Playlist Title and Description**: Ensuring the title and description fields functioned correctly with boundary testing.
- **Network and Offline Behavior**: Testing functionality under different network speeds and offline conditions.

## What I Found

During testing, I observed several critical and minor issues across both the **iOS** app and the **web platform**:

### iOS App:
- **Playlist Creation**: Worked without issues.
- **Adding Stories**: Both single and multiple story additions worked well, with an issue in the Recent Activity list showing incorrect counts when adding multiple stories.
- **Reordering/Removing Stories**: Functionality worked smoothly, though the removal process could be improved by allowing users to remove stories directly from the three-dot menu.
- **Title Input Issue**: The app allowed playlist titles consisting only of spaces, resulting in nameless playlists.
- **Offline Behavior**: Offline mode worked better than the web app, with elements turning gray to indicate no changes could be made.

### Web App:
- **Playlist Creation**: Worked without issues.
- **Adding Stories**: Both single and multiple story additions worked smoothly. However, there was a delay in updating the Library overview count until the page was reloaded.
- **Reordering/Removing Stories**: Seamlessly functional across platforms.
- **Favoriting**: The “like” count in the Account Overview tab remained at zero when favoriting individual stories or playlists.
- **Title Input Issue**: Similar to the iOS app, titles consisting only of spaces were accepted, creating nameless playlists.
- **Network Speed Testing**: Search results and story addition times were good under fast internet; however, performance slowed on slower networks.
- **Offline Testing**: Offline story additions showed UI changes but failed to synchronize with the server once reconnected.
- **Playlist Duration Issue**: There was a consistent discrepancy in the playlist duration, with a one-second difference between the total duration and the sum of individual story durations.

## Repo Structure

- **Google Docs Reports**: The detailed reports for both **iOS** and **Web** app testing. These documents contain the full findings, including steps to reproduce, expected vs. actual behavior, and device/browser details.
  
- **Postman Demo**: A video demonstrating the use of Postman for API testing can be found within the google docs. This showcases how requests were sent for manipulating playlists using data from the Chrome DevTools network tab.

- **Loom Videos**: Links to Loom videos demonstrating certain bugs and issues found during testing are included throughout the report.

---

## Conclusion

Through comprehensive testing, I identified several areas for improvement in both the **iOS app** and **web app**, including UI issues, performance discrepancies under network constraints, and edge cases involving playlist titles. Overall, the core functionality worked well, and suggestions for enhancing the user experience have been documented for further development.

---
