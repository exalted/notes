README
======

* Ambiguity *sucks*, there must be only one _right_ way to do it
* `is` and `are` keywords are synonyms
* `,` and `and` keywords are synonyms
* `: ... end` is a _block_
* `( ... )` anything in between is a comment (multiple lines)
* _Everything_ is an object, nothing is special
* [MoSCoW Method](http://www.projectsmart.co.uk/moscow-method.php)
* `.` is an empty block
* If something is not "defined" yet, you can't "use" it

================================================================================

```
Requirements for Human:
  - Must say something
end

Definition of OrdinaryPerson as Human:
  say something:
    (says something exactly once)
  end
end

Requirements for Climber as OrdinaryPerson:
  say something:
    repeat "OrdinaryPerson.say something" n-times
  end

  - Could echo n-times
end

Definition of MountainClimber as Climber:
  echo: 7
end

Definition of RoofClimber as Climber:
end
```
