# Sunpech's Blog

[![Netlify Status](https://api.netlify.com/api/v1/badges/f778afc7-e96b-4b11-881b-e455caf05776/deploy-status)](https://app.netlify.com/sites/quirky-nobel-cf5a0a/deploys)

This is the blog for sunpech.com. The blog was orginally on [Blogger](https://www.blogger.com), then converted to [Jekyll](https://jekyllrb.com/), and has now been migrated to [Hugo](https://gohugo.io/).

The theme is called [basic-theme](https://github.com/sunpech/basic-theme), which is based off of [Clean Blog Jekyll](https://github.com/IronSummitMedia/startbootstrap-clean-blog-jekyll).

## Creating a Post

At command prompt within folder of hugo project:

```
hugo new posts/YYYY-MM-DD-title-of-post.md
```

See `archetypes/posts/default.md` for format.

### Variables
* `title` - auto-generated from command line. Remove YYYY MM DD date.
* `headerimage` - can be set for custom header image. Should be 1900px wide. Also dim the photo, maybe 1-3 exposure stops.
* `images` - width should be 600px or wider. Recommended: 1080px. Dimension of 1080x720. It's an array, so multiple images can be added (up to 6).
* `thumbnail` - width should be 300px.
* `description` - should be filled out for better Twitter Cards and Facebook Graph posts (optional)
* `draft` - defaulted to true. Change to false to publish.

### Embedding a YouTube video

You can embed an iframe into a post, but to get it so it's responsive, use the following div and class around the iframe:

```
<div class="video-container">
<iframe... </iframe>
</div>
```

## Images and Photos

Images are responsive by default. Ideal width of image is 1080 pixels.

 ## Creating a Page

At command prompt within folder of hugo project:

 ```
hugo new new-page.md
```

 Create a Page-name.md file at the root of content folder. Or create it at subfolder with _index.md as the list page.

 See `archetypes/default.md` for format.


## Links
* https://github.com/lingxz/er - Atom feed
* [Hugo - Getting Started](https://gohugo.io/getting-started/quick-start/)

## TODO:
* Move all images to be local, instead of hosted on Blogspot.
* Change http to use https where possible.
* Update Taxonomies page, Tags. Include some kind of intro for page.