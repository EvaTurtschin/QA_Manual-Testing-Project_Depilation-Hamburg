#BR-03
## Bug Report: Logo Click Scrolls Incompletely – Top Block Hidden
**ID:** BR-03  
**Date:** 2025-10-01  
**Reporter:** Evgeniya Turtschina  
**Test Case:** 
  [TC01 – Header Navigation: Logo](/Test-Cases.md#tc01--header-navigation-logo)

**Environment:**  
- Browser: Edge 140  
- Resolution: 374–376px, 1320px, 1980px (DevTools)
- Device: Desktop 
- OS: Windows 11 

**Description:**  
Clicking the page logo does not scroll the viewport fully to the top, causing the top of the first content block to be hidden behind the fixed header.  

**Steps to Reproduce:**  
1. Open the website.
2. Click the "About me" navigation link in the header to scroll down the page.
3. Сlick the page logo in the header.

**Expected Result:**  
- The viewport scrolls completely to the top of the page.
- All header elements and the top content block are fully visible without overlap. 

**Actual Result:**  
- The viewport stops short of the top.
- The top part of the first content block is hidden behind the header.

**Severity / Priority:**  
- Severity: Major
- Priority: Medium 

**Attachments / Screenshots:**  
![BRo3](/Bug-Report%20Attachments/BR03.mp4)  

**Notes / Additional Info:**  
- Issue consistently reproducible across Chrome, Edge, and Firefox.
- Likely related to incorrect offset calculation for anchor scroll positions in combination with a fixed header.
