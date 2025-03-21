## Exercise 1: Using Variables

### Goal:
Define variables for colors and font sizes, and use them to style a button.

### Task:
1. Define a `$primary-color` variable for the button background.
2. Define a `$font-size` variable for the text size.
3. Use these variables to style a `.btn` class with padding, background color, and font size.

### Tip:
Variables help you maintain consistency and make changes to your design easily across the project.

---

## Exercise 2: Nesting Selectors

### Goal:
Practice nesting by styling a card component that contains a header and a body section.

### Task:
1. Style a `.card` class to have a border and padding.
2. Nest a `.card-header` inside the `.card` to style the title.
3. Nest a `.card-body` inside the `.card` to style the content area.

### Tip:
Limit your nesting to a few levels deep to avoid over-complicating your code. Aim for readability.

---

## Exercise 3: Partials and Importing

### Goal:
Organize your styles into different files using partials and `@import`.

### Task:
1. Create a `_variables.scss` partial and move all variables into this file.
2. Create a `_buttons.scss` partial and write button styles inside it.
3. In your main `style.scss`, use `@import` to include these partials.

### Tip:
Using partials and imports will keep your code modular and easier to maintain.

---

## Exercise 4: Inheritance with `@extend`

### Goal:
Use `@extend` to reduce repetitive styles.

### Task:
1. Create a `.base-btn` class with common button styles like padding, border, and font-size.
2. Create `.primary-btn` and `.secondary-btn` classes that inherit from `.base-btn`.
3. Add unique background colors for each of the button styles.

### Tip:
Use `@extend` to avoid repeating the same styles across different selectors.

---

## Exercise 5: Creating Mixins

### Goal:
Create a mixin for reusability in responsive design.

### Task:
1. Write a mixin called `responsive-text` that accepts a font size as an argument.
2. Use the mixin to adjust text sizes based on a media query.
3. Apply the mixin to your heading and paragraph styles.

### Tip:
Mixins can accept arguments and can make your code more flexible and reusable.

---

## Exercise 6: Using Functions

### Goal:
Write a custom function that manipulates colors.

### Task:
1. Create a function that lightens a color.
2. Use the function to lighten a background color in your `.btn` class.
3. Test different shades using the function to see its effect.

### Tip:
Functions allow you to create dynamic styles that are calculated at runtime. Explore built-in color functions in Sass, like `lighten()` and `darken()`.

---

## Exercise 7: Loops in Sass

### Goal:
Use loops to generate a series of classes.

### Task:
1. Use a `@for` loop to create 5 classes: `.margin-1` through `.margin-5`.
2. Each class should set a margin of 10px multiplied by the loop index (e.g., `.margin-1` would have `10px`, `.margin-2` would have `20px`, etc.).

### Tip:
Loops help you generate repetitive styles efficiently. This is particularly useful for utility classes.

---

## Exercise 8: Conditional Statements with `@if`

### Goal:
Use `@if` conditions to handle different themes.

### Task:
1. Define a variable `$theme` that can be either `light` or `dark`.
2. Write an `@if` statement that sets different background and text colors based on the theme.

### Tip:
Using conditional logic allows you to create theme-based styling in a clean and manageable way.

---

## Exercise 9: Mixin with Multiple Arguments

### Goal:
Create a mixin with multiple arguments for greater flexibility.

### Task:
1. Create a mixin called `box` that takes arguments for `width`, `height`, and `background-color`.
2. Use the mixin in two different classes, passing different values for each argument.

### Tip:
Mixins can take multiple arguments, making them a great tool for reducing repetitive code while keeping things customizable.

---

## Exercise 10: Using Built-in Sass Functions

### Goal:
Leverage built-in Sass functions for math operations.

### Task:
1. Create a class `.circle` that sets a `width`, `height`, and `border-radius`.
2. Use the built-in `percentage()` function to calculate the `border-radius` based on the height.

### Tip:
Sass provides a lot of built-in functions, including math, string, and color manipulation functions, that make complex styles easier to write.
