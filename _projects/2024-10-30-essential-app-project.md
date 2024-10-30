---
layout: project
title: "Essential App (iOS)"
comments: true
tags: iOS, Xcode.
excerpt_separator: <!--more-->
---

Essential App is designed to deliver a great user experience for users sharing their image feed with their friends.

The app was conceived as a platform that I can use to learn and apply the fundamentals of software development which are independent of the language or platform we use that include: modular design, automated testing, dependency management, codebase health monitoring, short release cycles, effective version-control, excellent cross-team communication as shared by Essentials Developer Academy by Caio and Mike.
<!--more-->

It uses UIKit, Core Data, and more==

This is the hack that I found to be good and easy after doing my research.


Prepare 3 image icons for each tab bar item as per Apple’s [Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/image-size-and-resolution/) website.

For resizing the image, follow the steps below.

- Create a name for your image for the particular icon in *Assets.xcassets* folder.
- Add your image to the 1x, 2x, and 3x boxes in *Assests.xcassets* folder.
- Click on the image in each box and right-click which should reveal the options and select the option as highlighted on the screenshot below:

![Open with Editor Explorer](/assets/img/images-resize-tab-bar-icons/section-1.png "Open with Editor Explorer")

- When you click `Open with External Editor` a preview will be shown to you.

- Click on Tools` then Adjust Size` as shown below.

![Adjust Size..](/assets/img/images-resize-tab-bar-icons/adjust-size.png "Adjust Size")

- Adjust the size of your image based on your requirements while keeping in mind Apple’s human interface guidelines. Save your changes and close the window. The image in Xcode should be auto-updated. Repeat the steps for each individual icon in the 1x, 2x, and 3x sections.

Thanks for reading, I hope it helps you. Happy hacking :-)


