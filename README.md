# About
See [octopress.fntsr.tw](http://octopress.fntsr.tw) for a live example.

The theme was created for use with [Octopress](http://octopress.org/).

## Installing the Theme
The theme is for the [Octopress](https://github.com/imathis/octopress) blogging
system. To install it either
[download the theme](https://github.com/fntsrlike/TechStory/zipball/master)
and drop the directory into the `./.themes` directory or add this repository as a
submodule:

```Shell
git submodule add git@github.com:fntsrlike/TechStory.git .themes/TechStory
```

You then need to tell Octopress to "use" the new theme.

```Shell
rake install['TechStory']
```

Test it out `rake generate && rake preview`.

## Updating the Theme
### Git Submodule

```Shell
cd .themes/TechStory
git pull
cd ../..
rake update_source['TechStory']
rake update_style['TechStory']
```

Done, test it `rake generate && rake preview`.

### Manually Installed  Directory

1. [Download the theme](https://github.com/fntsrlike/TechStory/zipball/master)
from GitHub.
2. Copy it into your `.themes` directory.
3. Update it

```Shell
rake update_sourc['TechStory']
rake update_style['TechStory']
```

Done, test it `rake generate && rake preview`.

## License
The theme is licensed under the "GPL license", for the exact terms please see the [_LICENSE_ file](https://github.com/fntsrlike/TechStory/blob/master/LICENSE).
