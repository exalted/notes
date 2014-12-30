Notes
-----

* Ambiguity *sucks*, there must be only one _right_ way to do it
* `is` and `are` keywords are synonyms
* `,` and `and` keywords are synonyms
* `:<indentation>...` is a _block_
* `( ... )` anything in between is a comment (multiple lines)
* _Everything_ is an object, nothing is special
* [MoSCoW Method](http://www.projectsmart.co.uk/moscow-method.php)
* `.` is an empty block
* If something is not "defined" yet, you can't "use" it
* Syntax shall not be _not_ case sensitive, but the script is
* Last argument of a method definition can be used either as an input value or a return value

Code Example
------------

```
Requirements for Human:
  - Must say something

Definition of OrdinaryPerson as Human:
  Say something:
    (says something exactly once)

Requirements for Climber as OrdinaryPerson:
  Say something: (this is a method override)
    (... but then we can explicitly call another implementation: (e.g., `like OrdinaryPerson`))
    Repeat "say something" like OrdinaryPerson n-times

  - Could echo n-times or "say something" like OrdinaryPerson

Definition of MountainClimber as Climber:
  Echo: 3 (this is a single line block)

Definition of RoofClimber is Climber.
```

Fake REPL
---------

```
> john as OrdinaryPerson say "Hello, World! ;-)"
(this prints "Hello, World! ;-)" exactly once)

> clark is MountainClimber
> clark say "Is anybody out there?"
(this prints "Is anybody out there?" three times)
```
