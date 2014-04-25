# Excalibur.js Site

## Contributing Content

All authored tutorials and documentation is under `content/docs`. Data is under `data`.

## Getting Started

### Requirements

- Node.js (0.10.x)
- Windows or Unix-like

Once you've cloned the repository, run the following commands:

    # If not already installed, install grunt globally
    npm install grunt -g

    # Install dependencies
    npm install

    # Run site for local development
    grunt design

We recommend using the free [Brackets](http://brackets.io) editor since it's easy to use and works on any platform.

## Deploying

If you're a core contributor, it's easy to push the site to GitHub. Just run:

    grunt deploy
    
You may need to type in your credentials, but after that the production site will be updated.

**Tip:** Don't do this if you don't want the latest changes to be public!

## Adding to Showcase

Edit the `showcase.json` file in `data`. Upload an image to `assets/images/showcase` as a PNG.

### Git Submodules

If the showcase is in Git and can be run in a sub-directory, you can initialize
a submodule in the `showcase` directory.

    git submodule add {clone url} showcase/{showcase name}
    
Example:

    git submodule add https://github.com/eonarheim/Excalibur-Shmup showcase/shmup
    
This is how we can include the Shoot 'Em Up demo without maintaining two versions.