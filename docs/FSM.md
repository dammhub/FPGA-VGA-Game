# Game State Machine

```text
                +----------------+
                |     START      |
                +----------------+
                        |
                 Space Key Press
                        |
                        v
                +----------------+
                |    STAGE 1     |
                +----------------+
                  |          |
            Collision     Goal Reached
                  |          |
                  v          v
          +---------------+  +---------------+
          |  GAME OVER    |  |   STAGE 2     |
          +---------------+  +---------------+
                                 |
                          Goal Reached
                                 |
                                 v
                         +---------------+
                         |   STAGE 3     |
                         +---------------+
                                 |
                          Goal Reached
                                 |
                                 v
                         +---------------+
                         |  GAME CLEAR   |
                         +---------------+
```
