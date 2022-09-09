# Foldable Phones: The Next Golden Era of Smartphones

</br>

Once the golden era of the mobile phone design was known to be the flip era, today that golden era is back again but slightly different with the foldable smartphones. Companies that have dominated the global market of smartphones such as Samsung, Motorola, Huawei have already released their rendition of the foldable smartphones, that have received quite good reviews across the board. However, with this new advancement in smartphone design has invited all new challenges for the developers down the line. 

<p align="center">
  <img src="https://fdn.gsmarena.com/imgroot/news/18/11/samsung-foldable-phone-render/-640/gsmarena_002.jpg" width="80%" />
</p>

New developers breaking into the scene, the veterans of old and any individuals who want to dip their toes in the field of app development are wondering how to design for this new line of smartphones. Since there is a change to the assembly of the phone, so will the well-established rules of development.

## What are foldable phones?

Foldable phones are smartphones that is capable of folding or rolling up. When the smartphone is unfolded, it opens to a much larger screen that gives the user more functions. And when the device is folded up, it takes a much smaller form, easily fitting into one's pocket. Considering the trend of the smartphone market in the last few years where the primary changes were a larger screen size and updated camery, battery and processor, this could be considered an innovation among mobile devices. 

## The rise of the foldable phone

Foldable phones have succeeded in rapidly taking over the market. A report from IDC shows that 7.1 millions units were shipped last year - which is a significant increase from the 1.9 million units shipped in 2020. Tech analysts predict that foldable phones phones will reach over 27 million units with a valuation of $29 billion by the year 2025.

**Worldwide Foldable Phone Shipments, Market Share, and Growth Forecast** (shipments in millions of units)

| Form Factor | 2021 Shipments | 2021 Market Share | 2025 Shipments | 2025 Market Share | 2020-2025 CAGR |
|-------------|----------------|-------------------|----------------|-------------------|----------------|
| Foldable    | 7.1            | 0.5%              | 27.6           | 1.8%              | 69.9%          |  
| Smartphone  | 1341.8         | 99.5%             | 1491.3         | 98.2%             | 3.1%           |  
| Total       | 1348.9         | 100.0%            | 1518.9         | 100.0%            | 3.5%           |   

Source: IDC, Worldwide Foldable Smartphone Forecast, 2021-2025, Feb 2022.


All of these stats are leading towards one fact, that is, we will have to "fold" in the near future of this industry. 

## Features of the successors
There are a number of features of this device that make it ideal for consumers and it is important that we go through them in the list below. 

* First, it is their flexible form factor. Depending on the design, these smartphones can have up to 3 folds, making it convenient for the user to make quick work of it as a smartphone or tablet. 
* Secondly, it offers more screen real estate over the traditional smart phone. Even though most of the newest smartphones offer multitasking windows, the smaller display can be a hindrance for users. The larger display plus the split screen feature would allow individuals keen on multitasking to increase their productivity by tenfold.
* The larger arhitecture of this phone will allow manufactures to add bigger and more powerful hardware, which in turn, means a significant leap in performance. 

To summarize, the features are exceptional, the expectations are high and the challenges will be great. Now, let us look at how one can go ahead and prepare to develop applications for this next era of smartphones. 

## Developing applications in the future

Let us finally look at what we should keep in mind as developers when creating an app for foldable smart phones

**Screen Continuity:** Seamless transition in screen before and after folding. To ensure a great user experience, during the transition from fold to unfold, the app will receive the configuration change. 

<p align="center">
  <img src="https://github.com/ehsanul18/foldable-phone/blob/main/image/fold-unfold.gif" width="80%" />
</p>

For this, the developer needs to make sure the app properly supports runtime configuration changes. For example, the following manifest code declares an activity that handles both screen orientation changes and keyboard availability change:

```
<activity android:name=".MyActivity"
          android:configChanges="orientation|screenSize|screenLayout|keyboardHidden"
          android:label="@string/app_name">
```

For the best experience, when screen size changes due to the folding transitions, declare `resizeableActivity=true` in the manifest.

**Multi-Resume:** All the activities in the split-screen of the foldable phone needs to be in the resumed state during any orientation. This was not initially available for the Android Pie but have since been added with Android 10 onwards. 

<p align="center">
  <img src="https://3.bp.blogspot.com/-mNHMGh4asB0/W-XBw1gNfUI/AAAAAAAAGFg/SGRaye6CwUwJUTck925c3o7TCt9ov9QggCLcBGAs/s1600/image1.png" width="80%" />
</p>

**Multi-Display:** A foldable phone offers 2 displays, Folded (Cover) and Unfolded (Main) display. 

Support for enhanced display had been included from Android 8.0 onwards. Applications with activity supporting multi-window mode allows the user to move the display from one activity to another. 

`ActivityOptions` provides two new methods to support multiple displays: `setLaunchDisplayId()` which specifies which display the activity should be shown on when it is launched and `getLaunchDisplayId()` which returns the activity's current launch display.

**Resizeable App:** The user interface needs to be designed in such a way that it handle multi-window mode and dynamic resizing which can done as mentioned previously by setting `resizeableActivity=true`. This can then be tested using a foldable phone or emulator. 

<p align="center">
  <img src="https://mobidev.biz/wp-content/uploads/2020/01/foldable-fold-out-resize.png" width="80%" />
</p>

## Conclusion: Where we go from here?
The steps thats needs to be kept in mind while developing for a foldable phone applies to the Ethereum balance retrieval app that I am currently developing. As mentioned before, I need to ensure the current and future features works properly in multi-display mode and adjusts to dynamic resizing. 

Current statistics show the growth of the foldable phones in the next few years. With time, these devices will surely be more advanced and offer a much wider range of features. So, it is high time now to develop for the future to reap the benefits when the market hits the inevitable peak.
