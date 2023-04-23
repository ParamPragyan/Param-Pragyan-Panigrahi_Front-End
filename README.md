## 1. Explain what the simple List component does.
<p>As props, the List component (which is a memorized component) receives an array of objects. This list's objects all have a text attribute. The List component renders the text property value of all the elements in the list argument as an unordered list. Each unordered list element has a red background by default, which turns green when the element is clicked. This feature might be used to tell the user that a certain element has been selected. At any given moment, just one element can be picked.</p>
<img align="top" alt="Coding" width="100%" src="https://github.com/ParamPragyan/assets/blob/main/ss1.jpg?raw=true">

## 2. What problems/warnings are there with the code?
a. For function calls, the ``arrow`` function should be used for handling any event.

<img align="top" alt="Coding" width="100%" src="https://user-images.githubusercontent.com/54448525/233854127-c44d644b-2e40-4d4b-a723-f080c344d0ab.png">

b. The first element of the array returned by ``useState`` is always ``state``and the second one is ``setState``.

![image](https://user-images.githubusercontent.com/54448525/233854231-dc7a596d-e9fa-4bc6-8017-1cfe54223d60.png)

c. The ``isSelected`` property requires a boolean value. This semantic mistake was detected using ``propTypes`` specified for the SingleListItem component. The possible solution is as follows: ``isSelected={selectedIndex === index}``


![image](https://user-images.githubusercontent.com/54448525/233854599-2035581d-a0bd-49d8-b899-8e2a10f29df4.png)

d. As we are defining types of array element the ``array`` should be ``arrayOf`` and as for syntax, the ``shapeOf`` should be just ``shape``.

![image](https://user-images.githubusercontent.com/54448525/233854337-a1cf0e9a-6a22-4570-9791-69a48ea22712.png)

e.  ``*note: we shouldn't be using "defaultProps" for this code as it is going to be deprecated in "React 18.3.0".``
the ``defaultProps`` should pass the items to display instead of being null.

![image](https://user-images.githubusercontent.com/54448525/233855428-90954b82-79e4-4fbf-baf9-6373ece82489.png)


## 3. Please fix, optimize, and/or modify the component as much as necessary.

<img align="top" alt="Coding" width="100%" src="https://user-images.githubusercontent.com/54448525/233852838-4b04f621-2cdf-4bee-8c80-7a72129ea1b4.png">
