> It can be difficult to understand data insights by examining individual data points or a table of information. Often, insights become more obvious when presented in an effective visual format. You can use data visualization (often called  “data viz”) techniques to help your audience interpret data in a concise, visual manner.

```
When creating data visualizations, you must strike a balance between presenting enough information for your audience to understand the meaning of the visualization and not overwhelming them with too much detail. In this reading, you’ll learn tips and techniques for crafting visualizations that are both impactful and effective. You’ll explore:
```

- Two frameworks for organizing data
    
- Pre-attentive attributes
    

## Frameworks for organizing your thoughts about visualization

Frameworks help organize your thoughts about data visualization and give you a useful checklist to reference as you plan and evaluate your data visualization. Here are two frameworks that employ slightly different techniques. Both are intended to improve the quality of your visuals. 

[The McCandless method](https://www.informationisbeautiful.net/visualizations/what-makes-a-good-data-visualization/)

You learned about the David McCandless method earlier in the course; as a refresher, the McCandless method lists four elements of good data visualization: 

1. **Information:** the data with which you’re working 
    
2. **Story:** a clear and compelling narrative or concept
    
3. **Goal:** a specific objective or function for the visual
    
4. **Visual form:** an effective use of metaphor or visual expression
    

The McCandless method provides terminology that isolates the specific elements of a graphic, allowing the person making a visual the ability to evaluate how well those criteria have been met. The aim when crafting a visualization is to incorporate all four elements effectively. Visualizations that fail to incorporate all four elements can be ineffective at communicating insights in various ways. For example, visual form without a goal, story, or data could be a sketch or even art. Data in visual form without a goal or function is just a pretty picture. Data with a goal but no story or visual form can be boring. All four elements need to be present to create an effective visual.

[Kaiser Fung’s Junk Charts trifecta checkup](https://junkcharts.typepad.com/junk_charts/junk-charts-trifecta-checkup-the-definitive-guide.html)

This approach is a set of questions that can help consumers of data visualization critique what they are consuming and determine how effective it is. You can also use these questions to determine if your data visualization is effective:

1. What is the practical question? 
    
2. What does the data say?
    
3. What does the visual say? 
    

Each of these questions offers an opportunity to investigate a given problem with a slightly different context. A well-designed visual effectively answers all three of those questions at once. Moreover, this framework helps you think about your data viz from the perspective of your audience. 

## Pre-attentive attributes

In addition to the frameworks mentioned above, several standard building blocks can help you construct your data visualizations. Creating effective visuals means leveraging what is known about how the brain works, and then using specific visual elements to communicate the information effectively. Pre-attentive attributes are the elements of a data visualization that people recognize automatically and without conscious effort. The essential, basic building blocks that make visuals immediately understandable are called marks and channels. 

### Marks

**Marks** are basic visual objects such as points, lines, and shapes. Every mark can be broken down into four qualities:

1. **Position:** Where is a specific mark in space relative to a scale or to other marks? 

For example, if you’re looking at two different trends, position allows you to compare the pattern of one element relative to another. 

![simple line chart with two lines. One is red and one is blue, and there is obvious space between them.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/w13YHmt8QaiMlhM_FMoQnA_20fa0b545f3d43779dad888c4eab81f1_PoHaiHktPbMb89eEc9Vpp-UE_BTfwzjST1tLbw1_3HOQ7m0bSk9A2t7Bv-w7nM_57RH4dUH92FkOsuNe0RN6mlu15J8WF1WP3NuoToX7QUOd2UCGjzosjgeeaPnG_gaVxJm4rOoCc5r-ApSOG6ZdPiw?expiry=1721260800000&hmac=NYavPUb8y3BEcNzSo7mBNIj0GOFNcSirWtlJYJmfEsU)

2. **Size:** How big, small, long, or tall is a mark?

The comparison of object sizes can be an easy visual interpretation for humans. This can be very useful for conveying the relationship between categories or data points. However, this also presents a potential problem: The human eye can inadvertently interpret comparisons that aren’t intended to convey meaning. For example, sometimes objects that appear to be the same size when they are not. Controlling the scale of a visual is important even when comparative sizes are not intended to offer information.

![A plot with points that are different sizes.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/G1By0iKbT6S20RyOJOLakw_8e3b96d8d62b41dab3a0e9b037da2cf1_GODjKcAHrADKXJsRxDT2itjTl9NO4ism_dt63kvp6YzrO7aIUOhVjyUscltPeyX2XNlXJwyEOGz1ibCd7JZXTnAlcjVB3Wvtfjcszugj1WSA4XWqoGP-UHGlrlC54ZNksUkdKtXHlg6Wg7AD_HJMgZU?expiry=1721260800000&hmac=cyqRqTD9SU771Hc6TjK5cm4xwos1Ydl3lnoYD4UhTSE)

3. **Shape:** Does the shape of a specific object communicate something about it?

Rather than using simple dots or lines, a bit of creativity can enhance how quickly people are able to interpret a visual by using shapes that align with a given application. In the example below, it is immediately obvious that numbers of people are represented because the bars are person-shaped. 

![horizontal bar chart, but bars are made of icons shaped like people](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/vIWV0cFASZG52lgye2TkcA_32e7afe4ba304c8db5d3dd396a1e5ff1__mfHWWDLd73KXZcCE8V0tPKY1iltunaMx63y5jMoIXySA0-d1Hx40MZctiQIlt2yZNTr_r0wp3NRjDA7L8mrPRJPZls-ta5RPIeDbYssZMDiLrfWolXOXKF5kkY67YPr8WfkgMzxZK-WNlB53g-_rIU?expiry=1721260800000&hmac=wEEWe_6RYOyG7CnJT8eKFAGcgYsdWEuHXNceafaDHxk)

4. **Color:** What color is a mark?

Colors can be used both as a simple differentiator of groupings or as a way to communicate other concepts such as profitable versus unprofitable, or hot versus cold. 

![a bar chart with a red, green, yellow, grey, and blue bar](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/i6Lpsc88RzeYrF-r61-lkA_c9ee968f09d24a33849524397a00a7f1_uWZn95j6KM0A4os33IazLDL0nNrpIix7WMtlZ_4sb9HafOB0G4kVuQ7vR0oXEhn9WVnLkCKj8sAMffZKaZHSN7z6gkgcLfK1plWtwxXdaFWB5mnMii8lgVewDtq6DRmzDad_9yzAFpQ1kFoGm12aWE8?expiry=1721260800000&hmac=2LfFfw3o0Aqsn3InyfAnEtrj69FBXWvqYIfGz3wv_Q0)

### Channels

**Channels** are visual aspects or variables that represent characteristics of the data in a visualization. They are basically specialized marks that have been used to visualize data. It’s important to understand that channels vary in terms of how effective they are at communicating data based on three elements: 

1. **Accuracy:** Are the channels helpful in accurately estimating the values being represented?

For example, color is very accurate when communicating categorical differences, such as apples and oranges. But it is much less effective when distinguishing quantitative data, such as 5 from 5.5.

![a plot with apples and oranges representing the data points](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Wf6s1QnXRXSjIqWek_8Sag_d7aefd5069c34982bb9e2b6ee00083f1_eddRCinr1PXCxLOOT7ouF1uWgWXoPJsomsNUfjno7rJ4AT4IDk10Elhyvr8HX8wIfxIj2Xj0ATEHcGv26wenha8PMqjkWo3UnZOToCze3iWgzhZx9_a6Zth5fSPHR7wC6fKxY0B4ICh9jHbLyB4L0QI?expiry=1721260800000&hmac=pDUJZADlNdYnVegEuhrVVRFRWd_WiPrbO6QLqcYhlUc)

2. **Popout:** How easy is it to distinguish certain values from others?

There are many ways of drawing attention to specific parts of a visual, and lots of them leverage pre-attentive attributes including line length, size, line width, shape, enclosure, hue, and intensity.

![a line chart with three blue lines of different shades, and one red line](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sxYBbaJKSsuP4_7UcjOeew_d8c55324fda24a5c9f4d53f59c393df1_9V9JqTSQJKOQ5Gn-fkp-ZmJILLWBHwvKOJGFXhrBXs2Vo2mOVUENTLqJbs9nQucXedmVprZ_EhmZz2JBTYTVpfWtSGDqfUaEOxP0Bm8TUwbKYLwjPwd4zpbL2AFUQJZ3xKKfrNqDoY8ofGqkPvqaI3Y?expiry=1721260800000&hmac=m61j7OYzvH0un1Q5qUBETMnbrA51zh4h6czIXg0RxnQ)

3. **Grouping:** How effective is a channel at communicating groups that exist in the data?

Consider the proximity, similarity, enclosure, connectedness, and continuity of the channel.

![bar chart with four groups of bars. In each group, there is a red bar and a blue bar](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/YVCqvj29RueUw-qbXakeiQ_55494966d85946208cb20fa514cddcf1_clRwSjOaDIJfbIETWvYtnENapMqisUqPNl6ZOpdVKMyD8UwKbulM6NodwVe3N_ePiuwzGm9qbaWSS10vHgnhAeICBrN5j4sDpO931SkKSriacYXA8OHcb3XYkyZzsrV5jD1x-CMXSxQ0ps1cOD0oEv8?expiry=1721260800000&hmac=ctKzjgHx6hTjBHA97sT-quFdeNV4wZNSSKQTZP-UuQI)

But, remember: The more you emphasize one single thing, the more that counts. Emphasis diminishes with each item you emphasize because the items begin to compete with one another.  

## Key takeaways

Throughout your career as an analyst, you will use different techniques and types of data visualizations to present data and insights in a concise, impactful manner. This will include organizing your data, selecting the right type of data visualizations, and designing them  in such a way that they are easy to understand and highly communicative while avoiding any visuals that are misleading or inaccurate.

Keep in mind that data visualization is an art form, and it takes time to develop these skills. Over your career as a data analyst, you will  learn how to design and evaluate data visualizations. Use these tips to think critically about data visualization—both as a creator and as an audience member.

## Resources

- [The beauty of data visualization](https://www.ted.com/talks/david_mccandless_the_beauty_of_data_visualization?language=en#t-150183): In this video, David McCandless explains the need for design to not just be beautiful, but for it to be meaningful as well. Data visualization must be able to balance function and form for it to be relevant to your audience. 
    
- [‘The McCandless Method’ of data presentation](https://artscience.blog/home/the-mccandless-method-of-data-presentation): At first glance, this blog appears to be written by a David McCandless fan, and it is. However, it contains very useful information and provides an in-depth look at the 5-step process that McCandless uses to present his data.
    
- [Information is beautiful](https://informationisbeautiful.net/): Founded by McCandless himself, this site serves as a hub of sample visualizations that make use of the McCandless method. Explore data from the news, science, the economy, and so much more and learn how to make visual decisions based on facts from all kinds of sources. 
    
- [Beautiful news](https://informationisbeautiful.net/beautifulnews/): In this McCandless collection, explore uplifting trends and statistics that are beautifully visualized for your creative enjoyment. A new chart is released every day so be sure to visit often to absorb the amazing things happening all over the world.
    
- [The Wall Street Journal Guide to Information Graphics: The Dos and Don'ts of Presenting Data, Facts, and Figures](https://www.amazon.com/Street-Journal-Guide-Information-Graphics/dp/0393072959): This is a comprehensive guide to data visualization, including chapters on basic data visualization principles and how to create useful data visualizations even when you find yourself in a tricky situation. This is a useful book to add to your data visualization library, and you can reference it over and over again.