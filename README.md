The project is tested and known to work in Linux. It *should* also work on Windows.

1) Open a command prompt window / terminal and get to the folder this README file is located in.

Run: cd blabla

2) To compile the program, we need to use javac. The classes needed are present in jars/cloudsim-4.0.jar

Linux:
javac -classpath jars/cloudsim-4.0.jar:. Project.java
Windows:
javac -classpath jars\\cloudsim-4.0.jar;. Project.java

This will produce the file Project.class
This file is already present in the upload because I compiled it earlier. You don't need to run the javac command unless you make changes to the code.

3) To run the program, we need to use Java.

Linux:
java -classpath jars/cloudsim-4.0.jar:. Project > logs.txt
Windows:
java -classpath jars\\cloudsim-4.0.jar;. Project

(The output of the program is very large and I redirect it to logs.txt)

What the code does is, it runs a simulation of N cloudlets on M VMs, and notes the average time it takes for the cloudlet to complete its job.
N varies from 1 to 400, and M varies from 1 to 10

The output is presented as comma separated values at the end of logs.txt. This can be copy pasted into a CSV file and opened in Exel.
One CSV file has already been generated for you, under the name out.csv
out.csv will show that there is a linear relationship between the time taken by a cloudlet, and the number of cloudlets running
on the Virtual machine.

If there is a problem running or compiling the code, check out examples.txt
