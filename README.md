# Blazor Notes

A cheat sheet for the Blazor syntax I keep looking up. Mostly small `.razor` examples that are easy to copy into a project and adjust.

**[Live site](https://YOUR_USERNAME.github.io/blazor-cheatsheet/)** (replace this link after publishing)

## What's here

- Razor syntax, loops, and conditions
- Event handlers and two-way binding
- Parameters, callbacks, and reusable components
- Routing and navigation
- Forms and validation
- Lifecycle methods, dependency injection, and HTTP
- Render modes, JS interop, and common gotchas

The site has search, a copy button, favorites, and a light/dark switch. Favorites and the theme are saved in your browser. No account or backend needed.

## Run locally

You can open `index.html` directly, or serve the folder:

```bash
python3 -m http.server 5500
```

Go to http://localhost:5500.

## Add a snippet

Open `js/data.js` and add an item to the `SNIPPETS` array. Give it a unique string `id`, a `category`, `title`, `description`, `code`, and optionally a `note`.

The website itself is plain HTML, CSS, and JavaScript, **not a running Blazor app**. It displays Blazor/Razor code examples. To actually run the `.razor` snippets, create a Blazor app using the .NET SDK. Interactive examples need an interactive render mode.

## Put it on GitHub

Create an empty repository named `blazor-cheatsheet`, then run these commands from this folder:

```bash
git init
git add .
git commit -m "Add Blazor notes site"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/blazor-cheatsheet.git
git push -u origin main
```

To publish: repository **Settings → Pages → Deploy from a branch → main / (root) → Save**. The site will appear at `https://YOUR_USERNAME.github.io/blazor-cheatsheet/` once deployed.

## Reference

Examples follow the concepts described in [Microsoft's Blazor documentation](https://learn.microsoft.com/aspnet/core/blazor/). Some snippets assume you've already configured services, render modes, or models in your own app. The notes on each example call out those assumptions.
