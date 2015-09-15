SassBuild Project - brad slattman 2014 - slattman@gmail.com

This project will automate the compile process of sass scripts using an ant script. It depends on Ruby and Sass.
Please feel free to email me or additionally you can consult with google for more information.

Step 1)
Install Ruby and Sass on the system

Step 2)
Import the SassBuild project into your workspace.

Step 3)
Edit the paths to your input and output files in SassBuild/bin/build.scss.bat

Step 4)
Setup automation:

1) Right click on the project which contains the scss files you wish to auto compile. i.e. Stores. Select Builders from the context menu.
	
2) Click New… and choose Ant Builder.

3) In the Name field type the name you wish to call the builder. i.e. SassBuild.

4) In the Buildfile field choose “browse workspace” and locate /SassBuild/build/build.xml

5) In the Base Directory field choose “browse workspace” and locate /SassBuild

6) Click on the “Refresh” tab and check the box; “Refresh resources upon completion”. Choose “Specify resources…” and browse to your css folder and put checkmark next to that folder. Ideally your scss files will also be in this folder. Make sure “Recursive include sub-folders” is checked.

7) Click on the “Build Options” tab. Ensure “Allocate Console” is checked and “Launch in background” is unchecked. Now check “Specify working set of relevant resources”. Click on “Specify Resources…”. Browse to your scss folder and put a checkmark next to that folder. Click finish when done.

8) Click Apply and Finish.

Step 5)
Make sure build automatically is enabled in your workspace.


Thats it!

Now when you make changes to any scss files in the specified relevent resources, the ant build script will run and execute the batch file. This will tell sass to compile the scss file you specified in build.scss.bat and it will output your compiled css.



