# Code-Level Examples

Insecure design is visible in code, but it is not caused by code.

Consider an API that processes orders.

```java
public void processOrder(String orderId) {
    Order order = orderRepository.find(orderId);
    order.complete();
}
The code works as written.
The flaw is not missing validation.
The flaw is that the design never required verification of who is allowed to process the order.

A secure design would have made ownership and authorization explicit requirements.
The code would reflect that decision.

public void processOrder(String orderId, User user) {
    Order order = orderRepository.find(orderId);
    if (!order.isOwnedBy(user)) {
        throw new UnauthorizedException();
    }
    order.complete();
}
The difference is not syntax.
It is intent.

Code cannot fix what design never defined.