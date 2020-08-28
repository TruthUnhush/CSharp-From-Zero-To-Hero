# C#: From Zero To Hero

## Chapter 4: TDD

### Lesson 1: Arrange, Act, Assert

#### Intro

Tests are a way of not only double checking if our code works, but also a way of having a living documentation.
It's hard to express in short how much tests help: easy check if all works, good design enforcements, documentation, fun to experiment...
It's time for you to play!

##### 3A



###### Arrange

Set things up. The first step for every test case. If input needs to be formed, component initialized, it should happen in this step. Sometimes, a test case might not have it and the reason is simply because either you're testing a stateless static function that needs no input, or the system itself was already initialized in Setup stage.

###### Act

Interact with the sut (system under test). Do 1 thing, no more, no less. Must happen in every test.

###### Assert

Check the output, verify that the expectation did happen. Every tests should have at least 1 assert, sometimes more. More than 1 assert is not recommended and if you can do something about reducing the number of asserts, then please do, because it breaks readability of tests. However, don't break tests into parts, just to test one thing. If test actually caused many things to happen, then verify the outcomes all in one test.

#### Task

Unit test ``/Gambling/GameComponents``.
