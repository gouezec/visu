# Summary
My visualization presents the proportion of survivors from the Titanic catastroph.
The key messages I want to communicate through the visualization are:
- women better survived in proportion than men,
- boys below 10 years better survived in proportion than rest of the men,
- passengers from first class better survived in proportion than the rest of the passengers.


# Design
## Initial design choices
I chose to build a chart that shows at the same time data for women and men. 
This enables readers to compare survival chances between women and men which is a key message.
I decided to display survival rates in percentage because absolute values do not take 
into account the unbalance in number of passengers between women and men.

I chose the bubble plot instead of a line plot because there is no interest to show the evolution
over all the age ranges. The only interesting evolution to notice is between the range 0..10 and the others.
I estimated that it did not justify to use a line plot.

The bar chart would be an intereting alternative but I judged the visualization of 2 side bars (one for each sex)
less easy to read than two bubbles on the same axis. And with an animation, seeing moving bubbles is greater than
bars growing or contracting.

For the legends, I just activated the legend display offered by dimple.js.

I selected the pink color for plotting the women bubbles and blue for the men ones because it is a quite conventional
association, at least in France.

## Changes made after collecting feedbacks
Here are the changes I made after collecting the feedbacks:
- I changed the color for the women. The pink was judged a bit sexist. I change it to a light red (Tomato) in order to have
a more neutral association, red vs blue.
- I changed the range labels for the x-axis by explicitly noting the range as "10..20" instead of "20". The initial choice
was judged too ambiguous.
- I added an activation of the mouse pointer when moving over the buttons which let select the passenger class.
- I changes the color of the passenger class buttons.
- I moved all the buttons and legends on the right.
- I completed the tooltip on bubble to add the total number of passengers in the category.
- I improved the legends by zooming in the color legend and by adding a legend about the meaning of the circle size.

One feedback claiming "2 circles are superimposed, we only know when we change category." was not taken into account.
I  did not know how to change it in dimple.js and I judged it not critical as there is only one case and the key messages
are not affected by this limitation.

# Feedback
To collect feedbacks, I hosted my visualization on GitHub and I submitted it by email to all my colleagues in the same 
company department as me.
There are roughly 90 people in the departement.
I asked 3 questions:
1. What message(s) did you understand?
2. What do you like?
3. What could be changed?

I received 30 answers. The answers are mostly written in French as lots of my colleagues are French.
Hereafter I included 6 feedbacks only to not get the summary too long. These feedbacks are a quite good 
summary of the various feedbacks I got, mainly in terms of improvement.

## Feedback 1
Original English feedback.
> Hi Frederic,
>
> The key messages which I have picked up on are:
> -	It’s best to avoid 3rd class when travelling by Titanic. It’s worth spending that little bit extra.
> -	Women are more skilled than men at getting into life rafts, irrespective of age.
> -	I must be nearing retirement, as the majority of people on that boat were younger than me.
>
> I particularly like the dotted lines which appear when you hover over a circle – nice touch.
>
> I don’t see how you could possibly improve on this piece of work – outstanding.

## Feedback 2
Original English feedback.
> Message understood:  At first glance, most women between 20 and 40 survived.  All females between 60 and 70 survived.  All males over 70 perished.
>
> What do I like:  The extra information given when focus is places on the circles
>
> What would I change: Get rid of the class rectangles on the left, it pollutes the graph and does relate to any information given.

## Feedback 3
Translation from French with Google Translate.
> There are more women who have survived than men
> Passengers of the 3rd class have survived less than those of the other classes
> A priori no correlation between survival chances and age
>
> It's dynamic, it sounds synthetic although a priori there is plenty of data behind
>
> I'm not sure I understand what the size of circles is
> Women in pink men in blue can bring remarks on storks, cabbage and roses

## Feedback 4
Translation from French with Google Translate.
> Hello,
>
> On the menu on the right, not easy to know that you have to click to change category.
> Nice presentation by bubbles
> Message = it respects women and children pretty well first!
> To change: when 2 circles are superimposed, we only know when we change category.

## Feedback 5
Translation from French with Google Translate.
> Hello,
>
> The message that I understood is that it is better to be in first class to have more chances to survive a shipwreck,
> and if the color code matches the sex of the passengers (not specified), it is also better to be a woman or a child.
> What I like is the different views ("all", "1st class", etc ...), and what should be improved is to add a legend of
> the color code (man = pink and woman = blue , that's it?) and the meaning of the different sizes of circles to 
> avoid having a doubt (number of passengers I imagine).

## Feedback 6
Translation from French with Google Translate.
> What message (s) did you understand?
>   A rich woman is far more likely to have escaped than a poor man ...
> What do you like?
>   - animations to change filters & bubble info
> What could be changed?
>   - The legend of the age scale is missing (we can guess thanks to the bubble info)
>   - The cursor on the filter buttons looks like the text edit mode, a hand to show that it's clickable would be more
>	- The pink color for women can be considered sexist 
>   - A way to directly visualize the percentage of survival (ex: color + dark) bring info directly without having to go through the info bubbles

# Resources
- https://github.com/PMSI-AlignAlytics/dimple/wiki
- http://learnjsdata.com/group_data.html
- https://www.w3schools.com/colors/colors_names.asp
- https://www.w3schools.com/css/
- https://translate.google.fr/?hl=fr
