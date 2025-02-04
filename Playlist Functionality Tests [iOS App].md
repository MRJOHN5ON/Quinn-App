# Playlist Functionality Tests - iOS App

**Ryley Johnson**  
**1/19/2025**  

## Creating a Playlist  
- Successfully created playlists appeared with a default title and no description.  
- **No issues observed.**  

## Adding Stories to Playlists  
### Single Stories  
- Stories were added **immediately and seamlessly**, with no performance issues, even when adding over **100 stories**.  

### Multiple Stories  
- Adding stories to a pre-existing playlist worked, but the **Library tab's Recent Activity list incorrectly displayed only one story** in the playlist.  
- Opening the playlist showed the **correct number of stories**.  
- **Video Evidence:** [iOS Recent Activity Issue](iOS_recent_activity.MP4)  

### Improvement Noted  
- The ability to **add stories from anywhere in the app via the three-dot menu** was a **major improvement** over the web app, eliminating the need to navigate back to a playlist.  
- **Video Evidence:** [iOS Enhancement](iOS_enhancement.MP4)  

## Reordering and Removing Stories  
### Reordering Stories  
- Worked **smoothly and seamlessly** with no glitches or errors.  

### Removing Stories  
- Functionality worked as expected.  
- **Improvement Suggested:** Allow story removal **directly from the three-dot menu** next to the story, rather than requiring multiple steps.  

## Classifying Playlists (Public/Private)  
- Privacy toggles worked **flawlessly**, with **visibility permissions updating immediately** across both the **iOS app and web browser**.  

## Favoriting Audio  
- Favoriting and removing favorites **functioned without any issues**.  

## Changing Playlist Title and Description  
### Boundary Testing  
- **Title field:** Accepted **1–25 characters**  
- **Description field:** Accepted **0–512 characters**  
- Both fields **adhered to these boundaries** during typing and copy-pasting.  
- **Tested Inputs:** Numbers, symbols, foreign languages, basic SQL injections.  

### Issue Identified  
- **Titles consisting of only spaces were still accepted, resulting in nameless playlists.**  

### Improvement Noted  
- **Playlist descriptions were correctly displayed in the iOS app**, unlike the web application.  

## Network Speeds and Offline Behavior  
### Offline Testing  
- **Elements turned a masked gray color when offline**, indicating that no changes could be made—**an improvement over the web app**.  

### Note  
- **Network speed testing was limited** due to time constraints and the lack of a **BrowserStack subscription**.  
- Further testing is required to fully validate performance across various network conditions.  

## Playlist Duration  
- **No discrepancies** were observed with playlist durations.  
- Unlike the web app, where the **total duration was off by one second**, iOS playlist durations were **accurate**.  
