<!-- BEGIN general-rules: managed by grip-build-scripts, do not edit here -->
# Writing rules for documentation and code comments

All documentation, code comments, commit messages, and pull request descriptions in this repository follow these writing rules. Many readers do not speak English as a first language. Write so that they can understand you the first time.

These rules apply to humans and to AI agents.

## Sentence rules

- Write procedural sentences with 20 words or fewer.
- Write descriptive sentences with 25 words or fewer.
- Put one idea in each sentence.
<!-- vale off -->
- Write one instruction in each sentence. Use the imperative form: "Close the valve." Do not write "The valve should be closed."
<!-- vale on -->
- Start a procedure step with a verb.
- Keep paragraphs to six sentences or fewer. Start each paragraph with its main topic.
- Put a warning or caution before the step it applies to.

<!-- vale off -->

## Word rules

- Use the active voice. Use the passive voice only when the actor is not known or not important.
- Use the simple present tense for descriptions and the imperative for instructions. Avoid the perfect tense, the progressive tense, and the future tense when a simple tense works.
- Use each word with one meaning only. If a word has two meanings, use it with the common meaning and choose a different word for the other.
- Use each word as one part of speech only. Do not use "test" as a verb in one place and a noun in another when a different word is clear.
- Use "must" for a required action. Use "can" for ability. Do not use "should", "may", or "might" to give instructions.
- Use a short, common word. Write "use", not "utilize". Write "start", not "commence". Write "show", not "demonstrate".
- Do not use phrasal verbs when a single verb is clear. Write "remove", not "take out". Write "continue", not "go on".
- Do not use idioms, slang, humor, or figures of speech.
- Do not use contractions. Write "do not", not "don't".
- Spell out an abbreviation the first time you use it. Keep the same term for the same thing in the whole document. Do not use synonyms.
- Do not use a long noun cluster. Write "the file that stores the user settings", not "the user settings storage file". Keep a noun cluster to three words or fewer.
- Include the word "that" or "which" when it makes the sentence clearer.

<!-- vale on -->

## Technical terms

- Use the exact name of a function, command, file, or setting. Put code names in code formatting.
- Do not rename a thing in the prose to make it sound better. Repeat the same name.

## Language order

- Name the four languages in this order: Python, Node.js, Rust, YAML.
- Use the labels `Python`, `Node.js`, `Rust`, and `YAML`. Do not write "Node" or "JS".
- Apply the order to prose, tabs, comments, docstrings, path globs, and lists in code.
- Check each new list of languages against this order.

## Code comments

- Explain why the code does something, not what the syntax does.
- Write each comment as a complete sentence with 20 words or fewer.
- Write the comment in the present tense.
- Do not leave a comment that repeats the code.

<!-- vale off -->

## Examples

Avoid: "You might want to go ahead and make sure that the config file's been properly set up before you kick off the build."

Write: "Make sure that the configuration file is correct. Then start the build."

Avoid: "This function is utilized for the purpose of validating user-supplied input."

Write: "This function checks the input from the user."

<!-- vale on -->

## Before you finish

- Read each sentence. Split it if it has more than one idea or more than the word limit.
- Run `vale sync`, then run `vale` on each Markdown file that you change. Fix each error.
- If a rule makes the text unclear, keep the text clear and add a short note in the pull request.
<!-- END general-rules -->
