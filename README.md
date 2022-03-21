# myring
myring is an easy-to-use [webring](https://en.wikipedia.org/wiki/Webring) template built using Jekyll. Use it to generate static webrings, perfect for hosting on services such as Neocities, DigitalOcean, AWS... really, anywhere you can host a static site!

## Requirements
- Jekyll - install using the [quickstart guide](https://jekyllrb.com/docs/)
- Light commandline experience
- Some web hosting experience, and a place to host your webring

## Basic usage
- To create a new webring, copy the template folder from this repository and rename the copy to whatever you want.
- Personalize the ring: edit `config.yml`, change out the images in `img`, and configure the stylesheets by editing the 'override' styles in `style`. You can edit the index and site viewer layout too, but it's not recommended.
- Add sites to the ring: see the example sites in `_sites` to get an idea for the format.
- Run `bundle exec jekyll serve` in the root of your ring's directory. You can then preview how the ring will look and act.
- Once you're ready, run `bundle exec jekyll build` to generate the ring. You can then publish the contents of `_site` (NOT `_sites`).

## Limitations
- Some sites may not work with myring, due to the use of an iframe in the site viewer. This is primarily a problem with modern sites, which disable embedding within iframes. Since webrings are primarily designed for groups of friends hosting smaller sites, this shouldn't be too much of an issue.
- Managing rings is still a bit rough; in the future I'd like to add a management tool to make things a bit easier.
- Might not work/look correctly on some old browsers, like IE6 and earlier.
