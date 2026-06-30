Steps to create and configure a new project:
- Create a new turbo repo project: bunx create-turbo@latest {{project-name}} --example basic --package-manager bun
- Remove apps/** folders: rm -rf apps/*
- Move to apps folder
- Create frontend project: bun create next-app frontend --src-dir --use-bun
- Create backend project: bun create elysia backend
- Change package names in package.json of each project, adding to this patter: @{{namespace}}/{{module}} ex: @myproject/backend
