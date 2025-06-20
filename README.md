# ai-routines
Creating natural-language Routines in AI IDEs like Cursor, Etc.

NOTE: This repo is part of a project to create AI Routines in various IDEs.  Because it's believed that there will be enough differences between IDEs - because of that, there will be one repository per IDE.  This 'top-level repo' will document the project and contain 'downlinks' to the repos for individual IDEs.

## The project
### What We Mean By 'Routines'
Development teams often create or adopt scripts (e.g., shell scripts, Node-based tools like Grunt, Gulp, Yeoman, npm scripts, or language-specific CLIs) to automate repetitive or routine tasks such as:

# scaffolding project components (e.g., yo generators)

compiling/transpiling code

starting/stopping local dev servers

running tests and linters

deploying code

syncing environments or updating dependencies

These scripts are usually invoked from within the context of a project, and most commonly:

Through a terminal embedded in the IDE (e.g., VS Code terminal)

Sometimes via custom buttons or tasks in the IDE (e.g., VS Code tasks.json, WebStorm run configurations)

Occasionally integrated into the project's package.json or build configuration (so they can be run with npm run something, make, etc.)

This kind of setup helps to enforce consistency, save time, and reduce onboarding friction for new developers.
