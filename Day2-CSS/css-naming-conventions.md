
# Semantic Naming:
Use class names that describe the purpose of the element.
example:
.header {}
.menu {}
.btn {}

# Hyphen Delimited (or Kebab Case):
Separate words with hyphens (-).
example:
.btn-primary {}
.header-top {}
.sidebar-menu {}

# Avoid Camel Case and Underscores:
Instead of camelCase or snake_case, use hyphens for word separation.
example:
/* Not recommended */
.btnPrimary {}
.header_top {}

/* Recommended */
.btn-primary {}
.header-top {}
Avoid ID Selectors:

# Use classes over IDs for styling. IDs have higher specificity and are harder to override.
example:
/* Not recommended */
#sidebar {}

/* Recommended */
.sidebar {}

# Prefixes for Component Names:
Use prefixes to group related styles together.
example:
.btn {}
.btn-primary {}
.btn-secondary {}

# Avoid Non-Semantic Names:
Choose class names based on what the element is, not how it looks.
example:
/* Not recommended */
.red-text {}

/* Recommended */
.error-message {}

# Short and Meaningful:
Keep class names short but descriptive.
example:
.btn {}
.nav {}

# Use Abbreviations with Caution:
Only use abbreviations if they are widely understood and make the code more readable.
example:
/* Not recommended unless widely understood */
.btn {}
.nav {}

/* Recommended */
.button {}
.navigation {}
Following these basic naming conventions will help you write cleaner and more maintainable CSS code.
