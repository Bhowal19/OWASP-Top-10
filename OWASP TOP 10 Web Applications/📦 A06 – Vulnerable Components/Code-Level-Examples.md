# Code-Level Examples

Vulnerable components are often invisible in application code.

Consider a simple import statement.

```java
import org.example.framework.CoreService;

here is nothing unsafe about this line.
Yet the imported framework may include vulnerable logic several layers deep.

The application code may never reference the vulnerable function directly.
Attackers do not care.
If the component is loaded, reachable, and exploitable, the application is exposed.

In some cases, components execute code during startup.

require("some-package");


This statement may trigger initialization logic that runs automatically.
If the package contains malicious or vulnerable code, execution happens before the application logic even begins.

The danger of A06 is that the vulnerability often exists outside the developer’s mental model.
The code looks clean.
The risk lives elsewhere.