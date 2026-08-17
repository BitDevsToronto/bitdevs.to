# BitDevs Toronto

Source for [bitdevs.to](https://bitdevs.to).

Forked from the [BitDevs NYC](https://github.com/BitDevsNYC/BitDevsNYC.github.io)
site, which most BitDevs chapters use.

## Adding a meeting agenda

1. Copy `_posts/_template.md` to `_posts/YYYY-MM-DD-socratic-seminar-NN.md`,
   using the date of the meeting.
2. Fill in the title, the venue, the times, and the signup link.
3. Add the discussion items, mostly from the
   [Bitcoin Optech](https://bitcoinops.org/en/newsletters/) newsletters since the
   last meeting.
4. Delete the `published: false` line so it appears on the site.
5. Commit and push to `main`. The site rebuilds itself within a minute or two.

Agendas can be published before the meeting and edited afterwards. Suggestions
from attendees are welcome as pull requests.

## Changing the site itself

- Site name, description, and menu: `_data/settings.yml` and `_config.yml`.
  Some values appear in both, so change both.
- Homepage text and the next-meeting notice: `index.html`.
- About page: `about.md`.
- Styling: `assets/css/`.

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
