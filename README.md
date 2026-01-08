# sppr

## Key Endpoints

* Find me recipes with X criteria
  * cook time (maybe just a sort to start)
  * ingredients I have
    * match by as few ingredients I don't have

## Arch decisions

* Data store
* FE/BE frameworks
* Hosting

## Data Structure Thoughts

### Recipe

* name
* description
* active_cook_time_mins
* total_cook_time_mins
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
