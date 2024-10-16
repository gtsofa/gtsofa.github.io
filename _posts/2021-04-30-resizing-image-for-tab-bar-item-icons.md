---
layout: post
title: "Resizing image for Tab Bar item icons"
comments: true
tags: iOS, UITabBarController, Xcode.
excerpt_separator: <!--more-->
---

I was struggling to add images to each of my tab bar items. This is common to iOS devs where they find themselves not knowing what to do when making icons for apps that have a Tab bar controller. An image you like has a size that is much bigger than the area of the bar item you need to display on your app. 
<!--more-->

This is the hack that I found to be good and easy after doing my research.


Prepare 3 image icons for each tab bar item as per Apple’s [Human Interface Guidelines](https://developer.apple.com/design/human-interface-guidelines/ios/icons-and-images/image-size-and-resolution/) website.

For resizing the image, follow the steps below.

1. Create a name for your image for the particular icon in *Assets.xcassets* folder.
2. Add your image to the 1x, 2x, and 3x boxes in *Assests.xcassets* folder.
3. Click on the image in each box and right-click which should reveal the options and select the option as highlighted on the screenshot below:

![Open with Editor Explorer](/assets/img/images-resize-tab-bar-icons/section-1.png "Open with Editor Explorer")

4. When you click `Open with External Editor` a preview will be shown to you.

5. Click on Tools` then Adjust Size` as shown below.

![Adjust Size..](/assets/img/images-resize-tab-bar-icons/adjust-size.png "Adjust Size")

6. Adjust the size of your image based on your requirements while keeping in mind Apple’s human interface guidelines. Save your changes and close the window. The image in Xcode should be auto-updated. Repeat the steps for each individual icon in the 1x, 2x, and 3x sections.

Thanks for reading, I hope it helps you. Happy hacking :-)


