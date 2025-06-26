# CS120
Project Overview

This project is a C++ console application designed to help the Corner Grocer analyze item purchase patterns from their daily records. The store generates a log of every item purchased throughout the day, and this program processes that file to determine how often each item appears. It provides a simple menu interface where users can look up individual item frequencies, view a list of all items with counts, or display a histogram that visualizes those frequencies. The program also automatically generates a backup file for reference. The purpose of this tool is to help the store make informed decisions about how to arrange their produce section based on customer behavior.

Reflection

What problem does this solve?
The program helps a local grocery store understand which items are purchased most frequently. This supports business decisions like reorganizing shelves and optimizing layout based on popularity. Instead of counting items manually or working with unstructured logs, the store now has a clear, automated way to access the data they need.

What did I do well?
I structured the code cleanly using object-oriented principles. The GroceryTracker class encapsulates all data processing and file I/O, which keeps the main function focused on user interaction. I also followed consistent naming conventions and commented the code in a way that explains the purpose of each function and logic block. My use of a map for tracking frequencies ensured that data is both sorted and efficiently accessed.

Where could the code be improved?
There are a few ways this project could be enhanced. I’d like to make item searches case-insensitive to avoid missing matches like “apples” vs. “Apples.” Adding better error handling for missing or corrupted files would also improve the program's resilience. If I refactor input validation into its own function, it would reduce repetition and clean up the main() function. These changes would make the program more secure, maintainable, and user-friendly.

What was most challenging?
The most difficult part was handling file input and output in a way that didn’t interrupt the program flow. I needed to make sure data was read correctly from the file and written to the backup file without causing crashes or losing information. I worked through this by researching examples and reviewing documentation until I understood how to isolate the file logic properly.

What skills are transferable?
This project gave me experience with class-based program design, file handling, and user input validation—all of which are useful in just about any software project. Understanding how to use maps for frequency tracking is something I’ll carry forward into data processing tasks, and writing clean, commented, modular code is a habit I’m continuing to build.

How did I make the program maintainable and adaptable?
The structure of the program supports future updates. The GroceryTracker class handles all internal logic, so if new features are added later, they can go into that class without affecting the menu system. The code is commented clearly, variables are named descriptively, and the file paths are passed as arguments so the input/output can be changed easily. These decisions were intentional to make the program easier to revisit and maintain over time.
