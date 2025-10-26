#BR-02
## Bug Report: Mobile Layout Breaks at 375px and Above
**ID:** BR-02  
**Date:** 2025-09-29  
**Reporter:** Evgeniya Turtschina  
**Test Case:** 
  [TC27 – Header Display on Mobile (375px)](Test-Cases.md#tc27--header-display-on-mobile-375px)
  [TC29 – Hero Section Display on Mobile (375px)](Test-Cases.md#tc29--hero-section-display-on-mobile-375px)
  [TC31 – Services Section Display on Mobile (375px)](Test-Cases.md#tc31--services-section-display-on-mobile-375px)
  [TC33 – Diploma Carousel Section Display on Mobile (375px)](Test-Cases.md#tc33--diploma-carousel-display-on-mobile-375px)
  [TC35 – About Me Section Display on Mobile (375px)](Test-Cases.md#tc35--about-me-section-display-on-mobile-375px)
  [TC37 – Contacts Section Display on Mobile (375px)](Test-Cases.md#tc37--contacts-section-display-on-mobile-375px)
  [TC39 – Footer Display on Mobile (375px)](Test-Cases.md#tc39--footer-display-on-mobile-375px)

**Environment:**  
- Browser: Edge 140  
- Resolution: 374–376px (DevTools)
- Device: iPhone SE / iPhone 13 mini (emulated)
- OS: iOS 17  

**Description:**  
According to design specs, mobile layout starts at 375px width. In reality, the mobile layout renders correctly only at 374px and below. From 375px and above, the layout collapses and elements overlap, resembling a broken tablet layout.  

**Steps to Reproduce:**  
1. Open the website in Chrome DevTools.
2. Set viewport width to 374px → observe correct mobile layout.
3. Increase viewport to 375px or larger.
4. Observe layout changes. 

**Expected Result:**  
- Mobile layout should be applied from 375px and below exactly as per design.
- No overlap or broken alignment should occur at 375px and above until next responsive breakpoint. 

**Actual Result:**  
- At 375px and above, mobile adaptation fails.
- Layout shifts into incomplete desktop/tablet view: menu items misaligned, text overlaps.

**Severity / Priority:**  
- Severity: Critical
- Priority: High 

**Attachments / Screenshots:**  
![BRo2](/Bug-Report%20Attachments/BR02.mp4)  

**Notes / Additional Info:**  
- Possible issue with media query breakpoint defined as max-width: 374px instead of max-width: 375px.

- Problem consistently reproducible across Chrome, Edge, and FireFox.
