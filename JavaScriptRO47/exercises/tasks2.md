# Advanced Sass Exercises

These exercises focus on more advanced Sass features like deeper nesting, loops, conditionals, complex mixins, and functions. You should be familiar with basic Sass concepts before attempting these exercises.

---

## Exercise 11: Responsive Grid Mixin

### Goal:
Create a mixin to generate a responsive grid layout.

### Task:
1. Create a mixin `grid` that accepts the number of columns and gap size as arguments.
2. Use the mixin to generate `.container` and `.item` classes that handle grid layout and gaps.
3. Add a media query within the mixin to adjust the grid for smaller screen sizes.

### Tip:
Using media queries inside mixins allows you to create responsive layouts without repeating code.

---

## Exercise 12: Looping with `@each`

### Goal:
Generate utility classes for text colors dynamically.

### Task:
1. Create a map of colors (`$colors: (primary: #3498db, secondary: #2ecc71, danger: #e74c3c)`).
2. Use `@each` to loop over the map and generate text color utility classes (`.text-primary`, `.text-secondary`, etc.).
3. Apply these classes to different elements to change text color.

### Tip:
Maps and loops together allow for highly dynamic CSS generation, reducing redundancy in utility classes.

---

## Exercise 13: BEM (Block Element Modifier) with Nesting

### Goal:
Implement a component using the BEM methodology.

### Task:
1. Create a `.card` block with nested elements `.card__header`, `.card__body`, and `.card__footer`.
2. Use modifiers like `.card--primary` and `.card--secondary` to change the appearance of the card.
3. Nest the elements and modifiers to keep the structure organized.

### Tip:
BEM combined with Sass nesting keeps your styles modular and easier to scale.

---

## Exercise 14: Conditional Mixins with Default Parameters

### Goal:
Write a mixin that conditionally applies styles based on passed parameters.

### Task:
1. Create a mixin `button` that accepts a color and a default argument `$is-rounded: false`.
2. If `$is-rounded` is true, add `border-radius` to make the button rounded.
3. Apply the mixin to different buttons with and without rounded corners.

### Tip:
Default arguments and conditional logic inside mixins can make them more flexible and reusable.

---

## Exercise 15: Generating Multiple Classes with `@for`

### Goal:
Create multiple width utility classes using a loop.

### Task:
1. Use a `@for` loop to create width utility classes from `.w-10` to `.w-100` where the number corresponds to percentage width.
2. Each class should apply a `width` property based on the loop index (e.g., `.w-10 { width: 10%; }`).
3. Ensure that all width classes are generated dynamically.

### Tip:
Loops in Sass can significantly reduce repetitive tasks and make generating classes easier.

---

## Exercise 16: Advanced Functions and Color Manipulation

### Goal:
Create a function to calculate complementary colors.

### Task:
1. Write a function `complementary-color` that accepts a color and returns its complement.
2. Use this function to apply a background color to `.btn` and use the complementary color for the text color.
3. Experiment with different colors and their complements.

### Tip:
Using custom functions in Sass allows you to manipulate values (like colors) and produce dynamic styles.

---

## Exercise 17: Placeholder Selectors with `%`

### Goal:
Use `%` to create placeholder selectors and extend them in other classes.

### Task:
1. Create a `%button-base` placeholder that includes common button styles like padding, border, and font-size.
2. Extend `%button-base` in `.btn-primary` and `.btn-secondary` classes, adding unique styles for each (e.g., background-color).
3. Ensure that no unused CSS is generated for the placeholder.

### Tip:
Placeholders using `%` won't generate CSS on their own, but when extended, they help avoid repetition.

---

## Exercise 18: Nested Media Queries

### Goal:
Nest media queries within specific selectors.

### Task:
1. Create a `.content` class that styles a container with padding and text color.
2. Add a media query inside `.content` to change padding and text color for smaller screens.
3. Nest the media query to apply only within the `.content` class.

### Tip:
Nesting media queries helps scope your responsive styles to specific components, keeping your code organized.

---

## Exercise 19: Complex Mixin for Flexbox Layout

### Goal:
Create a mixin for generating complex flexbox layouts.

### Task:
1. Create a mixin `flex-layout` that accepts arguments for `justify-content`, `align-items`, and `flex-direction`.
2. Use this mixin to create `.flex-center` and `.flex-space-between` classes.
3. Apply the mixin to a few elements to create different layouts.

### Tip:
Using mixins for layout systems like Flexbox ensures that your layout styles are reusable and maintainable.

---

## Exercise 20: Theme Switching with Maps

### Goal:
Switch themes using Sass maps.

### Task:
1. Define two theme maps: `$light-theme` and `$dark-theme` (containing colors for background, text, etc.).
2. Create a function `theme-color` that retrieves a color from the appropriate theme map based on a `$current-theme` variable.
3. Use the function to apply theme-based background and text colors to your `.container`.

### Tip:
Maps and functions in Sass are powerful tools for managing themes dynamically without duplicating a lot of code.

---

## Conclusion

These advanced exercises will help you dive deeper into the power of Sass. By leveraging features like maps, loops, conditionals, functions, and mixins, you can write more efficient, scalable, and maintainable CSS.

Happy Coding!