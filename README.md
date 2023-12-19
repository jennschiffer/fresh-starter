# Fresh project

Your new Fresh project is ready to go. You can follow the Fresh "Getting
Started" guide here: https://fresh.deno.dev/docs/getting-started

### Usage

Make sure to install Deno: https://deno.land/manual/getting_started/installation

Then start the project:

```
deno task start
```

This will watch the project directory and restart as necessary.

### Remix and deploy from Glitch to Deno Deploy

1. Create a Fresh project from [Deno Deploy](https://dash.deno.com/projects) assigned to a Github repo
2. Remix your Github repo by going to https://glitch.new/github/GITHUBUSERNAME/GITHUBPROJECT
3. add `.deno/` to .gitignore and add the contents of `glitch.json` so Glitch knows how to run
4. Open the Glitch terminal and update the Git commands in the next section to set your remote to be the Github repo of your Deno Deploy project
5. Install deno in the terminal using the [Shell instructions in their docs](https://docs.deno.com/runtime/manual/getting_started/installation) and follow the directions in the Terminal for setting the export path. Note: you'll probably need to boost your Glitch app so you get more disk space here.

#### Git commands Jenn ran
1. `git remote add gh https://github.com/USERNAME/PROJECT.git` I called my remote gh because github
2. `git pull gh` (and then fix any conflicts)
3. `git branch first-update && git checkout first-update`
3. `git push gh master: main`