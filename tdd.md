TDD & JavaScript
===

Who?
===

Joscha Meyer
Robert Kowalski

@OschenPoschen
@robinson_k

(Wer macht unit tests und wer macht sie für javascript)

Why Jimdo <3 TDD?
===

What do we have?
===

### Long living product - long living code

### Fast changing requirements - fast changing code


Why Jimdo <3 TDD?
===

### Less bugs

### Speed up

### Proven functioniality


What is TDD?
===

Unit Tests
===

### Avoid regressions

### Feedback (Continous, fast (F5, Clickpath))


What is TDD?
===

### Red

### Green

### Refactor

Why Red Green Refactor
===

### Describe the expected behaviour (name of test)

### Think about result (implement expectation)

### Green! (implement solution as fast as possible)

### Make it DRY (refactor)

### => Validated tests

QUnit Test
===

<% code do %>
test('firstLower lowers the first character', function() {
    var cc = new CC();

    var result = cc.firstLower('FirstToLowerString');

    strictEqual(result, 'firstToLowerString');
});
<% end %>

<% code do %>
test('firstLower should keep lower first characters', function() {
    var cc = new CC();

    var result = cc.firstLower('firstToLowerString');

    strictEqual(result, 'firstToLowerString');
});
<% end %>

Stubbing and Mocking
===

### Stubs: Fake Implentations (return values)

### Mocks: Like Stubs, but with expectations

Stub: Example
===


Do's and don'ts
===

### One assertion per test

### Tests should be living docs

### Test the communication with other Objects, don't test dependencies (external libraries, DOM)

### If you cannot test it, fake it

Further "Reading"
===

 * Test Driven Development: By Example - Kent Beck
 * Test-Driven JavaScript Development - Christian Johansen
 * http://www.cleancoders.com/ Screencasts
 * Working Effectively with Legacy Code - Michael Feathers