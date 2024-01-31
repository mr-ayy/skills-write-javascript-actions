# skills-write-javascript-actions

## My Joke Action

My Joke Action, created as part of the Microsoft [Create Custom GitHub Action Exercice](https://learn.microsoft.com/en-us/training/modules/create-custom-github-actions/exercise-create-custom-action). Original repository this was cloned from can be found on [skills/write-javascript-action](https://github.com/skills/write-javascript-actions).

This action provides the following functionality for GitHub Actions users:

* Provides a joke using the [icanhazdadjoke](https://icanhazdadjoke.com/) API.
* Prints and provides the joke as part of `output.joke-output`

## Basic Usage

See [action.yml](action.yml).

```yaml
steps:
  - id: joke
    name: My Joke Action
    uses: mr-ayy/skills-write-javascript-actions@v2

  - run: echo "${{ steps.joke.outputs.joke-output }}"
```
