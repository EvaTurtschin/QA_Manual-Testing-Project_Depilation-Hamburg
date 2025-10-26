#BR-06
## Bug Report: Location Icon Hover Area Overlaps Other Elements
**ID:** BR-06  
**Date:** 2025-10-02  
**Reporter:** Evgeniya Turtschina  
**Test Case:** 
  [TC05 – Header Navigation: Location with Address Hover](/Test-Cases.md#tc05--header-navigation-location-with-address-hover)
  [TC15 – Footer Navigation: Logo](/Test-Cases.md#tc15--footer-navigation-logo)

**Environment:**  
- Browser: Edge 140  
- Resolution: 1980px (DevTools)
- Device: Desktop 
- OS: Windows 11 

**Description:**  
The hover area of the Location icon in the header and in the footer extends too far, causing unintended overlaps with page content below. When the page is scrolled, attempting to interact with elements (e.g., the top of the map) can trigger the Location hover action, opening the location link in a new tab unexpectedly.  

**Steps to Reproduce:**  
1. Open the website.
2. Scroll the page so the map section appears below the header.
3. Attempt to click on the top part of the map, near where the header’s Location icon would be (when the Location icon changes color on hover)

**Expected Result:**  
- Hover and click areas of the Location icon are limited to the icon/text block in the header.
- Interactions with page content below the header are not affected.

**Actual Result:**  
- Hover area extends beyond the header.
- Clicking elements under the extended hover area triggers the Location action, opening the link in a new tab.

**Severity / Priority:**  
- Severity: Major
- Priority: Medium 

**Attachments / Screenshots:**  
![BRo6](/Bug-Report%20Attachments/BR06.mp4)  

**Notes / Additional Info:**  
- Likely caused by oversized hover/click area in CSS for the Location icon block.
- Problem reproducable with Location link in Header and in Footer