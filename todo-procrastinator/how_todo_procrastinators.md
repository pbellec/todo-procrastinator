---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
(how-to)=
# How-to

## Software
Let's start with a bit of logistics. The to-do list for procrastinators does not rely on a particular software, or website. It can probably be implemented with any solution you are already familiar with. If you have already found a to-do list software you like, I would encourage you to stick with it. I am personally implementing the to-do list with a simple text editor and a format called markdown to keep track of headers, and links, etc. Markdown gets rendered as a web page mostly for aesthetics. Sometimes I will explain how a particular aspect of the to-do list is implemented in my text-based system, but hopefully you can adapt this aspect easily in whatever software you are using.   

## A list of to-do lists
The to-do list for procrastinators is not a single list, but rather a list of lists. This is very important, critical even. If you, like me, are using a text editor to manage your to-do list, simply use a folder with each to-do list stored in a separate file, e.g.:
```
todo_executive.md
todo_work.md
todo_perso.md
todo_stack.md
```

```{warning}
It is absolutely necessary that you are able to access your various to-do lists independently of each other, adopting a divide-and-conquer strategy.
```

## The executive to-do list

You will most commonly access a single to-do list, called the `executive` to-do list. This to-do list contains the items that require immediate action. In a way, that is the only to-do list you really need to care about. The `executive` to-do list is by design short, and features only a fixed number of set categories. The category themselves only contain a limited number of tasks. Here is an example of an executive to-do list:
```
# Executive to-do list - an example

## Now (max 1)
  * Taxes. Get copies of income forms.

## Fast (max 3)
  * send a copy of invoice from Netlify to <admin@my.job>.
  * complete [evaluation form](https://mail/16544) for John Doe's committee.
  * fill the [doodle](https://doodle/452) for Jane Doe's committee.

## Emails (max 3)
  * Answer [John Doe's long winded question on linux](https://mail/12545).
  * Send a doodle to set a recurring meeting with Jane Doe.
  * Decline Jane Doe's [request](https://mail/47272) to give a 3 hours training.   

## Urgent (max 3)
 * Financial report for John Doe's grant. Create template document. Deadline: last week.
 * House cooperative meeting. Draft agenda points. Deadline: March 8th.

## Important (max 3)
 * Write the first draft of the "executive to-do" paragraph.
 * John Doe imaging paper. Draft 1st paragraph of results.
```
Let's talk about the different categories, starting with `Now`.

## Now

The `Now` category is **special**: it tells you _what you're supposed to be doing, right now_. There's only one (1) possible item in that category, because multi-tasking is not really a thing, and certainly not for procrastinators. The idea is that when you have to decide what to do, you go through your `executive` list, select one item, move it to `Now`, and get going. However, it is very possible that you will procrastinate and start working on something else, rather than the `Now` item. That's absolutely OK. Actually, that's how the `executive` to-do list is supposed to work. More on that later.

## Other executive categories
The other categories of the `executive` to-do list are simpler than `Now`, and they all feature a maximum of three (3) items:
  * `Fast` is for, well, fast tasks. Say _under 30 mns_ to complete.
  * `Emails` are for emails that require some substantial amount of work. Maybe the answer will be long to type, say more than 2 mns, or the answer is short but the email requires a lot of decision (or emotional) processing prior to answering. Note that your other emails should either be answered immediately, or not at all (just archive them or let them collect dust in your inbox for ever, it's fine). For `Emails` tasks, it is useful to keep a link right to the email, so you do not waste time looking for it when time comes to answer.
  * `Urgent` is a category for tasks with a deadline in the near future or, most often, in the past. For these tasks, it is useful to indicate the deadline in the task description.
  * `Important` are for things which really matter to you. There is typically little outside pressure to get these tasks done, but they should be treated with similar priority, or even higher, than tasks in the urgent category. That's either because you have an healthy dose of selfishness, or because you realize that the `Important` items are what brings you joy, and will fill you with the necessary emotional fuel to deal with the other task categories in your list.

```{note}
You may notice that there is no category for tasks which are both long, not urgent, and unimportant. I suggest to simply wait for those to become urgent before adding them to your `executive to-do list`, or avoid doing those tasks altogether. If you really think it is necessary for you to schedule this type of tasks, you may want to add a category `Misc`. I would then suggest having only one (1) item in that list.
```

## Why and how the `executive` to-do list works
Say you start your day, and you pick up a task in your `executive` to-do list. Right after choosing the task, you start to procrastinate and do something else. Because _you are a procrastinator_, after all. Yet, you have just been primed by reading your executive to-do list, which is filled with less anxiety-provoking, less annoying or more fun tasks than your `Now` task. Part of you realize the values of getting those tasks done. There is a solid chance that you will procrastinate using another item from your `executive` to-do list. Otherwise, you may even actually start working on your `Now` task. In all these cases, you win: **you are actually knocking down an item off your to-do list**.

```{admonition} Number and size of categories
:class: tip
Having four (4) main categories in the `executive` to-do list means that you have at all times a nice spectrum of tasks to procrastinate from, with a range of time commitment, boredom, anxiety levels and topics. Having only three (3) items per category means that you can go through the entire list in a few minutes. Checking your `executive` to-do list will feel like an easy task that you are unlikely to procrastinate from. If you find the `executive` too short or too long, you may want to adapt the numbers of categories as well as the number of items per category to your needs.
```

## Other to-do lists

It should now be evident that the tasks in the `executive` to-do list need to be selected with care. That selection process is where our other to-do lists come in the picture. The other to-do lists are expansive, which means they contain an unlimited number of categories, and an unlimited number of items per category. What those expansive to-do lists are and what categories they feature really do depend on what you do in life, and your interests. Maybe you are really into gardening, and you have lots of tasks related to your garden, in which case you may want to have a `todo_garden.md` list dedicated to garden activity planning, with related categories (`orchard`, `vegetables`, `flowers`, etc). I personally only use two lists:  
 * `todo_work.md`: is for the various projects I deal with at work. The categories can be related to the organization of a course (I do teach), or running a series of scientific experiments (I do research), or writing an article (I write occasionally). I will give an example of a category latter.
 * `todo_perso.md`: is for my personal projects, outside of work.

 ```{admonition} To-do list and personal projects
 :class: tip
  I tend to avoid using to-do lists for my personal life, so that list is pretty short. More precisely, I try to keep my personal life simple and spontaneous enough that I do not need a to-do list for most things. But there are of course exceptions. Filling out taxes, dealing with my immigration paper work or following up with house maintenance are all worthy of a section in a to-do list.
 ```

## The stack list
There is another special expansive to-do list I use, as some kind of overflow for the `executive` to-do list. I call it `todo_stack.md`. It often happens that something comes up suddenly, that is urgent. If I am ready to deal with it immediately, then great: it will not involve the to-do list at all and I just do it. But this urgent action may still need to be scheduled - if I am already doing something or need time to prepare. In that case, the task needs to be added to the `executive` to-do list - this is an *absolute* rule, you cannot work on it otherwise. If said `executive` to-do list is full, then you will instead add this item to `todo_stack.md`. That list is structured exactly like your `executive` to-do list, except it does not have a `Now` category (there is only one `Now`), and there is no limit on the number of items per category. If you want to address this new task quickly, you will *have* to first get one item off your `executive to-do list`, in order to make space for the new task. I found the surge in anxiety coming from being unable to attend an immediate issue is a very powerful motivator to deal with short but emotionally taxing items from my to-do list.

## Categories in expansive to-do lists

Here is an example of a category in my `todo_work.md` list:

```
## The to-do list for procrastinators
 * draft intro
 * draft first section
   * paragraph on problems with procrastination
   * paragraph on success and procrastination
 * draft second section
   * paragrah on the executive to-do list
   * paragraph on the stack
```

A couple of notes here. First, you will notice that each task is indicated by a bullet (or `*` in markdown). The number of spaces before the `*`, the so-called indentation, indicates the level of the task. So `draft first section` is a main task, while `paragraph on problems with procrastination` is a subtask of `draft first section`.

Second, it is *very important* that you break down tasks into very small subtasks. If a big task ever makes it to your `executive` to-do list, it will clog the list, possibly for weeks, and will make you unable to adapt to on-going demands or your mood.

Third, you do not have to plan a given category in details. You can start with a few generic tasks, and add subtasks while you are working on a project. You can also revisit a task that was too big or poorly designed to change it - for example breaking it into subtasks.

 ## Feeding the `executive` monster

 There is no special time for you to add an item to your to-do list. Whenever you are low on tasks, something urgent comes up, and you have a sudden urge to work on a particular project, just visit one of your expansive to-do list, select an item, copy it to the executive `to-do list` and "voilà"! Of course, if your to-do list is full, you will *have* to get something done on the list before adding any new item. Procrastinating with tasks outside of the `executive` to-do list should be seen as off-limits.

 ```{admonition} A never-ending to-do cycle
 :class: tip
 You should never expect to empty your executive to-do list. Tasks will keep getting added as soon as there is space. This actually should bring you comfort: you will never fail again to clear up your to-do list - it's never expected to happen - and you will not have to plan your daily schedule in details - just follow your fancy in the `executive` to-do list.
 ```

## Trouble shooting
```{admonition} I find this system awfully complicated, can you explain it again?
:class: note
Make a short to-do list, and when you have some time to work, pick a single item for what you are supposed to do `Now`. All the rest really is bells and whistles.
```

```{admonition} I have not looked at my executive to-do list for several days.
:class: note
Maybe the list is too long and scary. Consider dropping one category. May I suggest dropping `Emails`? `Emails` can generally go under `Fast`. You can also limit the number of items per category to 1 or 2.
```

```{admonition} Some items never get done in my to-do list.
:class: note
You may want to remove the problematic task, and break it into subtasks. You may also want to consider whether this task actually needs to get done at all, or - slightly different angle - whether you are actually ready not to do it and face the consequences. I will discuss this internal dialogue a bit in the {ref}`third section <origins>`.
```

```{admonition} My stack to-do list is growing endlessly.
:class: note
You may want to transfer some items to other expansive lists. You may also want to come to term that some of these tasks will not get done, and simply remove them. Do not feel too guilty: for some of these tasks someone will come back with a reminder. And you may then find the courage to deal with them.
```

```{admonition} One of my list is so long I don't want to look at it.
:class: note
Split that list into several lists. I tend to be an horizontal thinker: I would rather see everything in one giant list in order to set my priorities (but **not** to decide what I have to do now - then I would get anxious). But some people are more vertical: they like better having many shorter lists. Experiment and find what works best for you.
```
