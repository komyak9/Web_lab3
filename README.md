# JavaServer Faces Framework application that detects points in a given area on the coordinate boundary.

### Task:

The application must display 2 facelets templates - the start page and the use of the application page, as well as a set of managed beans (managed components) that implement server-side logic.


#### The start page should contain the following elements:

1. "Header" containing the student's full name, group number and option number.
2. An interactive clock showing the current date and time, updated every 11 seconds.
3. A link that allows you to go to the main page of the application.


#### The main page of the application should contain the following elements:

1. A set of components for setting the coordinates of a point and the radius of an area in accordance with the setting option. You may need to use additional component libraries - ICEfaces (prefix "ace") and PrimeFaces (prefix "p"). If a component allows input of deliberately incorrect data (such as letters in point coordinates or a negative radius), then the application must validate them.
2. A dynamically updated picture depicting an area on the coordinate plane in accordance with the number of the variant and points, the coordinates of which were specified by the user. Clicking on the image should initiate a script that determines the coordinates of a new point and sends them to the server to check if it falls into the area. The color of the dots should depend on the fact of hitting / missing the area. Changing the radius should also initiate a redraw of the image.
3. A table listing the results of previous checks.
3. A link that allows you to return to the home page.

#### Additional application requirements:

1. All verification results must be stored in a database managed by the PostgreSQL DB.
2. To access the database, you must use JPA with an ORM provider at the discretion of the student.
3. An Application-scoped Managed Bean must be used to manage the list of results.
4. Managed beans must be configured using parameters in the configuration file.
5. Navigation rules between application pages must be specified in a separate configuration file.

![index](https://user-images.githubusercontent.com/42679553/171596315-3c572492-b4e7-4c3a-8c04-01cce8f70991.png)

![main](https://user-images.githubusercontent.com/42679553/171596458-72ddd63e-f13d-4fe2-9af1-15fc9b6221d6.png)



