
**Create a Watch Face With Tag Expression in Watch Face Studio – Easy & Simple**

<img width="468" alt="image" src="https://github.com/user-attachments/assets/95411946-8489-49c4-beb5-1b75b2272874" />

![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.001.png)

Designing watch faces for Wear OS devices is simple, especially thanks to Samsung’s Watch Face Studio. This platform provides the opportunity to build a custom watch face design. Anyone can easily create watch faces. Watch Face Studio also offers Tag Expressions, which allow designers to add dynamic elements to their watch faces. In this guide, we will learn how to make a watch face from scratch, as well as how to use Tag Expressions to build a watch face in an easy manner. If you're a watch face enthusiast, then this article is for you—you're in the right place.

*First, we need to understand the basics of Watch Face Studio, then move on to using Tag Expressions to build a dynamic watch face.*

<img width="468" alt="image" src="https://github.com/user-attachments/assets/5c56759b-65ad-4a2d-96c2-4d3cba03a9a6" />


![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.002.png) 

At the top of the menu bar, you’ll see an option to "Add Component." This option allows you to add text, index, progress bar, analog clock, digital clock, and many other elements. It’s quite easy to add an index or a watch hand for minutes, seconds, or hours. You can also add a digital clock from here. In the "Add Component" section, there’s also an option for the "Complication Slot." From here, you can add a circle, shape, or progress bar in an organized manner. Once ![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.003.png)that’s done, your clock will be ready to start ticking the time.

<img width="291" alt="image" src="https://github.com/user-attachments/assets/88691f89-8be2-46c0-a952-5ce39698e8f1" />

What Are Tag Expressions?

Tag Expressions are tools in Watch Face Studio that help you add interactive and dynamic features to your watch face. Tags pull real-time data from the smartwatch, like battery percentage, step count, or time. You can combine these tags with conditions to make your design respond to changes.

*You will find many tags in the options. These tags are used to control watch data, such as the date, time, battery status, or steps.*

<img width="468" alt="image" src="https://github.com/user-attachments/assets/c28822cb-d9d5-41c0-99ae-0c81846797b2" />


![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.004.png)![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.005.png)Let’s use a tag to manipulate the battery percentage. You’ll scroll down to find the tag [BATT\_PER]. This tag controls the opacity of the selected item on the watch face and changes dynamically according to the battery percentage.

<img width="469" alt="image" src="https://github.com/user-attachments/assets/9fd527c5-4a7b-4d40-a414-2561bab6a46e" />

Let’s write a condition:

**[BATT\_PER] <= 15**

If the battery percentage is less than or equal to 15%, **[BATT\_PER] <= 15** will be true and return 1. If the battery percentage is greater than 15%, **[BATT\_PER] <= 15** will be false and return 0.

Now, if you want to remove the green light from the battery when the battery percentage is less than or equal to 20%, what should you do? 

![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.006.png)
<img width="333" alt="image" src="https://github.com/user-attachments/assets/6a7f6e58-0c74-4f7c-a220-e63c72d96704" />

You can write a condition in the tag section like this:

**[BATT\_PER] <= 20 ? 0 : 100**

What does this mean? It sets the condition that if the battery percentage is less than or equal to 20%, the opacity will be set to 0, effectively removing the green light. If the battery percentage is greater than 20%, the opacity will be set to 100. That’s it! 

You can write many more tags like this. Same as the red light. You can find more tags in here [Tag Expressions!](https://developer.samsung.com/watch-face-studio/user-guide/tag-expression.html)

![](Aspose.Words.e33cce68-31ca-46de-adeb-dabfc574b291.007.png)
<img width="289" alt="image" src="https://github.com/user-attachments/assets/324d3f4d-561a-49fc-aecb-37b4802ba853" />

After designing your watch face, you can test and preview it. Click Run in Watch Face Studio to preview your design. Use the simulator to test how the battery indicator behaves at different levels. Refine your design as needed to ensure everything looks and works perfectly.

Watch Face Studio is Fun!
