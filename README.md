# Overview

In this project, an HTML page is built to display all recorded UFO sightings in the US in the first few days of year 2010. Using javascript, capability is provided to filter this information based upon:
* A specific date
* City
* State
* County
* Shape of the UFO object

# Results

The search functionality is provided using input text boxes. An event listener fires every time the user enters data in the search box **and clicks somewhere or presses the enter button**. An example search and the corresponding result is demonstrated in the picture below.

![Search](static/images/search.png)

The search is done using the following criteria:

* Date: 1/1/2010
* State: ca
* County: us
* Shape: light

# Summary

## Drawbacks:

* **placeholder** values for the textbox give the wrong impression of having made a selection for that filter (example, the city **benton** in the above textbox is not selected).
* The code would need to change if more attributes are made available in future for UFO sightings.

## Further Improvements:

* Provide a dropdown menu for each filter (such as Excel) to let the user choose from available values rather than making a blind search.
* Rather than putting the filters in HTML, insert them directly from Javascript. It is easy to control from the code which and how many filters we should make available to the users.
* While loading the table each time for every page refresh from scratch works for small tables, it would be prohibitive for larger tables. In such cases, use a database and push the current filter from the user in the database, and retrieve it for each page reload to display only the rows selected from the last filter.
