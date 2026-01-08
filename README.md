# sppr

## Key Endpoints

* ingredient autocompklete
* Find me recipes with X criteria
  * cook time (maybe just a sort to start)
  * ingredients I have
    * match by as few ingredients I don't have
  * ingredients I don't want to use
  * ingredients we assume you have
* Oh and also I want to do a soup builder part where you're like I want to start with a broth base and I want something with rice and I want it to have chicken


## Arch decisions

### Infrastructure

* Data store
  * postgres instance
  * Opensearch indexes
* FE and BE frameworks
  * golang api
* Hosting

  
### BE design

* API layer
* Index/ingestion layer
* Authentication/Accounts


### FE design

* framework
* FE vs BE rendered
* can't be a static site bc it needs to fetch recipes

## Data Structure Thoughts

This could also work as a NoSQL database that's just recipes
Ooooh it could be an Elasticsearch instance to let us practice our search work

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

### Style(s)

### Region(s)

THEN WE CAN RENDER A MAP OF THE WORLD TO SHOW REGIONAL SOUPS

### Ingredients

* name
* category (another bridge table?)

#### Ingredients to recipe

* soup_id
* ingredient_id
* quantity (numeric)
* unit (string or enum)
* addtl_notes
* substitution_notes


### Tags

Want to tag soup styles & regions (chowder, 
Something to flag recipes/ingredients as vegan, vegetarian, gluten, dairy, alcohol, various allergens, etc

### Accounts

so you can define your "I have this already" ingredients


