# `site-academic`: The Source Repository for http://lin-jennifer.github.io 

## Building the site

**Automatically**: Run `update.sh`

**By Hand**:

Method 1: Run the `server site` under the blogdown admin menu in R Studio.

Method 2: If that fails, run `build-site.R`

Either way: PUSH `lin-jennifer.github.io` to the master branch

*It is recommended that you try all three methods at least once because we don't know for sure yet which one will work 100% of the time.*

# Manual Breaking changes when updating

- [ ] Check for pages.html update and copy to `layouts/partials/widgets/` and ADD to localization section

```
{{ else if eq $items_type "research" }}
  {{ $i18n = "more_research" }}
```

- [ ] Check `i18n` ENGLISH updates. Copy to `i18n/` and add

```
- id: more_research
  translation: See all ongoing projects
 
- id: more_talks
  translation: See all presentations
```

- [ ] For customize pages, repeat