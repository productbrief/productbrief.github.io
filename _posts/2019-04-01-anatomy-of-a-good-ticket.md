---
layout: post
title:  "Anatomy of a Good Ticket"
author: ryan
categories: [ user-story, requirements, writing ]
image: https://s3.amazonaws.com/ryanhaber/productbrief/content/images/take-a-number.jpeg
featured: true
hidden: false
---

<style>
    table, th, td {
    border-collapse: collapse;
    border: 3px solid #bbdefe;
    padding: 5px;
    margin: 5px;
}
</style>

*tl;dr*: A good ticket is clear, correct, complete, and concise. It uses straightforward grammar, includes background information to aid good decision-making, and sets clear expectations. A good ticket is neither too big nor too small.

# The Problem

Unless you are a single developer writing code to solve your own, individual problem, the people who want the software are not the exact same set as those who make it. As a result, communication is necessary between the set of wanters and the set of makers. And the greater the size of the sets and the less they overlap, the more crucial it is to have clear written communication to avoid wasted effort.

# The Solution

Work requirements usually get broken down into tickets. These tickets can be seen as atomic or, perhaps, as being small molecules.

**Good tickets include background information.** This aids good decision-making by people who come after the original writer. It is often packaged as a **user story**. A user story explains:

* who will benefit or has a problem that needs to be solved
* the problem or the desired solution
* the end goal of the beneficiary

The format of a user story is usually something like:

> As a (kind of user), I want/need (solution to problem) so that I (experience or result obtained).

With this information, the product development team of designers and engineers can start solving a problem, enabling them to take ownership of the problem and the customer's pain. Most importantly, it's formatted in a way that engages their skills and talents, which is why they were hired in the first place.

**The Four Cs of Good tickets are:**
* **correct** - They reflect what is actually wanted, precisely and accurately. The key to this is that the Product Manager (PM) or Product Owner (PO) must work with stakeholders and understand industry standards. In case of uncertainty, a good PM/PO works with a very knowledgeable subset of the product team to arrive at a precise and accurate definition. 
* **clear** - They are clear. I recommend running the description portion of tickets through a readability scanner like [Hemingway App](https://www.hemingwayapp.com).
* **complete** yet **concise** - They contain everything the team needs to get started, otherwise they will have to waste time coming back for more information. While writing a ticket, you should cut unnecessary details, attachments, and even words or phrases; otherwise, the ticket quickly becomes a jungle, and key information will get lost in the clutter.

If a ticket lacks any of these four Cs, the team will waste time having to reconnect and sort through old notes trying to figure out what was meant and whether it still applies.

**Good tickets use straightforward grammar.** This is part of clarity. It is also worth calling out specially. The point of writing a ticket is to make its contents understood. Lots of people unconsciously use unnecessarily long or complicated words and phrases. A common offense is to use words like _utilize_ rather than _use_. The cumulative effect of big words and long sentences is cluttered communication. Avoid jargon that your intended audience is unlikely to know. Every extra or unknown word increases the chance of a reader getting distracted or giving up.

Run your writing through a readability scanner to see where you can make improvements. Aim for writing at the 7th to 9th grade level so that any adult can read it quickly and comfortably. My favorite scanners:
* [Readable](https://www.readable.io)
* [Hemingway App](https://www.hemingwayapp.com)

**A good ticket is not too big or not too small** It suits the time-frame and team members involved in its execution. Think of an atom or a small molecule, not a rocket ship.

# A Bad Ticket

Imagine a ticket's contents broken up into this form.

|form field         |field contents                                          |
|-------------------|------------------------------------------------------- |
|summary            |Fix developer portal                                    |
|reporter           |Ryan                                                    |
|date created       |2019-03-29                                              |
|team               |Front End Team                                          |
|current assignee   |tbd                                                     |
|status             |backlog                                                 |
|user story         |                                                        |
|acceptance criteria|1. The fly-out panel on the left should work. Right now when I click it, nothing happens. When it opens, it obstructs my ability to interact with other controls on the page and this interferes with my workflow preferences. Then I can't get it to close by clicking the X button.|
|Definition of Done |No bugs                                                 |
|attachments        |                                                        |
|work log           |                                                        |
|last modified by   |                                                        |
|last modified date |                                                        |

There are a few general problems with this ticket:

* The summary is vague.
* The reporter field may not give enough information to help readers contact the writer.
* Without background information, the Front End Team won't really know why they're doing what they're asked to do.

The acceptance criteria:

* is vague and incomplete. It does not provide clear guidance about what is expected or required.
* jumbles multiple problems into one ticket.

The definition of done states only the obvious.

# A Good Ticket

Let's look at the same ticket reworked.

|form field         |field contents                                          |
|-------------------|------------------------------------------------------- |
|summary            |Developer portal's left flyout panel blocks underlying form   |
|reporter           |ryan.haber@mycompany.com                                |
|date created       |2019-03-29                                              |
|team               |Front End                                               |
|current assignee   |tbd                                                     |
|status             |backlog                                                 |
|user story         |As an external developer, I need to enter long key values in a form on MyCompany's developer portal that I retrieve from a flyout panel in the same portal, but this panel covers the controls. So that I can work more accurately, I need to easily enter these values without having to jot them down on paper.|
|acceptance criteria|1. The panel helps developer-users capture and enter the values in some digital way. E.g.: "copy to clipboard" button or at least a copy-and-paste-able field to hold any values that might need to be recorded by the developer.                    |
|  |2. The interface makes valid workflow(s) intuitive.            |
|  |3. Success is indicated by a 50%+ increase in the rate of form completion over 3 months.                                                 |
|Definition of Done |1. Finished build asses all unit and integration.                                                 |
| |2. Finished build accommodates at least 25 concurrent users.                                                 |
| |3. Meets all standards set in MyCompany Base SLA.                                                 |
|attachments        | userFeedbackSurveySummary.xlsx                                                      |
|work log           |                                                        |
|last modified by   |                                                        |
|last modified date |                                                        |

What do we see in this revised ticket?
* The summary is clear and complete.
* Readers will know who to contact with further questions.
* The user story provides background information that the development team needs to think of a good way to solve the problem.
* The ticket does not not attempt to micromanage the team, but does provide clear requirements.
* The ticket has peeled off separate, albeit related, issues for other tickets.
* Other useful information is attached that may help the team get a sense of what is frustrating users.

If you use this approach, you give the development team the information and freedom they need to make intelligent decisions to solve a problem rather than to act like cogs in a machine that needs constant managerial tinkering.

# Conclusion: Coordinate - Not Dominate

You wouldn't want an urban planner telling a civil engineer how to build a new bridge. The urban planner understands what is required, coordinates other moving parts, and makes this information available to the architects and engineers who then develop and implement a safe, economic, and beautiful design to enhance a city and serve its needs.

Likewise, it is not the role of a product manager, product owner, or business analyst to tell engineers how to do their job. Instead, these product management types should make clear what outcomes the stakeholders need and what constraints the business and its market impose on the situation.

The atomic unit of organization for the workflow that results is a ticket or issue. A good ticket serves as a point of reference for all involved. When they are well written, managers can arrange them into different to-do lists, epics, user story maps, or any other pattern they like. Managers can assess relative or even actual costs and values for development and then make sound decisions about organization priorities.

That all starts with a good, clean ticket.