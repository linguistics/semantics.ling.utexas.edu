# Minerva project website

_Modeling Discourse and Social Dynamics in Authoritarian Regimes_

Hosted at <http://semantics.ling.utexas.edu/>


## Development

Initialization:

    bundle install --path vendor/bundle

Build site:

    bundle exec jekyll build

Deploy to server:

    rsync -rPz _site/ semantics:/www/semantics.ling.utexas.edu

<!-- That might leave a mess on the server, but we don't want to use `rsync --delete`
  since there are some shared data files in that directory on the server. -->
