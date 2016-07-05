reStructuredText Tutorial
=========================

This file will give you a short tutorial showing you the basics of the reStructuredText (.rst) language.


First Things First
------------------

Paragraphs and Titles are the first things you'll encounter.  To make a paragraph all you have to do is type the text out like you would normally but without indentation.  In order to separate paragraphs or content put one or more lines in between the two items of content like the example below (in order to separate sections put two or more lines in between)::

  This is paragraph one.  This is just some text to show you how to write a paragraph.  Aren't paragraphs fun?

  This is paragraph two.  Just some more filler text to make every thing look like two paragraphs.  Yea, they kind of are!


There are two types of titles with the difference being one is larger than the other.  The biggest title or ``headline title`` as we will call it, is made by putting a series of equal signs under it::

  Headline Title
  ==============

And the smaller title or the ``section title`` is made by putting a series of dashes underneath like so::

  Section Title
  -------------


Make Sure You're Inline
-----------------------

Any kind of italics, underline or what have you, will be considered ``inline markup``.  Below is an example on how you would do each::

  *italics*
  **boldface**
  ``codesamples``


Links on Links
--------------

There are two ways to link external sites in your documentation.  The first way is the easiest and most used way.  Use the following format::

  This is a sentence that has `Link Text <www.example.com>`_ in it.

The second way is mainly for when you reference the same link over and over again.  You can set a variable and then call that variable in a sentence.  First you must put the variable at the top or bottom of your page with spaces after or before it and then reference the name later on::

  .. _name of the link: www.example.com

  Later on in a sentence you could reference the `name of the link`_.


Lists and Quotes
----------------

Lists are somewhat easy in the sense of all you have to do is hit enter and add a new symbol to make a new list item.  The following shows you different ways to make a simple list::

  * Bulleted lists start with asterisks
  * And can also take up
    two lines if need be.

  1. Numbered lists can be made one of two ways.
  2. Starting with numbers

  # Or they can start with pound signs too.
  # These act as normal lists

You can also make lists inside of lists by indenting the the sublist item and separating it from the main list items by a full space::

  * This is a main point

    * With this being a sub-point

  * Main points continue

In order to make a definition just remove the symbols::

  Definition
    A definition of the word placed above.


Code Blocks
-----------

If you need to reference code that isn't short you would use a code block.  The explanation will go on top followed by ``::`` then putting a space between the explanation and the code and indenting the code like so::

  This is the explanation::

    These lines will be a block of code. Anything after the ``::`` and underneath the space of the explanation will be automatically transformed into a code block.

  While adding a space after the code and typing will be back to regular paragraph form.


Last But Not Least
------------------

Images are important as you need screenshots to go along with what you are talking about most of the time.  So in order to add an image in to the documentation you must save the image in a folder that is in the documentation folder and use::

  This is a sentence explaining something that needs the screenshot below:

  .. image: img_folder/example_image.png

  This continues on after the image.
