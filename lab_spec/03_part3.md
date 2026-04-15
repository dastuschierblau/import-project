# Import is Important Tutorial
## Lab: Animal Classification System

### Part 3: Package-Level Imports with `__init__.py`

Right now, access to attributes for a specific fish requires importing the full path to that fish. Let's explore how `__init__.py` can control what's accessible when you import a package.

#### Task 3.1: Make Modules Accessible at Package Level
**Goal:** Import the fish package into `main.py` and access individual fish (like shark) through it, without having to import the full path to each fish.

**Experiment:**
1. Try importing just the `fish` package into `main.py` and access the `shark` module through it. Try both absolute and relative imports. 
2. If this doesn't work initially, research how `__init__.py` can help
3. Modify the appropriate `__init__.py` file to make individual fish modules accessible

##### Reflection
- What happens when you import a package?
- What role does `__init__.py` play in controlling access?

#### Task 3.2: Make Attributes Accessible at Package Level
**Goal:** Access shared fish attributes (like `has_scales`) directly from the `fish` package, not just from individual fish modules.

**Experiment:**
1. In `main.py`, try accessing a shared attribute directly from the `fish` package without going through `shark`
2. If it doesn't work, figure out what you need to add to `__init__.py`
3. Make it so attributes are accessible at multiple levels (both from the package and from individual modules)

##### Reflection
- At how many different levels can you now access `has_scales`?
- Draw or describe the namespace hierarchy
- What are the benefits and drawbacks of making attributes available at multiple levels?

---

Next Up: [Part 4: Complete the Classification System](04_part4.md)

