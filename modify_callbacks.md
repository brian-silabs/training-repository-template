---
sort: 2
---

# Modify the callbacks to integrate your application

-	Always add at the top this header
```
---
sort: 2
---
```

- 	Add some code mentioning its language

```c
#include EMBER_AF_API_NETWORK_CREATOR
#include EMBER_AF_API_NETWORK_CREATOR_SECURITY
#include EMBER_AF_API_FIND_AND_BIND_TARGET

#define WINDOW_COVERING_ENDPOINT (1)
EmberEventControl networkManagementEventControl;
EmberEventControl networkOpeningEventControl;

void networkManagementEventHandler(void);
void networkOpeningEventHandler(void);
```

-	Add some console steps

```console
zcl window up
```
