#BR-05
## Bug Report: Facebook Icon Click Opens Wrong Page
**ID:** BR-05  
**Date:** 2025-10-02  
**Reporter:** Evgeniya Turtschina  
**Test Case:** 
  [TC09 – Header Navigation: Social Media Icon Facebook](/Test-Cases.md#tc09--header-navigation-social-media-icon-facebook)

**Environment:**  
- Browser: Edge 140  
- Resolution: Desktop 1920x1080
- Device: Desktop 
- OS: Windows 11 

**Description:**  
Clicking the Facebook icon in the header opens the website’s main page instead of the intended Facebook profile in a new tab.  

**Steps to Reproduce:**  
1. Open the website.
2. Click on the Facebook icon in Header

**Expected Result:**  
- A new tab opens with the correct Facebook profile.
- The original page remains open. 

**Actual Result:**  
- A new tab opens with the website’s main page instead of the Facebook profile.

**Severity / Priority:**  
- Severity: Major
- Priority: High 

**Attachments / Screenshots:**  
![BRo5](/Bug-Report%20Attachments/BR05.mp4)  

**Notes / Additional Info:**  
- Likely issue with incorrect href or target attribute on the Facebook icon link.
