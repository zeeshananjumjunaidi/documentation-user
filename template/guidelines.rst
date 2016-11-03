=====================
How to write user doc
=====================

How to figure out a topic
=========================
* The documentation must be like a cookbook (one page = one problem). 
  Topics must focus on business concepts, not Odoo concepts.

* Sometimes a single concept (payment term) may cover several business 
  concepts, do 2 pages:
  
  * Cash discounts on customer invoices
  * Defining and using payment terms


How to write titles
===================
Talk "business need", not "how to use":

* Bad title: How to create checks?
* Good title: How to pay supplier bills by checks?


How to structure a page
=======================
A good structure for the document is:

* General Business concept

  * what is it? why should you use it?
  * explain concepts needed to understand the flow
* Business flows in Odoo
* Configuration if needed

  * simple flows
  * advanced flows
* Specific use cases (questions)
* Reporting


How to write
============

Who is the audience
-------------------
Target readers: lambda user, but not too stupid

* Don't explain how to create/delete documents
* Focus on business concepts

How to write cleanly
--------------------
* Not more than 80 char per row for easy technical reviews
* Title underlining must have the extact same length than text

How to write nice content
-------------------------
* The shorter the better

* Take clean screenshots (smaller possible, cut if needed, 
  with red frames/circles to emphasize on important buttons, fields)

  * Name screenshots this way in the section media repo: 
    app_topic_#.png (e.g. ecommerce_catalog_01.png,   ecommerce_catalog_02.png)
  * All documents & screenshots must be based on latest Odoo version.

.. image:: ./media/template_guidelines_01.png
   :align: center

* Write a ``Button`` this fashion (e.g. click on ``Action``). 
  Write the text exactly like in the system, respecting the case. 
  It's ok to have an uppercase here.

* When you use the name of an **App** or a **Menu**, put it in **bold** (e.g. 
  Once in **Sales Orders** menu...)

* Give navigation paths for advanced handlings: e.g. go to 
  a :menuselection:`Inventory --> My Account --> Overview`. Just give the menu 
  to use and a screenshot. NO NEED TO GO INTO THE DETAILS: e.g. it opens a 
  list view, click on *Create* button, click on *Save*. Don't do that. 

* Include links to external documents: e.g. go to 
  `Odoo Official Website <https://www.odoo.com>`_.

* Redirect to a demo database in order to illustrate a concept better (use action xml_id)

.. demo:action:: sale.action_orders

   Create a Quotation

.. tip:: Tips are always good for advanced features.

.. note:: Notes are also appreciated to keep remarks out of the main paragraph.

* Add links to related business topics at the bottom (can be in others apps)

.. seealso::

  * :doc:`topic1`
  * :doc:`../sales/products_prices/prices/currencies`