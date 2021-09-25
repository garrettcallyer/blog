---
layout: post
title:  "Entity Relationship Reflection"
author: Garrett Collier
date:   2021-09-24 08:23:00 -0500
categories: Database and Entity Creation
---
Some assumptions I made when creating the chart and database based around the description included:
 - Giving the Owner and Customer their own personal primary key ID as entities  
 - Making Order an entity with the ability to have all the substitution and special instruction parts in the attributes of the table

As for my pictures directly, I tried to piece together the relationships and references in a way that would allow the order and items the ability to access one another to then be able to update and change the quantity values when an item is purchased and finalized as sold.

Are you satisfied with your resulting data representation?<br>

For the most part yes, I wish their was an easier way to reference items in the UI, so that I could give owners, items, and orders access to the item_id row, but I couldn't figure that piece out. I think I did the best I could with what I was able to use. I wish I had come up with a better way to distinguish between finalized and ongoing orders, but nothing made sense other than this.

What are some complications that you could encounter implementing this model?<br>

A primary and foriegn key issue with the pieces explained above. The website would only make sense to me if item_id was like a global parameter or variable that anyone could access. That way everyone could access an item and see how much of it was left. I think another issue that could arise would be the pickup and delivered data types and just how much the order entity has to keep track of. I couldn't figure out an easier way to account for all the ways to get the groceries, the instructions for the groceries, the time and date of the order when finalized, as well as the substitution of different items. This may cause issues with space and put a burden on a single entity, but I also may be overthinking the process if I were to implement this.

![Vertabelo Database]({{site.baseurl}}/pictures/Vertabelo.jpg)

![Lucidchart Entity Relationship]({{site.baseurl}}/pictures/Lucidchart.jpg)
