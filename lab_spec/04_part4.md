# Import is Important Tutorial
## Lab: Animal Classification System

### Part 4: Complete the Classification System

![Vertebrates Classification Diagram](../.devcontainer/vertebrates.png)

#### Task 4.1: Implement All Animal Modules
Expand your package to include **two animals each** from **at least three** of the five classifications the vertebrates classification system diagram above, for a total of **six animal modules**. Each animal should:
1. Be represented as its own module
1. Have access to its classification's shared attributes
1. Have the three unique attributes specific to that animal species from the classification diagram
1. Use a variety of different import methods, including the following:
   * absolute imports
   * relative imports
   * the `from <module> import ..." structure
   * adding imports to `__init__.py`
   * modularizing code where it's beneficial and importing into the original files

**Stretch Goal:**
Complete all modules for all 10 animals in the vertebrates classification system.

##### Success
You'll know you succeeded when:
1. You have 6 - 10 animal modules (2 per classification)
2. Each animal module can be imported without errors
3. Each animal has access to its classification's shared attributes without copying them into each animal's module

#### Task 4.2: Make Everything Accessible
For each classification package, configure the package initialization so that:
1. All individual animal modules can be accessed through the package
1. All shared attributes can be accessed at the package level
1. The import paths are as readable and clear as possible for users of your package

##### Success

**NOTE:** Your choices regarding where the attributes are stored will change the package and module structure. Therefore, your imports may not look exactly like the examples shown below.

You'll know you succeeded when:
1. You can import a classification and access individual animals through it
2. Shared attributes are accessible at the package level
3. The challenge examples `fish.shark.has_scales` and `fish.has_scales` both work

**Challenge:** Modify your imports so someone can write `import vertebrates.cold_blooded.fish as fish` and then access both `fish.shark.has_scales` and `fish.has_scales`.

---

Next Up: [**Stretch Goal** Part 5: Reflection](05_part5.md)