---
layout: post
title: "Lab 6: Figuring Out Vertabello & LucidChart"
author: Fin Lockert
categories: misc
---

This week's lab marked a significant transition from familiar territory to new horizons. As I learned how to use Lucidchart and Vertabello for creating Entity-Relationship Diagrams (ERDs), I encountered  challenges and advantages.

**1. The Shift from Lucidchart to Vertabello**

At the outset, Vertabello was a bit disorienting. In Lucidchart, I got used to using oval shapes to represent entity attributes, providing a clear visual distinction. However, Vertabello took a different approach, and I had to adjust to the absence of these ovals. It was a minor hiccup but one that required a shift in my thinking.

![Vertabello Schema](/assets/images/schema.jpg "Vertabello Schema")

**2. Understanding Data Limits and M/PI**

One of the immediate challenges was determining the appropriate text limit for attributes. In Lucidchart, this wasn't a concern, but Vertabello required me to set a limit. Deciding on the right number was of a huessing game than anything else; it required considering the potential length of data for each attribute.

Additionally, I grappled with the concepts of "M" (Mandatory) and "PI" (Primary Key). While I understood their importance in database design, I found it challenging to pinpoint when to mark an attribute as "M" or "PI." It's a critical decision, as it dictates data integrity and uniqueness. Not to mention, at the beginning, I had no idea what those checkboxes even meant.

**3. Vertabello's Hidden Advantages**

Despite these initial hurdles, I slowly found the advantages of Vertabello. The ability to view detailed information about each attribute without cluttering the diagram was a game-changer (putting any more amount of detailed info into LucidChart feels daunting, and like it would make the whole thing look horrible). It made it easier to understand the nuances of the data model at a glance, something I'm not sure I could've done in LucidChart.

![LucidChart Diagram](/assets/images/erd.jpg "LucidChart Diagram")

**4. Diamond-Shaped Relationships**

One notable difference in Vertabello was the non-use of diamond shapes to represent entity relationships. Admittedly, I opted not to include them in my LucidChart diagram because I was uncertain about their placement and worried they might complicate the visual representation. However, I understand that they play a crucial role in defining relationships, and I plan to explore their usage in future projects.

As for why certain things were markes as PIs, Ms, or neither:
1. **Primary Keys (PI)**:
   - The IDs: The IDs for each entity were designated as a Primary Keys because they serve as a unique identifier for each entity (owner, manufacturer, customer, etc.). Each entity should have a distinct ID, ensuring data integrity and enabling efficient data retrieval.

2. **Mandatory (M)**:
   - Name (Customer and Owner): Names of customers and owners were marked as Mandatory because they are essential pieces of information. Every customer and owner must have a name.
   - Email (Customer and Owner): Email addresses were designated as Mandatory for both customers and owners. This ensures that contact information is always available and valid.
   - OrderDate: OrderDate was marked as Mandatory because every order must have a date associated with it. It's a fundamental attribute for tracking orders.
   - OrderStatus: OrderStatus was designated as Mandatory because it represents the current status of an order, and it's vital to know the status of each order in the system.

3. **Neither**:
   - Description: The Description attribute for items was not marked as Mandatory or as a Primary Key because it represents additional information about the item. While it's valuable for providing details, it may not be required for all items, and multiple items can have the same description.
   - QuantityAvailable: QuantityAvailable was not marked as Mandatory because it can vary for different items. Some items may have limited availability, while others may be in abundant supply. It's not inherently mandatory for every item.
   - ManufacturerName: The ManufacturerName attribute in the Manufacturer entity was not marked as Mandatory or as a Primary Key because it represents information about manufacturers. While it's valuable for identifying manufacturers, the ID will suit that job better.

This attribute designation rationale ensures that the database schema accurately reflects the data's nature and requirements, promoting data consistency and usability.

The selection of attributes as Primary Keys, Mandatory, or neither is driven by the necessity of each attribute to uniquely identify records, its essentiality in the context of the entity, and the variability of the data it represents. These designations aim to maintain data integrity and facilitate efficient data management in the online grocery shopping web application. As for why the Primary Keys are also marked as Mandatory (even if it may seem redundant), it was something the Vertabello required.

In summary, lab 6 introduced me to Vertabello, a powerful tool with its own set of conventions and nuances, and LucidChart, which I think while having less info is easier to understand at a glance. While they presented some initial challenges, I can already see their potential for creating more comprehensive and informative ERDs. As I continue to work with Vertabello and LucidChart, I aim to get better at defining mandatory attributes and primary keys with confidence, unlocking its full potential.

Looking forward to the learning journey ahead!