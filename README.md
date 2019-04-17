# leitmotiv [laɪtməʊtiːf]

Quickstart setup for bootstrapping nodejs applications with some sane start decisions and setups.

## Usage

IMPORTANT:

please have a proper look to the provided scripts in the usage section.
Please use the commands only if properly understood and adjusted for
your environment.
The commands were tested using Apple MacOS, but they might fail or produce harm
on other machines. Different OS' might differ in arguments and usage.

```
git clone git@github.com:codument/leitmotiv.git ./desired-package-name
cd desired-package-name

# replace   occurrences of leitmotiv to your desired package name
find . -type f -exec sed 's/leitmotiv/desired-package-name/g' {} \;

# rename binary to your desired package name. If you want something different
# as resulting bin name, you should update the package.json accordingly.
mv bin/leitmotiv.js bin/desired-package-name.js

# check your changes
git diff

# remove git setup from this repo, once you are ready to start
rm -rf .git

# start fresh git history
git init
```
