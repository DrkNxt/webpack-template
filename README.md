# webpack-template

## Do immediatly

Change `insert-name-here` in `package.json` and `package-lock.json` to repo name

Run `npm install` to install all dependencies

## Dev Server

`npm run dev` to start dev server

`Ctrl+C` to close dev server

## Deployment

If this is the first deployment: `git branch gh-pages`

Do the following in order for every deployment:

1. Commit all edits
2. `git checkout gh-pages && git merge main --no-edit`
3. `npm run build`
4. `git add dist -f && git commit -m "Deployment commit"`
5. `git subtree push --prefix dist origin gh-pages`
6. `git checkout main`
7. Set GitHub Pages source branch to `gh-pages`
