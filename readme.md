
### How it works

Everything about me should be contained within the `me.toml` file.
*Currently, this info is being stores within the `me` R package.*

### How to deploy updates to `me.toml`

When `me.toml` is updated, everything else can be updates as follows:

``` r
# install the 'me' package
devtools::install_github("anthonypileggi/me")
library(me)

# generate my awesome-cv
awesome_cv("cv", color = "emerald")

# generate my hugo-resume website
hugo_resume("site", base_url = "https://www.sqwerl.life/")

# compile pdf

# make awesome-cv available on website
file.copy("cv/resume_cv.pdf", "site/static/cv.pdf")
```

Now everything should be set for deploying on Netlify.
