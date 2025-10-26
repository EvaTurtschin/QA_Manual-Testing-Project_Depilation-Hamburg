#BR-04
## Bug Report: Location with Address Hover Color Inconsistent Between Text and Icon
**ID:** BR-04  
**Date:** 2025-10-02  
**Reporter:** Evgeniya Turtschina  
**Test Case:** 
  [TC05 – Header Navigation: Location with Address Hover](/Test-Cases.md#tc05--header-navigation-location-with-address-hover)

**Environment:**  
- Browser: Edge 140  
- Resolution: 1980px (DevTools)
- Device: Desktop 
- OS: Windows 11 

**Description:**  
Hovering over the "Location with Address" header element changes the text color inconsistently: hovering over the text changes both text and icon color, but hovering only on the icon changes only the icon color. Expected behavior is a unified hover effect for the entire block.  

**Steps to Reproduce:**  
1. Open the website.
2. Hover over "Location with Address" in the header:
 - First hover over the text.
 - Then hover over the icon only.

**Expected Result:**  
- The entire "Location with Address" block (text + icon) changes color on hover.
- Layout remains intact. 

**Actual Result:**  
- Hovering over the text changes color for both text and icon.
- Hovering only over the icon changes color only for the icon.

**Severity / Priority:**  
- Severity: Minor
- Priority: Medium 

**Attachments / Screenshots:**  
![BRo4](/Bug-Report%20Attachments/BR04.mp4)  

**Notes / Additional Info:**  
- Likely CSS selector issue: hover effect not applied to the parent block containing both text and icon.
