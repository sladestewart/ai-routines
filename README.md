# ai-routines
Creating natural-language Routines in AI IDEs like Cursor, Etc.

NOTE: This repo is part of a project to create AI Routines in various IDEs.  Because it's believed that there will be enough differences between IDEs - because of that, there will be one repository per IDE.  This 'top-level repo' will document the project and contain 'downlinks' to the repos for individual IDEs.

## The project
### What We Mean By 'Routines'
Development teams often create or adopt routines in the form of scripts (e.g., shell scripts, Node-based tools like Grunt, Gulp, Yeoman, npm scripts, or language-specific CLIs) to automate repetitive or routine tasks such as:
- scaffolding project components (e.g., yo generators)
- compiling/transpiling code
- starting/stopping local dev servers
- running tests and linters
- deploying code
- syncing environments or updating dependencies
- various other day-to-day tasks related to developing on a team

These scripts are usually invoked from within the context of a project, and most commonly:
- Through a terminal embedded in the IDE (e.g., VS Code terminal)
- Sometimes via custom buttons or tasks in the IDE (e.g., VS Code tasks.json, WebStorm run configurations)
- Occasionally integrated into the project's package.json or build configuration (so they can be run with npm run something, make, etc.)
- This kind of setup helps to enforce consistency, save time, and reduce onboarding friction for new developers.

### Where 'AI Routines' Fit In
The concept of 'AI Routines' (and also its 'sister concept' of 'AI Scripts') revolves around using AI to manage these.

#### AI Routine
The scripts that dev teams create are a specific 'flavor' of Routines, expressed in a specific formal language.  AI Routines are another 'flavor' - a Routine expressed in natural language.  It still has the concept of 'Steps' (and perhaps, as this project evolves - if it ends up making sense - other concepts from structured programming might get 'pulled in'), and it still has an algorighmic approach.  But the way it's expressed is in natural language.  This intends the following benefits
- To the appropriate extent, formal languages are removed from the equation - so that the current situation, where a dev might know one scripting language really well, others reasonably well, and quite a few others not well - but be required 'across the projects' to use a lot of different scripting languages, sometimes using them ineffectively - is ameliorated
- Guided creation, interpretation, and execution: The project intends for there to be Rules (a concept brought in from Cursor and - we anticipate - implemented in some form by just about every AI-enabled IDE) that guide both the AI and the user (dev) - and often a combination of both - in developing and executing effective and correct Routines.  When executing, the user has 'wiggle room' to use more or less precise language and the AI, along with these AI Routines and this standard, can figure out - perhaps by first engaging in conversation with the user as necesssary/appropriate and perhaps in an iterative process - what to execute/create/etc. i.e. 'what Routine to call and how to call it' or 'how to create the Routine'
- Discoverability: The standard for an AI Routine document supports 'self-documentation' and discoverability, essentially through the inclusion of YAML frontmatter sections with required and/or semi-required attributes/values.
- So (speaking concretely) the following prompts will accomplish what's intended by them
  - "Create a new Routine named Clean Up Database"
  - "Tell me about Routine Clean Up Database"
  - "Show me Routine Clean Up Database"
  - "List all Routines that are about cleaning up databases"
  - Help me to find a Routine we can run to clean up a database"

This project helps accrue these benefits by promulgating a minimal standard for the document comprising an AI Routine.  For a given AI-enabled IDE, this will likely (as mentioned above) be embedded in Rules.  To see this concretely 'in action', look at the 'Cursor AI Routines repo'.

