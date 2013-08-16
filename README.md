#pullall

Update a group development env of node modules

So you are developing `projectA`, a project with a lots of small Node modules.

Run pullall in the directory where you have cloned the modules.
For each module, if the directory is clean (no uncommited changes),
the script will update the source, check if `package.json` has
changed and if so, `npm install` all dependencies, `npm link` gobally, and
`npm link` to dependencies which you also have on that same folder.

## Installation

    $ npm install pullall -g

## Usage

    $ cd project # the place you have lots of cloned repos
    $ pullall
