#BR-01
## Bug Report: Header "Location with Address" Overlapping in 769–1370px Range
**ID:** BR-01  
**Date:** 2025-09-28  
**Reporter:** Evgeniya Turtschina  
**Test Case:** [TC26 – Header Display on Desktop (768px)](Test-Cases.md#tc26--header-display-on-desktop-768px)  

**Environment:**  
- Browser: Edge 140  
- Resolution: Desktop viewport range 769–1370px (DevTools)  
- Device: Desktop  
- OS: Windows 11  

**Description:**  
The "Location with Address" link in Header navigation overlaps with the "Contacts" link when screen width is between 769px and 1370px.  

**Steps to Reproduce:**  
1. Open the website in Edge.  
2. Open DevTools and set viewport width to values between **769px and 1370px**.  
3. Observe the Header navigation.  

**Expected Result:**  
- At widths greater than 768px, "Location with Address" should be visible and correctly positioned.  
- Navigation items should not overlap or collide.  

**Actual Result:**  
- From 769px to ~1370px, "Location with Address" appears but overlaps with "Contacts".  
- Layout breaks and links are partially unreadable.  

**Severity / Priority:**  
- Severity: Major  
- Priority: High  

**Attachments / Screenshots:**  
![BRo1_1](/Bug-Reports/BR01_1.png)  
![BRo1_2](/Bug-Reports/BR01_2.png)
![BRo1_3](/Bug-Reports/BR01_3.png)

**Notes / Additional Info:**  
- At exactly 768px width, design specifies that "Location with Address" is hidden. This is working as expected.  
- Issue reproduces only in the 769–1370px range, indicating a missing responsive breakpoint or incorrect CSS handling.


