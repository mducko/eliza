This is a Processing library based on the Java implementation of the Eliza program by Charles Hayden.
Hayden's code is a complete and faithful implementation of the original program described by Joseph Weizenbaum in the <a href="http://www.cse.buffalo.edu/~rapaport/572/S02/weizenbaum.eliza.1966.pdf">Communications of the ACM in January 1966</a>.

ACKNOWLEDGMENTS

1) Charles Hayden's Java implementation of Eliza:
http://chayden.net/eliza/Eliza.html 	

2) Processing Library Template:
https://github.com/processing/processing-library-template

INSTRUCTIONS

The library is easy to use. Just import it, and then create an Eliza object:

```java
import codeanticode.eliza.*;

Eliza eliza;
eliza = new Eliza(this);

String response = eliza.processInput("Hello");
println(response);
```

You can use the readScript() function to change the script that Eliza uses to construct its answers:

```java
eliza.readScript("script");
eliza.readScript("http://chayden.net/eliza/script");
```

To go back to the default script that is loaded when Eliza is initialized, call the readDefaultScript() function.

For detailed instructions on how to modify the script file that determines Eliza's "behavior", read the following notes by Charles Hayden:  
http://chayden.net/eliza/instructions.txt

ANDROID DEPLOYMENT

To deploy the Eliza library as an Android app, follow these steps:

1. Ensure you have Android Studio installed.
2. Create a new Android project in Android Studio.
3. Copy the `src/codeanticode/eliza` directory into the `app/src/main/java` directory of your Android project.
4. Add the `AndroidManifest.xml` and `build.gradle` files provided in this repository to your Android project.
5. Modify the `examples/ElizaChat/ElizaChat.pde` file to be compatible with Android.
6. Add necessary Android dependencies in `build.gradle`.
7. Build and run the app on an Android device or emulator.

FURTHER REFERENCES

1) Wikipedia article about Eliza: http://en.wikipedia.org/wiki/ELIZA

2) Article from the Jul-Aug 1977 issue of the Creative Computing magazine, with a complete listing in Altair BASIC of a version of Eliza by Jeff Schrager: 
http://vintagecomputer.net/cisc367/Creative%20Computing%20Jul-Aug%201977%20Eliza%20BASIC%20listing.pdf
