---
title: "Using Bookmarks"
weight: 1300
---


# Using Bookmarks

One of the most important features supported by most _Object Views_ is an ability to save and restore visual view state. Saving and restoring visual state of an _Object View_ enables rapid switching between different data regions and is similar to bookmarks used in Web browsers.

Initially an _Object View_ is created as _transient_. It means that its state is not saved. To save current state of a view select an item with the view name in the _Bookmarks_ part of the _Project View_ windows and select the _Add bookmark_ item in the context menu:


![](/images/65929321/96665608.png)

For every persistent view UGENE automatically saves the state of the view in the _Auto saved_ bookmark when the view is closed.

Now, by activating bookmarks you can restore the original view state. For example for the _Sequence View_ bookmarks you can store a visual position and zoom scale for the sequence region.


![](/images/65929321/96665609.png)

Use the _Update_ option for overwriting the existing bookmarked state.

Use the F2 keyboard shortcut to rename a bookmark. To remove a bookmark press the Delete key.

UGENE has limited set of built-in _Object Views_. Extensions modules or plugins can be used to adjust the existing views or to add new views to the tool.
