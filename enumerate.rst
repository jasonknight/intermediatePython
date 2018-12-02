Enumerate
---------

Enumerate is a built-in function of Python. Its usefulness can not be
summarized in a single line. Yet most of the newcomers and even some
advanced programmers are unaware of it. It allows us to loop over
something and have an automatic counter. Here is an example:

.. code:: python

    for counter, value in enumerate(some_list):
        print(counter, value)

And there is more! ``enumerate`` also accepts an optional argument which
makes it even more useful.

.. code:: python

    my_list = ['apple', 'banana', 'grapes', 'pear']
    for c, value in enumerate(my_list, 1):
        print(c, value)

    # Output:
    # 1 apple
    # 2 banana
    # 3 grapes
    # 4 pear

The optional argument allows us to tell ``enumerate`` from where to
start the index. You can also create tuples containing the index and
list item using a list. Here is an example:

.. code:: python

    my_list = ['apple', 'banana', 'grapes', 'pear']
    counter_list = list(enumerate(my_list, 1))
    print(counter_list)
    # Output: [(1, 'apple'), (2, 'banana'), (3, 'grapes'), (4, 'pear')]

Enumerate will also work with strings so that you can go char by char with an index counter, consider:

.. code:: python
  s = "Hello World"
  for index,char in enumerate(s):
    print("%d: %s" % (index,char))
  # Output: 
  # 0: H
  # 1: e
  # 2: l
  # 3: l
  # 4: o
  # 5:
  # 6: W
  # 7: o
  # 8: r
  # 9: l
  # 10: d
