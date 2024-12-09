---
layout: post
title: "Design for Dimension"
author: "Ally Smith"
categories: journal
tags: [documentation,sample]
image: forest.jpg
---


We learned how to design for a target user group by re-designing Knotty&Board's website to fit 3 different screen sizes. We created personas to identify our users, drew many sketches, received feedback on our ideas, and made our final prototypes on Figma.


<div class='sk-ww-medium-post' data-embed-id='25497055'></div><script src='https://widgets.sociablekit.com/medium-post/widget.js' defer></script>

## Notable features

* Compatible with GitHub Pages.

* Support for Jekyll's built-in Sass/SCSS preprocessor and data files for making customizing easier.

* [Google Analytics](https://www.google.com/analytics/) support.

* Commenting support powered by [Disqus](https://disqus.com/).

* Optimized for search engines.

* LaTeX support through [MathJax](https://www.mathjax.org/).

## Table of Contents

1. [Introduction](#introduction)
   1. [What is Jekyll](#what-is-jekyll)
   2. [Never Used Jeykll Before?](#never-used-jekyll-before)
2. [Installation](#installation)
   1. [GitHub Pages Installation](#github-pages-installation)
   2. [Local Installation](#local-installation)
   3. [Directory Structure](#directory-structure)
   4. [Starting From Scratch](#starting-from-scratch)
3. [Configuration](#configuration)
   1. [Sample Posts](#sample-posts)
   2. [Site Variables](#site-variables)
   3. [Adding Menu Pages](#adding-menu-pages)
   4. [Posts](#posts)
   5. [Layouts](#layouts)
   6. [YAML Front Block Matter](#yaml-front-block-matter)
4. [Features](#features)
   1. [Design Considerations](#design-considerations)
   2. [Disqus](#disqus)
   3. [Google Analytics](#google-analytics)
   4. [RSS Feeds](#rss-feeds)
   5. [Social Media Icons](#social-media-icons)
   6. [MathJax](#mathjax)
   7. [Syntax Highlighting](#syntax-highlighting)
   8. [Markdown](#markdown)
5. [Everything Else](#everything-else)
6. [Contributing](#Contributing)
7. [Questions?](#questions)
8. [Credits](#credits)
9. [License](#license)

## Introduction

Lagrange is a Jekyll theme that was built to be 100% compatible with [GitHub Pages](https://pages.github.com/). If you are unfamiliar with GitHub Pages, you can check out [their documentation](https://help.github.com/categories/github-pages-basics/) for more information. [Jonathan McGlone's guide](http://jmcglone.com/guides/github-pages/) on creating and hosting a personal site on GitHub is also a good resource.

### What is Jekyll?

Jekyll is a simple, blog-aware, static site generator for personal, project, or organization sites. Basically, Jekyll takes your page content along with template files and produces a complete website. For more information, visit the [official Jekyll site](https://jekyllrb.com/docs/home/) for their documentation. Codecademy also offers a great course on [how to deploy a Jekyll site](https://www.codecademy.com/learn/deploy-a-website) for complete beginners.

### Never Used Jekyll Before?

The beauty of hosting your website on GitHub is that you don't have to actually have Jekyll installed on your computer. Everything can be done through the GitHub code editor, with minimal knowledge of how to use Jekyll or the command line. All you have to do is add your posts to the `_posts` directory and edit the `_config.yml` file to change the site settings. With some rudimentary knowledge of HTML and CSS, you can even modify the site to your liking. This can all be done through the GitHub code editor, which acts like a content management system (CMS).

## Installation

### GitHub Pages Installation

To start using Jekyll right away with GitHub Pages, [fork the Lagrange repository on GitHub](https://github.com/LeNPaul/Lagrange/fork). From there, you can rename your repository to 'USERNAME.github.io', where 'USERNAME' is your GitHub username, and edit the `settings.yml` file in the `_data` folder to your liking. Ensure that you have a branch named `gh-pages`. Your website should be ready immediately at 'http://USERNAME.github.io'. Note: if you are hosting several sites under the same GitHub username, then you will have to use [Project Pages instead of User Pages](https://help.github.com/articles/user-organization-and-project-pages/) - just change the repository name to something other than 'http://USERNAME.github.io'.

Head over to the `_posts` directory to view all the posts that are currently on the website, and to see examples of what post files generally look like. You can simply just duplicate the template post and start adding your own content.

### Local Installation

For a full local installation of Lagrange, [download your own copy of Lagrange](https://github.com/LeNPaul/Lagrange/archive/gh-pages.zip) and unzip it into it's own directory. From there, open up your favorite command line tool, enter `bundle install`, and then enter `jekyll serve`. Your site should be up and running locally at [http://localhost:4000](http://localhost:4000).

### Directory Structure

If you are familiar with Jekyll, then the Lagrange directory structure shouldn't be too difficult to navigate. The following some highlights of the differences you might notice between the default directory structure. More information on what these folders and files do can be found in the [Jekyll documentation site](https://jekyllrb.com/docs/structure/).

```bash
Lagrange/
├── _data                      # Data files
|  └── settings.yml            # Theme settings and custom text
├── _includes                  # Theme includes
├── _layouts                   # Theme layouts (see below for details)
├── _posts                     # Where all your posts will go
├── assets                     # Style sheets and images are found here
|  ├── css                     # Style sheets go here
|  |  └── main.css             # Main CSS file
|  |  └── syntax.css           # Style sheet for code syntax highlighting
|  └── img                     # Images go here
├── menu                       # Menu pages
├── _config.yml                # Site build settings
├── Gemfile                    # Ruby Gemfile for managing Jekyll plugins
├── index.md                   # Home page
├── LICENSE.md                 # License for this theme
├── README.md                  # Includes all of the documentation for this theme
└── rss-feed.xml               # Generates RSS 2.0 file which Jekyll points to
```

### Starting From Scratch

To completely start from scratch, simply delete all the files in the `_posts`, `assets/img`, and `menu` folder, and add your own content. You may also replace the `README.md` file with your own README. Everything in the `_data` folder and `_config.yml` file can be edited to suit your needs. You may also change the `favicon.ico` file to your own favicon.

## Configuration

### Sample Posts

Visit the [the demo site](https://lenpaul.github.io/Lagrange/) to find sample posts that show what different types of text formatting look like. You can find these posts in the `_posts` folder, which show what the best practices for setting up your own site are.

### Site Variables

To change site build settings, edit the `_config.yml` file found in the root of your repository, which you can tweak however you like. More information on configuration settings and plugins can be found on [the Jekyll documentation site](https://jekyllrb.com/docs/configuration/). This is also where you will be able to customize the title, description, and the author/owner of your site.

If you are hosting your site on GitHub Pages, then committing a change to the `_config.yml` file will force a rebuild of your site with Jekyll. Any changes made should be viewable soon after. If you are hosting your site locally, then you must run `jekyll serve` again for the changes to take place.

In the `settings.yml` file found in the `_data` folder, you will be able to customize your site settings, such as setting Disqus comments, Google Analytics, what shows up in your menu, and social media information.

### Adding Menu Pages

The menu pages are found in the `menu` folder in the root directory, and can be added to your menu in the `settings.yml` file.

### Posts

You will find example posts in your `_posts` directory. Go ahead and edit any post and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention of `YYYY-MM-DD-name-of-post.md` and includes the necessary front matter. Take a look at any sample post to get an idea about how it works. If you already have a website built with Jekyll, simply copy over your posts to migrate to Lagrange.

### Layouts

There are two main layout options that are included with Lagrange: post and page. Layouts are specified through the [YAML front block matter](https://jekyllrb.com/docs/frontmatter/). Any file that contains a YAML front block matter will be processed by Jekyll. For example:

```
---
layout: post
title: "Example Post"
---
```

Examples of what posts looks like can be found in the `_posts` directory, which includes this post you are reading right now. Posts are the basic blog post layout, which includes a header image, post content, author name, date published, social media sharing links, and related posts.

Pages are essentially the post layout without any of the extra features of the posts layout. An example of what pages look like can be found at the [About](https://lenpaul.github.io/Lagrange/menu/about.html) and [Contacts](https://lenpaul.github.io/Lagrange/menu/contact.html).

In addition to the two main layout options above, there are also custom layouts that have been created for the [home page](https://lenpaul.github.io/Lagrange/) and the [archives page](https://lenpaul.github.io/Lagrange/menu/writing.html). These are simply just page layouts with some [Liquid template code](https://shopify.github.io/liquid/). Check out the `index.html` file in the root directory for what the code looks like.

### YAML Front Block Matter

The recommended YAML front block is:

```
---
layout:
title:
author:
categories:
tags: []
image:
---
```

`layout` specifies which layout to use, `title` is the page or post title, `categories` can be used to better organize your posts, `tags` are used when generating related posts based on the topic of the post, and `image` specifies which images to use. Have a look at some posts in the `_posts` directory to see how these variables are set.

## Features

### Design Considerations

Lagrange was designed to be a minimalist theme in order for the focus to remain on your content. For example, links are signified mainly through an underline text-decoration, in order to maximize the perceived affordance of clickability (I originally just wanted to make the links a darker shade of grey).

### Disqus

Lagrange supports comments at the end of posts through [Disqus](https://disqus.com/). In order to activate Disqus commenting, set `disqus.comments` to true in the `_data/settings.yml` file. If you do not have a Disqus account already, you will have to set one up, and create a profile for your website. You will be given a `disqus_shortname` that will be used to generate the appropriate comments sections for your site. More information on [how to set up Disqus](http://www.perfectlyrandom.org/2014/06/29/adding-disqus-to-your-jekyll-powered-github-pages/).

### Google Analytics

It is possible to track your site statistics through [Google Analytics](https://www.google.com/analytics/). Similar to Disqus, you will have to create an account for Google Analytics, and enter the correct Google ID for your site under `google-ID` in the `settings.yml` file. More information on [how to set up Google Analytics](https://michaelsoolee.com/google-analytics-jekyll/).

### RSS Feeds

Atom is supported by default through [jekyll-feed](https://github.com/jekyll/jekyll-feed). With jekyll-feed, you can set configuration variables such as 'title', 'description', and 'author', in the `_config.yml` file.

RSS 2.0 is also supported through [RSS auto-discovery](http://www.rssboard.org/rss-autodiscovery). The `rss-feed.xml` file (based on the template found at [jekyll-rss-feeds](https://github.com/snaptortoise/jekyll-rss-feeds)) that the feed path points to when using RSS 2.0 is automatically generated based on the appropriate configuration variables found in `_data/settings.yml`.

To use RSS 2.0, ensure the following is done:

* Uncomment the last two lines in the `_config.yml` file.

* In `_data/settings.yml`, under 'social', comment out the rss-square that points to `feed.xml`, and uncomment the rss-square that points to `rss-feed.xml`.

* In `_includes/head.html`, comment out `{% feed_meta %}` and uncomment the line under the RSS 2.0 comment.

### Social Media Icons

All social media icons are courtesy of [Font Awesome](http://fontawesome.io/). You can change which icons appear, as well as the account that they link to, in the `settings.yml` file in the `_data` folder.

### MathJax

Lagrange comes out of the box with [MathJax](https://www.mathjax.org/), which allows you to display mathematical equations in your posts through the use of [LaTeX](http://www.andy-roberts.net/writing/latex/mathematics_1).

### Syntax Highlighting

Lagrange provides syntax highlighting through [fenced code blocks](https://help.github.com/articles/creating-and-highlighting-code-blocks/). Syntax highlighting allows you to display source code in different colors and fonts depending on what programming language is being displayed. You can find the full list of supported programming languages [here](https://github.com/jneen/rouge/wiki/List-of-supported-languages-and-lexers). Another option is to embed your code through [Gist](https://en.support.wordpress.com/gist/).

### Markdown

As always, Jekyll offers support for GitHub Flavored Markdown, which allows you to format your posts using the [Markdown syntax](https://guides.github.com/features/mastering-markdown/). Examples of these text formatting features can be seen below. You can find this post in the `_posts` directory as well as the `README.md` file.

## Everything Else

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll's GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/

## Contributing

If you would like to make a feature request, or report a bug or typo in the documentation, then please [submit a GitHub issue](https://github.com/LeNPaul/Lagrange/issues/new). If you would like to make a contribution, then feel free to [submit a pull request](https://help.github.com/articles/about-pull-requests/) - as a bonus, I will credit all contributors below! If this is your first pull request, it may be helpful to read up on the [GitHub Flow](https://guides.github.com/introduction/flow/) first.

Lagrange has been designed as a base for users to customize and fit to their own unique needs. Please keep this in mind when requesting features and/or submitting pull requests. Some examples of changes that I would love to see are things that would make the site easier to use, or better ways of doing things. Please avoid changes that do not benefit the majority of users.

## Questions?

This theme is completely free and open source software. You may use it however you want, as it is distributed under the [MIT License](http://choosealicense.com/licenses/mit/). If you are having any problems, any questions or suggestions, feel free to [tweet at me](https://twitter.com/intent/tweet?text=My%question%about%Lagrange%is:%&amp;via=paululele), or [file a GitHub issue](https://github.com/lenpaul/lagrange/issues/new).

## Credits

### Creator

#### Paul Le

* [www.lenpaul.com](http://lenpaul.com)

* [Twitter](https://twitter.com/paululele)

* [GitHub](https://github.com/LeNPaul)

### Contributors

* [nikolalukovic](https://github.com/nikolalukovic)

* [gmemstr](https://github.com/gmemstr)

* [lynn9388](https://github.com/lynn9388)

* [robqiao](https://github.com/robqiao)

* [Mauladen](https://github.com/Mauladen)

* [dhanus](https://github.com/dhanus)

* [mlewand](https://github.com/mlewand)

* [Hguimaraes](https://github.com/Hguimaraes)

* [ilhamadun](https://github.com/ilhamadun)

* [brianclemens](https://github.com/brianclemens)

* [leyhline](https://github.com/leyhline)

* [aritra24](https://github.com/aritra24)

* [DuckSoft](https://github.com/DuckSoft)

* [larrylawl](https://github.com/larrylawl)

* [borting](https://github.com/borting)

### Icons + Demo Images

* [Death to Stock](https://deathtothestockphoto.com/)

* [Font Awesome](http://fontawesome.io/)

### Other

* [Jekyll](https://jekyllrb.com/)

* [Free Code Camp](https://www.freecodecamp.org)

* [Khan Academy](https://www.khanacademy.org/)

## License

Open sourced under the [MIT license](https://github.com/LeNPaul/Lagrange/blob/gh-pages/LICENSE.md).


For this Design Sprint, Alp, Devon, and I redesigned the website for Knotty & Board, a local furniture store, focusing on the needs of a specific user group. The website redesign targeted improving both the landing page and a secondary furniture page, ensuring the design could serve users of different ages and technological abilities. The goal was to create a user-friendly interface that is intuitive, visually cohesive, and budget-conscious, offering a smooth shopping experience across multiple devices: desktop, smartwatch, and large multitouch displays.


User Group
The first step of design is identifying the user group and their needs. Therefore, each of us crafted a persona that could be a target user for our website.

Debby (51 years old): A teacher from Cornelius, Debby wants to modernize her mismatched furniture with cohesive pieces. She prefers high-quality but affordable furniture. While she’s good with technology like laptops and large displays, she struggles with visualizing how furniture pieces would look together.
Catherine (22 years old): A recent graduate with a low budget, Catherine shares a living space with three roommates. She’s proficient with technology and wants to ensure the furniture fits her small space. She also cares about her roommates’ opinions and seeks a cozy, homey feel. Her main frustration is determining the right size of furniture for her space.
Rose (74 years old): A retired accountant living alone in Huntersville, Rose has an existing collection of antique furniture. She wants new pieces that match her current collection. However, she struggles with technology and has difficulty seeing small images on screens. Affordability, knowing the origin of furniture, and continuing her collection are her key concerns.
Despite their different needs, all personas shared common goals: budget-friendly furniture, cohesive design, and the ability to see how furniture fits into their home. We tailored our design to ensure each of these aspects was addressed for all personas.

Needs & Features
We identified the unique needs of our personas and developed a unified approach to meet their goals while ensuring that the design catered to their diverse technological abilities, preferences, and challenges.

1. Visualizing Furniture Together
All three personas shared a common frustration: not being able to easily visualize how furniture pieces would look together in their spaces. To address this, we introduced a “Room Preview” tool across all devices:

Debby, who wants a cohesive, modern look, can upload an image of her room and virtually place selected furniture pieces within it. The website’s AI suggests additional matching pieces based on her style preferences.
Catherine can also use this tool to visualize furniture in her small shared space. Rather than guessing the sizing she needs or measuring herself, the website will automatically input the furniture into the image of the room proportionally to how it would be in real life.
Rose can use the same feature to see how new furniture items will match her existing antique collection. Because she is not as good with technology, the larger display would allow her to see and compare pieces better.
2. Customizing the Search Experience
Each persona has specific requirements when browsing for furniture, and our design ensures a tailored search experience:

Debby values high-quality, budget-friendly pieces that work well together. The search feature allows her to filter by style, quality, and price, while also suggesting decor that matches her existing selections.
Catherine, on a tight budget, needs to find affordable, space-saving furniture. She can filter by price, size, and style to ensure that she only sees items that fit both her budget and her small space. The system also suggests homey, cozy furniture styles, catering to her desire to create a warm environment.
Rose looks for vintage pieces at a low price point. Her search filters include price, material, and furniture origin, and the system highlights items that match the classic, antique aesthetic she prefers. Because Rose cares about the details of the items, there is a “Read More” link to see more information about a specific piece.
3. Simplified Navigation
Considering the wide range of technological literacy, our design focuses on clear, simple navigation and visual accessibility:

Debby, comfortable with technology, can navigate the website via a clean, intuitive layout with large images and drop-down menus.
Catherine, being tech-savvy, can quickly access filters and adjust them for price, style, and size across different pages, with features like “Room Preview” to visualize how the furniture fits in her space.
Rose, who is less experienced with technology, benefits from simplified search functions, making it easier for her to navigate and find pieces that fit her existing collection.
4. Budget Management
Since all three personas have budget constraints, we implemented a price range filter that allows users to input their budget and view only the furniture within that range.

Debby can balance quality and affordability, Catherine can stick to a tight budget as she shops for her shared space, and Rose can find reasonably priced vintage or antique-style furniture.
By integrating these features seamlessly into each version of the Knotty & Board website, we ensure that the unique needs of Debby, Catherine, and Rose are met, providing an efficient, personalized, and enjoyable shopping experience.

Design & Sketches
We designed the Knotty & Board website for three types of devices: desktops, smartwatches, and large multitouch displays.

Desktop Design
Landing Page:

Large, clear images indicate the difference between the Furniture Market and Interiors Market and display their Design Services. Images of best-selling pieces help users get a feel for the kind of pieces Knotty & Board has.
A top navigation bar, featuring drop-down menus for furniture and decor categories helps users easily navigate to other pages and access information such as store locations, hours of operation, and their accounts.
A search bar is prominently placed at the top to allow quick access to specific furniture or decor items.
Furniture Page:

The top navigation bar with drop-down menus continues onto the furniture page, allowing easy access to specific categories, the search bar, or other pages.
Users can insert specific price and size ranges as well as select a certain style of furniture they want.
Pieces are displayed with an image, name, size, price, and a “Read More” link. Users can click on this link for a description of the piece and where it came from.
The “Room Preview” tool allows users to upload an image of the room, select pieces of furniture, and see how the items match each other, fit in the room, or match the room. The website will add items proportionally to ensure the sizing is easy to determine.

Large Multitouch Display Design
Landing Page:

This design is very similar to the desktop design. With such a large display, overloading the home page may overwhelm the user. Therefore, images of the two locations, popular items, and information about the Design Service ensure users can find what they are looking for.
The top navigation bar with drop-down menus continues in this display
Furniture Page:

Similar to the desktop display, customizable searches can be done with drop-down menu selections and inputting price and size ranges. Based on the information, furniture pieces will be displayed.
The “Room Preview” tool is more interactive on the large display. A camera on the top of the large multitouch display can display the room in real-time. Users can drag items into the room and the website will place them proportionally. Users can more easily drag the furniture into different places in the room and see how it looks.
Using information from the customizable search, selected items, and how the room looks, the website suggests other furniture and decor items.


Watch Design
Landing Page:

Displaying information on such a small screen can get cramped, so many of the sketches use icons to display a link that will take the user to their desired page.
Furniture Page:

To ensure some customization of the search, users select which kind of furniture they are looking for, and popular pieces will come up. As users scroll through, they can add items to their cart.
Using their phone, users could hold up their camera to the room they need furniture for. Then, they can send the selected furniture from their watch to show up on their phone screen. So, they can see how the furniture looks in the room.

Testing
We tested our design with Alice, James, and Jeremy. They gave us many good suggestions and asked questions that helped us refine our sketches closer to the final prototype. The following are the highlights of their feedback:

Desktop
Landing Page: The top bar is liked, but some designs felt crowded. Breaking up sections with location images worked well. A horizontal layout was confusing for some users.
Furniture Page: The drop-down menus are useful, but showing too many furniture types at once made the page feel cluttered.
Large Multitouch Display
Landing Page: A simple design worked best. They liked the layout that used location images to separate content.
Furniture Page: Drop-downs helped prevent clutter, and having more options displayed at once was useful. However, whether furniture pieces “match” can be subjective.
Watch
Landing Page: The Apple Watch-style layout was favored for its organized information. Some screens felt either too plain or unsuitable for a watch display.
Furniture Page: Having back/home buttons for easy navigation was preferred. Customizable search options fit the personas’ specific needs.
Based on this feedback, we focused on simplicity, reducing clutter, and improving navigation.

Final Sketches
Using the feedback and focusing on our target user group, we combined aspects of our different sketches to create a better end product.

Desktop
Landing Page: Rather than having the furniture and decor items displayed next to each other, we broke them up with images of the Furniture Market and Interiors Market. This provides some division and variety to the page. We made the top bar large and spread out because it is easier to read and use.
Furniture Page: We focused on finding the balance of a customizable search because too many options can burden the user and crowd the screen. Therefore, users can only select one kind and one style of furniture to see.

Large Multitouch Display
Landing Page: We used the same philosophy we used in the computer landing page design. Therefore, we displayed all the information in a format that readers can easily glance at and find what they need.
Furniture Page: Some of our sketches had the feature of using AI to tell users if the furniture they selected matched, however, this is very subjective. So, we prioritized giving suggestions for other furniture or decor that relate to the selected ones.

Watch
Landing Page: The watch interface is inspired by the Apple Watch’s home screen, featuring “bubbles” that link to different pages, such as the furniture page, decor page, Furniture Market location information, etc. Users can scroll around to reveal different “bubbles.” This design allows for a lot of links to be displayed, but not too crowded or small.
Furniture Page: The first page users see has three links: Furniture Type, Price Range, and Size Range. Clicking on them goes to another page where the user can customize their search more. Based on the user input, suggested pieces come up. Clicking the Knotty & Board logo returns to the landing page and clicking the chair icon returns to the first furniture page.

Visual Design
We developed a mood board to capture the aesthetic direction of our redesign. The goal was to create a modern, stylish look without overwhelming users with too much visual noise. After analyzing competitor sites frequently visited by our target demographic, we chose:

Color Palette: Neutral tones like sage green, terracotta, and natural browns create a rustic, warm feel without distracting from the furniture.
Font: We opted for Times New Roman to give the site a more elegant feel while maintaining readability.
Visual Simplicity: Given the personas’ focus on the furniture itself, we kept backgrounds clean and simple to avoid overwhelming users with design elements.

Prototypes
We created prototypes for desktops, smartwatches, and large multitouch display interfaces using Figma. These prototypes were created with a combination of our target users’ needs, many sketches, and feedback from our classmates. Here is the link to our Figma page and images below.

Desktop
Landing Page

Furniture Page

Large Multitouch Display
Landing Page

Furniture Page

Watch
Landing Page

Furniture Page

Conclusion
Our Knotty & Board website redesign successfully incorporates the needs of users across different ages, technological abilities, and goals. By focusing on simplicity, personalization, and interactivity, we created a shopping experience that works across desktops, smartwatches, and large multitouch display interfaces. Through iterative design, testing, and feedback, we refined the experience to provide a cohesive and budget-friendly solution for furniture shoppers. If we were to continue developing this design, we could test our prototypes with more users of diverse backgrounds. We received feedback from three senior computer science majors. Therefore, we could expand our testing to people of different ages and technological backgrounds to create even better interfaces.
