
### How it works

Everything about me should be contained within the `me.toml` file.

### How to deploy updates to `me.toml`

When `me.toml` is updated, everything else can be updates as follows:

``` r
# install the 'me' package
devtools::install_github("anthonypileggi/me")
library(me)

# generate an awesome-cv
awesome_cv(color = "emerald")

# generate a hugo-resume website
hugo_resume()
```

Then upload the generated files to the appropriate places in this repo so that they can be deployed by Netlify.
