1. What is inheritance?
2. What is polymorphism?
3. What is composition?
4. What is an abstraction in ruby?

- Polymorphism //  duck typing : when different sub classes of another class have different methods
- Abstractions are when methods are called from the parent, but are abstracted--changed--so that the contents of the child method are different from the parent.

```ruby
class Mom
    def smile
        :knowing_smile
    end
end

class Child
    def smile
        super
        :innocent_smile
    end
end
```
