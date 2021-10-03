# A very common website feature

This exercise is to recreate a section that is found on many informational websites.

For this one you will need to edit the HTML a little bit too. We can't be making things _too_ easy for you. You'll want to add containers around the various elements so that you can flex them. Good luck!

## Desired outcome

![desired outcome](./desired-outcome.png)

### Self Check

- All items are centered on the page (horizontally, not vertically)
- Title is centered on the page
- 32px between the title and the 'items'
- 52px between each item
- Items are arranged horizontally on the page
- Items are only 200px wide and the text wraps
- Item text is centered

Analysis:

I created a different class for each plant item. I understood that each plant item would have the same styling, so I consolidated the styles under multi class rule using a unique class for each plant item. Instead I could have applied those styles to the .plant-list container since all plant items would inherit from there. This would work since their stylings were identical.

I did not need to turn the 'information' div into a flex box. A simple'text-align' property on the body would have allowed me to center this text. This would also have eliminated my need to add text-align to the plant items (redundant style). The text-align property would have been inherited from the parent body style container.

I used a flex-wrap: no wrap styling on the plant items so that the text would be under the icons. If I remove it, the text appears to the right of the icon. I could not think of a better way to do this. However, this is achieved in the solution css without using flex-wrap: wrap.

Bottom line is that there is a lot of redundant styling in my cade. The solution consolidated all of this redundant code by taking advantage of cascading. All of the elements (other than the title) were wrapped in a container that had all of their common stylings (display:flex, align-items, justify-content, gap).

Despite the redundancy, my code got the job done. The appearance and functionality is as required by the README specs.

