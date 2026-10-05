# Personal site: blog and projects

## Publish on GitHub Pages

1. On GitHub, create a public repository named `RavindraKP.github.io`.
2. Upload every file and folder from this directory to the repository (drag and drop on the web page works).
3. Open `_config.yml` and replace `RavindraKP` with your GitHub username. Add your LinkedIn URL and email if you want them in the footer.
4. In the repository, go to Settings > Pages. Under Build and deployment choose "Deploy from a branch", select the `main` branch and the `/ (root)` folder, then save.
5. After one to two minutes the site is live at https://RavindraKP.github.io

## Write a blog post

Add a file in `_posts/` named `YYYY-MM-DD-short-title.md`:

    ---
    title: "Your title"
    summary: One-sentence description.
    tags: [topic]
    ---
    Your text in Markdown.

Posts dated in the future will not appear until that date.

## Update a project

Edit the file in `_projects/`. Change `status` to In progress or Complete and paste the repository link into `github`.

## Add a new project

Copy any file in `_projects/`, rename it, and change the `order`, `title`, `sector`, `summary` and other fields.

## Maths and code

- Inline maths: `\( x^2 \)`. Display maths: `$$ ... $$`.
- Code blocks: three backticks followed by the language name.

## Preview on your own computer (optional)

Install Ruby, then run `bundle install` and `bundle exec jekyll serve`, and open http://localhost:4000.
