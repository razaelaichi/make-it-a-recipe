## ★ make-it-a-recipe ★
# Recipe Explainer Skill

Sometimes, technical concepts and algorithms can be tough to wrap your head around. The Recipe Explainer is an AI prompt template designed to break down complex or abstract coding concepts by turning them into easy-to-follow cooking recipes.

By mapping technical elements to familiar culinary equivalents, it provides an analogy framework that makes hard-to-grasp ideas a lot more memorable.

## Why it works

The prompt enforces a few strict rules to make sure the analogy actually helps rather than confuses:
- **Consistent Metaphors:** It maps inputs to ingredients, loops to repeated actions (like stirring), functions to tools, and errors to cooking mistakes. 
- **Predictable Structure:** Every explanation reads just like a real recipe. It includes the yield, a list of ingredients (variables), and step-by-step instructions.
- **Handles Complex Logic:** It's built to explain not just simple scripts, but also complex logical paths like recursion and backtracking.

## How to trigger it

If you're using an AI assistant loaded with this skill, you can ask for an explanation using phrases like:
- "Explain this like a recipe"
- "Make this a recipe"
- "Teach me this as cooking"
- "Write this as a recipe"

It can also just step in if you express confusion about a concept and it thinks an analogy would naturally help.

> **Note:** While this prompt works with various AI models, it is best used with **Claude**, which is particularly strong at rigidly following the structural rules and maintaining the culinary metaphor.

## How the mapping is handled

Behind the scenes, the skill translates programming concepts into cooking terms before writing out the explanation:
* Inputs and Data become ingredients.
* Variables and State become bowls, containers, or temperature settings.
* Functions and Methods become kitchen tools or actions (mix, chop, bake).
* Loops become repeated actions (like "stir continuously").
* Conditionals become "taste and adjust" decisions.

### What you get back

Every response uses a strict structure:
1. **Title:** The name of the dish.
2. **Yield & Prep Time:** A fun nod to algorithmic complexity (e.g., `Prep time: O(n)`).
3. **Description:** A plain-language summary of what the "recipe" does.
4. **Ingredients:** The inputs, variables, and constraints you need.
5. **Instructions:** Step-by-step actions with clear reasoning attached to each step.

## Example Usage

**Prompt:** "use this skill and teach me insertion sort"

**Answer:**

### Sorting Stew (Insertion Sort)

Yields: 1 sorted list | Prep time: O(n²) worst case

**Description**

This recipe takes an unsorted list and gradually builds a perfectly sorted dish by inserting each element into its correct position.

**Ingredients**
- 1 list of elements (array): The data you want to sort
- 1 index pointer (i): Tracks the current element being inserted
- 1 key element: The item currently being positioned correctly
- 1 comparison pointer (j): Moves backward to find the right spot
- Constraint: Elements before index i are always sorted

**Step-by-Step Instructions**

1. **Preheat the Sorted Section**
   - **Action:** Assume the first element (index 0) is already sorted.
   - **Reason:** A single element is always sorted, so this forms your starting base.

2. **Pick the Next Ingredient**
   - **Action:** Move to the next element (i = 1) and store it as the key.
   - **Reason:** This is the element you will insert into the sorted portion.

3. **Compare Backwards**
   - **Action:** Set j = i - 1 and compare the key with elements before it.
   - **Reason:** You need to find the correct position for the key in the sorted section.

4. **Shift Larger Elements**
   - **Action:** While j >= 0 and array[j] > key, shift array[j] one step to the right.
   - **Reason:** This creates space for the key by moving bigger elements ahead.

5. **Insert the Key**
   - **Action:** Place the key at array[j + 1].
   - **Reason:** This is the correct sorted position after shifting.

6. **Repeat the Process**
   - **Action:** Move to the next index (i++) and repeat steps 2–5.
   - **Reason:** Each iteration expands the sorted portion until the whole list is sorted.

**Chef’s Notes**
- If the list is already sorted, this runs very fast: O(n).
- Worst case happens when the list is reverse sorted: O(n²).
- This algorithm is stable, meaning equal elements keep their original order.
- It works well for small datasets or nearly sorted lists.

## License
MIT
