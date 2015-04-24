## Introduction
For over a year I've been working as a front-end developer with Magento. Magento is a pretty complex eCommerce platform where the front-end consists of CSS, JavaScript, templates and an XML layer called 'Layout'. All of these exist in packages and themes, which can easily be changed or used as a building blocks for new themes.

Last year with the Magento Enterprise Edition 1.14 release Magento introduced a new theme called RWD, which is, as far as I know, its first official responsive theme. You might say: "better late than never", but there is more: the best thing about RWD is that it's using Sass!

## First version
At my company we wanted to create a default package, something that we could easily demo to our customers and show them all possibilities, modules and customization options. The front-end had to be responsive and easy to customize into the colors and look and feel of the customer. It had to be easy to maintain and maybe even more important: Magento updates should not be a pain in the ass and break it. This might sound logical to you, but the past taught us that these things weren't always written in stone.

For our first version of our own Default theme we copied all the RWD Sass files into our own package and theme folders. This made RWD the base of our own theme, but as we noticed later, Magento updates with changes in the RWD Sass files weren't visible in our own theme, because ours was still based on an earlier version.

### Pros
- Because we copied all Sass files from RWD to our own theme there was no fallback to RWD in place for our Sass files. This means we had the freedom to change the RWD styling to whatever we wanted without any consequences.
- Because there was no Sass fallback we didn't have to undo RWD styling in our own theme by resetting values everywhere.

### Cons
- Magento updates messed with our styling because we used an older version of the Sass files in our own Default theme. We were missing styling for new features and bug fixes that were done by the Magento team.
- Because we wanted our Default theme to be the starting point for customized customer themes this meant we copied all Sass files from Default to Customer and ended up with the same problems during updates as described above. This meant updates would not only have to be implemented into our own Default theme, but also again for each of our customer theme. Creating a lot of extra work that we rather spend on something else.

## Second version
With the above in mind I started to work on a second version of our Default theme. I wanted to use Magento's fallback where possible for the Sass files, so that we easily could benefit from the Magento updates without the need to manually go through the files and copy the changes into our own codebase.

For some reason we never got

## Future
