# Visualisation-of-DS-Algo
Visualisation of Sorting algorithms, Linked List, Stack and Queue operations.

## Sorting Algorithms Visualisation
    1. First, we need to import given python libraries.
    • random module in order to generate an array of numbers to be sorted.
    • matplotlib pyplot and animation
    2. Create a swap function to swap the elements in a given array. Sorting needs swapping therefore creating a different function will be helpful.
    3.  Create a bubble_sort function to implement the Bubble Sort algorithm.
    1. Run through two loops and repeatedly swap adjacent elements if they’re in wrong order.
    4. Create an insertion_sort function to implement the Insertion Sort algorithm.
    1. Iterate from array[1] to arr[n] over the array.
    2. Compare the current key element to its predecessor.
    3. If the key element is smaller than its predecessor, compare it to the elements before.
    4. Move the greater elements one position up to make space for the swapped element.
    5. Create a quick_sort function to implement the Quick Sort algorithm.
    1. Pick the last element as pivot.
    2. Partition the array on the basis of pivot.
    3. Starting from the leftmost element, keep track of indexes of smaller or equal to elements as i.
    4. While traversing, if we find a smaller element, we swap the current element with arr[i].
    5. Apply quick_sort on the left partition recursively.
    6. Apply quick_sort on the right partition recursively.

    6. Create a selection_sort function to implement the Selection Sort algorithm.
    1. The algorithm maintains two subarrays: 1) Sorted subarray 2) Remaining unsorted subarray.
    2. Sort the array repeatedly by finding the minimum element from the unsorted part.
    3. Put that element at the beginning of the sorted array.
    7. Create a Merge_sort function to implement the Merge Sort algorithm.
    1. Arguments: array, l, r
    2. Check if r>l
    3. Find the middle point to divide the array into two halves
    4. Call merge sort for first half
    5. Call merge sort for second half
    6. Merge the two halves sorted in step d and step e.
    8. Create a heap_sort function to implement the Heap Sort algorithm.
    1. Build a max heap from the input data.
    2. At this point, the largest item is stored at the root of the heap.
    3. Replace it with the last item of the heap followed by reducing the size of heap by 1.
    4. Finally, heapify the root of the tree.
    5. Repeat the steps above while the size of the heap is greater than 1.

    9. Create a shell_sort function to implement the Shell Sort algorithm.
    1. Initialize the value of h
    2. Divide the list into smaller sub-lists if equal intervals h
    3. Sort these sub-lists using insertion sort
    4. Repeat until the complete list is sorted.
    10. Create a count_sort function to implement the Count Sort algorithm.
    1. Find max from the given array
    2. Initialize an array of length max+1 with all elements 0.
    3. Store the count of each element at their respective index in count array
    4. Store cumulative sum of the elements of the count array.
    5. Find the index of each element of the original array in the count array to get the cumulative count.
    6. Place the element at the calculated index.
    7. After placing each element at its correct position, decrease its count by one.

    11. Let the user choose the number of elements they want to sort.
    12. Display a menu for choosing the sorting algorithm to display the visualization.
    13. Create a random list of numbers to be sorted by using .shuffle from the random library.
    14. A menu for choosing the algorithm is displayed using the if elif condition.
    15. Use .Normalize() to normalize color code data into [0.0, 1.0] interval.
    16. Set the colors of the bars according to their values using .LinearSegmentedColormap().
    17. Insert values of “red”, “green”, “blue” into the above function.
    18. Now, we will create a canvas for the animation using the matplotlib figure and axis.
    19. Use set_title() to display a title to your respective sorting algorithm.
    20. Create a bar container, then a bar plot where each bar will represent one number of the array.
    21. Set the view limits of x and y axes using set_xlim and set_ylim functions.
    22. text() is used to show the number of operations on the canvas. 
    23. The first two arguments are the position of the label.
    24. Use transform=ax.transAxes that tells that the first two arguments are the axis fractions, not the data coordinates.
    25. Set iteration = 0, which will keep track of the operations performed.
    26. The text displaying the number of operations will be shown in the upper left corner.
    27. Create an animate() function with the arguments - array, rects and number iterations. We will be repeatedly calling it.
    28. Set the size of each bar equal to the value of the element they are representing by using zip() and set_height().
    29. Height of each bar will be updated using the functions above.
    30. We will now create anima object in which we pass frames = generator that takes the generator function, and then it passes the generated or updated array to the update_plots.
    31. fargs takes additional arguments, i.e. bar_rec and iteration.
    32. interval is the delay between each frame in milliseconds.
    33. We set repeat to false.
    34. And, at last, we use plt.show() to plot the animated figure.

## Linked List Operations Visualisation
    1. First, we need to import given python libraries.
    • tkinter library for Python GUI.
    • messagebox widget.
    2. Create a Linklist class which contains various function definitions.
    3. Create init function which initialises the window with various graphical elements like background, height, width and other properties. Also set list properties and buttons, widgets and co-ordinates.
    4. Create another function for heading and status/information initialization process.
    5. Another function for start and other pointer initialization.
    6. Next we have the make button function to make some buttons to give instruction to the program.
    7. Now we have another function which makes a structure in which we will take input and display output.
    8. Next we check if such a node is existent.
    9. Then we have a function which makes the node with labels.
    10. Create a function which takes input.
    11. Then we have an insert node function.
    12. Then we have a reset function which resets co-ordinates and and stores values, arrow and next label.
    13. Next there is a delete node function which deletes the last node and particular node .
    14. Create delete first node function.
    15. Next is a method for deleting a particular node process start.
    16. Now in the main function we create a window  using the tkinter library.
    17. Next we initialize the title, geometry and icon of the window.
    18. Later we initialize maxsize and minsize of the window
    19. Lastly we call the Linklist class passing the created window and call mainloop function which runs the Tkinter event loop which listens for events, such as button clicks or keypresses, and blocks any code that comes after it from running until the window it's called on is closed. 

## Stack Operations Visualisation
    1. First, we need to import given python libraries.
    • tkinter library for Python GUI.
    • messagebox widget.
    2. Create a class StackVisualizer which contains various function definition.
    3. Create init function which initialises the window with various graphical elements like background, height, width and other properties. Also set list properties and buttons, widgets and co-ordinates. Also it makes some function calls.
    4. Create a function to set label for main heading, sub heading and indicator.
    5. Make buttons to access and make top with arrow.
    6. Make stack container.
    7. Set index of stack.
    8. Define the push button label with various functionalities like access button deactivation.
    9. Set function to make block.
    10. Create a function which implements the push button with horizontal and vertical controls and functionalities.
    11. Then we have reset position function which resets window and activates push and pop buttons.
    12. Next we implement pop function to pop element from stack.
    13. Lastly we call the StackVisualizer class passing the created window and call mainloop function which runs the Tkinter event loop which listens for events, such as button clicks or keypresses, and blocks any code that comes after it from running until the window it's called on is closed. 
