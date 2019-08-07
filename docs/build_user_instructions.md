#Build & User Instructions

##Back End
Do this first!
1.Fork and clone the ABQ Trails Serverside from github using SSH key.
2.Checkout and import as Maven project using your preferred IDE.
	a. Use JDK 1.8 for your build.
	b. We highly recommend IntelliJ IDEA. If you are not using IntelliJ you may need to import the dependencies separately. See the backend dependencies in Functional Inventory listed 
here.
3.Build the application once all imports/whatnot are complete
	a. If you get an error indicating that a bean factory could not be built, double check your connection to the MySQL database using database tools. This will be the cause.
	b. A few moments after the application has started, you should see the data import from CABQ begin. You should see SELECT trail followed by INSERT trail. This will build the table trails_table in db_trails. 
Subsequent builds will simply show SELECT trail unless CABQ makes a change to their data. 
4. Your database should now be up and running. Proceed to fork and clone/import ABQ Trails Client Side.


##Front End
1.Fork and clone the ABQ Trails Client Side from Github using SSH key.
2.Checkout and import as Gradle project using your preferred IDE.
	a. Use JDK 1.8 for your build.
	b. We highly recommend IntelliJ IDEA. If you are not using IntelliJ you may need to import the dependencies separately. See the frontend dependencies in Functional Inventory listed here.
3. You will need to either generate your own connection to the Google maps API OR contact a member of our team to add your SHA1 key to our API.
4. Ensure that your Android emulator has Google Play and that you have a Gmail account you can use to log in.
5. Build the app.
