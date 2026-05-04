## make-it-a-recipe :3
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

## License
MIT
