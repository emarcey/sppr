# sppr

## Data Structure Thoughts

### Recipe

* name
* description
* active_cook_time
* total_cook_time
* submitted_by
* created_at
* updated_at

#### Recipe steps

uq on recipe_id + iterator

Bridge tables to:

### Equipment

### Ingredients

#### Ingredients to recipe

* soup_id
* ingredient_id
* quantity (numeric)
* unit (string or enum)
* addtl_notes
* substitution_notes


### Tags

Something to flag recipes/ingredients as vegan, vegetarian, gluten, dairy, alcohol, etc
