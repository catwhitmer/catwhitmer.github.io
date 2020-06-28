---
layout: post
title:      "What is Self?"
date:       2020-06-28 14:09:53 +0000
permalink:  what_is_self
---

Self is a nifty little keyword in Ruby that is very confusing at first, but once understood it can be extremely helpful. Self basically represents the current object viewed in different context. It also really helps in keeping your code DRY and easier to read.

**How to use self**



**Class Method**

In a class, self represents the class itself. For example, if you are in a User class, it will always point to the user. It can be thought of as a substitution of the class name.

```
class User
  self
end

=> User
```

But if you define a method inside a class named Author, then self would be the Author object.
```
class Author
  def write
    puts self
  end
end

Author.new.write
#<Author:0x6s14c7>
```

It can also be used to define class-level methods.
```
class Author
  def self.write_a_book
      ....
    end
end

Author.write_a_book
```

**Instance Method**

In an instance method, self is representing the instance of that class and can only be called on instances.

```
class User

  def name   #instance method
    puts "#{self}"
  end

end

user = User.new   #new instance
puts "The user's name is: #{user.name}"
```

**Other Uses**

Self is also very useful in other ways such as:

* Debugging
* Comparing objects (==)
* Default receiver of method calls

If you are stuck and cannot figure out why your code is not working, try self to debug.

