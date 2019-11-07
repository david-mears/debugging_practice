(This is a temporary place to store this exercise until [this PR](https://github.com/makersacademy/skills-workshops/pull/58) is merged.)

# Debugging Practice

## Learning Objectives 
- Apply the mantra 'tighten the loop, gain visibility'
- Debug a simple application

## Introduction 

In the [previous exercise](https://github.com/makersacademy/skills-workshops/blob/master/practicals/debugging/debugging_approaches.md) you were introduced to a bug fixing approach that we'll call 'tightening the loop and gaining visibility'.

Tightening the loop refers to the process of singling out exactly where in your code a bug is hiding, gaining visibility means 'looking into' this area of your programme by printing out values.

Let's practice applying this approach with another example.

## Exercise

Before we get started, lets set up a directory and a ruby file for the project:

```bash=
$ mkdir broken-fizzbuzz 
$ cd broken-fizzbuzz
$ touch fizzbuzz.rb
```

Once you've done this, open the file in your text editor, copy and paste the code below into it, then save.

```ruby
class FizzBuzz
  def play(number)
    return "fizz" if is_divisible_by(num, 3)
    return "fizzbuzz" if is_divisible_by(num 15)
    return "buzz" if is_divisible_by(num 5)
    number
  end

  def is_divisib1e_by(number, divisor)
    number / divisor == 0
  end
end


fizzbuzz = FizzBuzz.new
(1..100).each do |number|
  puts fizzbuzz.play(number)
end
```

You should now be able to run the file using irb:
```bash=
$ irb
$ require './fizzbuzz'
```

Follow the process you developed in the previous exercise in order to eliminate the bugs in this programme.  

Remember - your job is **not** to fix the code, but rather to **uncover** why the code is not working. Fixing the problems will be a happy side effect.
