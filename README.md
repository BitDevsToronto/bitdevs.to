# BitDevs Toronto

Source for [bitdevs.to](https://bitdevs.to). Forked from
[BitDevs NYC](https://github.com/BitDevsNYC/BitDevsNYC.github.io).

## Adding a meeting agenda

Copy `_posts/_template.md` to `_posts/YYYY-MM-DD-toronto-socratic-NN.md`, fill it
in, delete the `published: false` line, and push to `main`. The site rebuilds
itself within a minute or two.

If the date is not settled yet, add `date_display: "September 2026"` and a
`permalink:` without a day in it. Both override the date in the filename, which
Jekyll requires but never shows.

Agendas can go up before the meeting and be edited afterwards. Suggestions from
attendees are welcome as pull requests.

## Changing the site itself

Name, description and menu live in `_data/settings.yml` and `_config.yml`, and
some values appear in both. Homepage text is `index.html`, the about page is
`about.md`, styling is `assets/css/`.

## Running it locally

Needs [Ruby and Jekyll](https://jekyllrb.com/docs/installation/).

```
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Hosting

GitHub Pages builds and serves this repo. `CNAME` is what tells it to answer at
bitdevs.to.
