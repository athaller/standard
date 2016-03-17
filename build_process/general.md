# General Best Practices

## NPM Scripts

Our projects use different build systems (Gulp, Grunt, custom, etc), but many times they have tasks that do
similar things on every project. As developers move from project to project we can save some cognitive overhead by 
standardizing the commands we use for these common tasks. Since most of our build systems are built on node
and npm we can use [npm scripts](https://docs.npmjs.com/misc/scripts) as shortcuts to our various common tasks.

- `npm start` - This default script should be reserved for tasks that execute a server in a deployed environment
- `npm run dev` - For a task that runs a local development build with watches and an optional local server
- `npm run prod` - For a task that runs a production build
- `npm run test` - For a task that runs the projects tests
- `npm run help` - For listing all available build tasks for this project

