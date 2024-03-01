Purpose: demonstrate simple Java command line compilation and
debugging, and using Gradle to build and run Java, to use arguments etc. 

Compile and run on the command line:
Independent of the system you are on, the following command should work.

#1. Running with Gradle#
Included in the project directory is a Gradle build file: build.gradle

In your command line go to the folder where the build.gradle file is located. 
Run 'gradle tasks --all' it will show you all available tasks and their description. 
Especially important: build, clean, run, runApp, runFraction

Take a look at the build.gradle file and run all the different taks and play around with it to understand Gradle better. 


#2. Compiling and running the debugger from the command line#

cd src/main/java
javac -d . -g Fraction.java
jdb -classpath . Fraction
stop in Fraction.main
stop in Fraction.<init>
stop in Fraction.setNumerator
run                    


