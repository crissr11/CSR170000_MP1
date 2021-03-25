# MP1
# Part 1 code includes: TestDominatorFinder.java, DominatorFinder,java, and GCD.java
The code was executed and I was able to see the complete breakdown of the dominator analysis from each of the return statments in the output.

# Part 2 code includes: Example.java and TestSootCallGraph.java
After running TestSootCallGraph and getting an output, I was able to learn that class hierarchy analysis (CHA) is able to identify all the possible methods that could be returned by a class that is not always precise. The other form of analysis is points-to analysis (PTA) which shows more precision than CHA but has to go through the entire program to complete its analysis. The output for the CHA code of the program contains a total of 12 edges being evaluated but is slightly inaccurate, and that becomes evident with the fact that Fish may call animal.saySomething() which is not possible based on the program. The output for the PTA code of the program only shows 7 edges due to its precision and does not have the issue that CHA had from its results. In terms of speed the CHA output took 0.011 ms to complete while the PTA output took 0.203 ms to complete. This shows that CHA is the faster code but that leads to its inaccuracies while PTA is slower but is more accurate. To run the code you would need to comment/uncomment the code snippets on lines 50-51.

# Part 3 code includes: TestSootLogging.java, Log.java, and HelloThread.java
The code needed to complete internalTransform() was completed and I got an output similar to the document.
Output from program:

Thread Thread-13 wrote static field x
Thread Thread-14 wrote static field x
Thread Thread-14 read instance field y of object $i0 = r0.<a1.HelloThread$TestThread: int y>
Thread Thread-14 read instance field y of object r0.<a1.HelloThread$TestThread: int y> = $i1
Thread Thread-13 read instance field y of object $i3 = $r2.<a1.HelloThread$TestThread: int y>
Thread Thread-13 wrote static field x
Thread Thread-13 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
Thread Thread-15 wrote static field out
