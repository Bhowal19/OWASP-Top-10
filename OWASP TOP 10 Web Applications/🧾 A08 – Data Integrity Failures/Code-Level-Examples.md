# Code-Level Examples

Data integrity failures often hide behind clean code.

Consider insecure deserialization.

```java
ObjectInputStream in = new ObjectInputStream(request.getInputStream());
Object obj = in.readObject();
