# Reading 03

- When should you use an unordered list in your HTML document?
  - To make a list with items of the same importance.
- How do you change the bullet style of unordered list items?
  - list-style-type
- When should you use an ordered list vs an unorder list in your HTML document?
  When you want to organise items in order of importance or to give instructions, for example.
- Describe two ways you can change the numbers on list items provided by an ordered list?
  - list-style-type or type(a,A,i,I,1). First is preferred.
- Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box - Model”?
  - The padding surrounds the content and the margin surrounds the border.
- List and describe the four parts of an HTML elements box as referred to by the box model.
  - Content box: The area where your content is displayed; size it using properties like inline-size and block-size or width and height.
  - Padding box: The padding sits around the content as white space; size it using padding and related properties.
  - Border box: The border box wraps the content and any padding; size it using border and related properties.
  - Margin box: The margin is the outermost layer, wrapping the content, padding, and border as whitespace between this box and other elements; size it using margin and related properties.
    (https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)
- What data types can you store inside of an Array?
  - Strings, numbers, booleans and other arrays.
- Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
  - I don't think it is valid because there is a falsy value inside, but not sure. If it is valid, you can access the items inside using indexOf() or people[index number from 0].
- List five shorthand operators for assignment in javascript and describe what they do.
  - x = f() --> assigns a value to x
  - x += f() --> f() is equal to f() plus x
  - x -= f() --> f() is equal to f() minus x
  - x \*= f() --> f() is equal to f() times x
  - x /= f() --> f() is equal to f() divided by x
- Read the code below and evaluate the last expression and explain what the result would be and why.
  - The result is "10dog". You can't add a boolean to a number, so JS puts 10, which is read as a string, and dog together as a string.
- Describe a real world example of when a conditional statement should be used in a JavaScript program.
  - You can check if someone has written the correct password. If the password stored matches the password written, allow logging in.
- Give an example of when a Loop is useful in JavaScript.
  - You can use loops to repeat a condition. For example, to make sure hte user only uses numbers in an answer.
