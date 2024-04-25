## Password Policies
# Task: 
Create a class named Policy with the following specifications:
- the class must contain 1 protected attribute named isChecked of type boolean.
- the class must contain 1 purely virtual public method called check. It must not return anything, and as a parameter it must receive a std::string (the password you need to check) as a constant reference.
- The class must contain a public method without any parameter called getCheck, which must return the isChecked attribute. The method must be declared const qualified.

Create a class named LengthPolicy with the following specifications:
- the class must be inherited from the Policy class.
- the class must contain 2 private attributes named minLength and maxLength, these being 16-bit unsigned integers.
- the class must contain a public constructor with 1 parameter, which initializes the minimum with the given value and the maximum with the value 255.
- class must contain a public 2-parameter constructor, which initialises the minimum and maximum with the given values.
- classes must implement the check method of the base class. It must check what is specified in the requirement.

Create a class named ClassPolicy with the following specifications:
- the class must be inherited from the Policy class.
- the class must contain 1 private attribute called minClassCount, which is a 16-bit unsigned integer.
- the class must contain a public constructor with 1 parameter, which initialises the attribute with the specified value.
- classes must implement the check method of the base class. It must check what is specified in the requirement.

Create classes named IncludePolicy and NotIncludePolicy with the following specifications:
- the classes must be inherited from the Policy class.
- the classes must contain 1 private attribute named characterType, which is of type char.
- the classes must contain a public constructor with 1 parameter, which initialises the attribute with the specified value.
- classes must implement the check method of the base class. This must check what is specified in the requirement.

Create a classes named RepetitionPolicy and ConsecutivePolicy and with the following specifications:
- the classes must be inherited from the Policy class.
- the classes must contain 1 private attribute named maxCount, which is of type 16-bit unsigned integer.
- the classes must contain a public constructor with 1 parameter, which initialises the attribute with the specified value.
- classes must implement the check method of the base class. This must check what is specified in the requirement.

Write a function called checkPassword, which receives 2 parameters, the first of type std::string, representing the password you want to check, and the second a std::vector of objects of type Policy*, representing the policies read from the keyboard. The function must return a std::string that is either "OK" or "NOK", depending on the password.

