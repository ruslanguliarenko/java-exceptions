# java-exceptions
<b>[UUID](https://medium.com/@frontman/%D0%BF%D1%80%D0%BE%D1%81%D1%82%D0%BE%D0%B9-%D1%81%D0%BF%D0%BE%D1%81%D0%BE%D0%B1-%D0%B3%D0%B5%D0%BD%D0%B5%D1%80%D0%B0%D1%86%D0%B8%D0%B8-%D1%81%D0%B8%D0%BC%D0%B2%D0%BE%D0%BB%D1%8C%D0%BD%D1%8B%D1%85-id-%D0%B8-uuid-88af71466574)</b><br />

A universally unique identifier (UUID) is a 128-bit number used to identify information in computer systems. The term globally unique identifier (GUID) is also used, typically in software created by Microsoft.

When generated according to the standard methods, UUIDs are for practical purposes unique, without depending for their uniqueness on a central registration authority or coordination between the parties generating them, unlike most other numbering schemes. While the probability that a UUID will be duplicated is not zero, it is close enough to zero to be negligible.

Thus, anyone can create a UUID and use it to identify something with near certainty that the identifier does not duplicate one that has already been, or will be, created to identify something else. Information labeled with UUIDs by independent parties can therefore be later combined into a single database or transmitted on the same channel, with a negligible probability of duplication.

<b>[Exceptions in Java](https://www.geeksforgeeks.org/exceptions-in-java/)</b><br />
An exception is an unwanted or unexpected event, which occurs during the execution of a program i.e at run time, that disrupts the normal flow of the program’s instructions.<br />

<b>Default Exception Handling</b><br />
Whenever inside a method, if an exception has occurred, the method creates an Object known as Exception Object and hands it off to the run-time system(JVM). The exception object contains name and description of the exception, and current state of the program where exception has occurred. Creating the Exception Object and handling it to the run-time system is called throwing an Exception.There might be the list of the methods that had been called to get to the method where exception was occurred. This ordered list of the methods is called Call Stack.<br />

<b>[Checked and Unchecked](https://habr.com/ru/post/268683/)</b><br />
Checked are the exceptions that are checked at compile time. If some code within a method throws a checked exception, then the method must either handle the exception or it must specify the exception using throws keyword.<br  />
Unchecked are the exceptions that are not checked at compiled time. In C++, all exceptions are unchecked, so it is not forced by the compiler to either handle or specify the exception. It is up to the programmers to be civilized, and specify or catch the exceptions.

<b>Operations with URL</b> <br />
First you have write the command and if you need write argument.<br /> 
<b>UUID add(String URL)</b>  - Associates the URL value with the UUID key and return UUID key. Method can throw OutOfBoundUrlsException <br />
<b>UUID check(String URL)</b>  - Returns UUID key if contains URL else throw ValueNotFoundException<br />
<b>String getUrlById(UUID uuid)</b> - Returns URL if present UUID key else throw ValueNotFoundException<br />
<b>String deleteById(UUID uuid)</b> - Delete and return URL and UUID if present UUID key else throw ValueNotFoundException<br />
<b>Map cleanAll()</b> - Delete and return all URL <br />