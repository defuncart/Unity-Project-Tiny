# PT01 - Hello World

A simple *Hello World* project which follow's Mike Geig's [Basic Workshop](https://www.youtube.com/watch?v=-yubuk7jAb4&index=1&list=PLX2vGYjWbI0TPRStIWx3UyNB8QqjNUj98).

**Unity Version:** 2018.3.02f
**Tiny Version:** 0.13.4
**Language:** TypeScript
**Platform:** Web

### How to Play

The game can be played [here](/docs/PT01-HelloWorld/index.html).

The goal of the game is to avoid oncoming alien spaceships. Your spaceship can be moved using WSAD (up, down, left, right respectively). **Note** that touch input isn't supported.

### Notes

I experienced a strange issue in which the player ship always collided with itself. Maybe this is the way I constructed up the player entity? As a workaround, in *PlayerCollisionSystem* I ensure that the player isn't colliding with itself (using the overlapped otherEntity index).
