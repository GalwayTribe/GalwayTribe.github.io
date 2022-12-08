# Tribe Website

This is the repository from which the Tribe Website is built. It uses [Hugo](https://www.gohugo.io) and is loosely based on the Hugo Hero Theme. The website is published on github pages at https://galwaytribe.github.io/. 

## Contributing 
### Indirectly contributing content
If you are not comfortable contributing directly simply ping Eoghan on Slack and send him the plain text of the content you want to submit along with any images.

### Directly making changes to the site
- [Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) the repository.
- [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) to your local machine.
- Make changes to your fork of the repo and test your changes locally.
- [Create a Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
  - Make sure to add a description of your pull request, especially if any changes have been made to the html or css files.

## Basics

**Deployment**
- The website is deployed from the `docs` directory ⚠️ **DO NOT DIRECTLY EDIT THESE FILES**.

**Content Management**
- The website's content is all editable via markdown files in the `content` directory.
- Associated images should be added to the relevant folder in the `static` directory.

**Menu**
- Responsive menu managed in `config.toml`
- Animated hamburger menu on mobile
- You can edit and add main menu links in the `config.toml` under `[[menu.main]]`

**Layout**
- The layout of the website can be edited by editing the files in the `layouts` directory.

**Style - SCSS**
- The style fo the website is built from the scss files located in the `assets` directory.


## Using Hugo to Work on the Site

**1. Install Hugo**

To work with this website you will first need to have Hugo installed. Please follow the official [installation guide](https://gohugo.io/getting-started/installing/)

⚠️ **Note:** Check your Hugo version - **Hugo Extended** is required!

The underlying theme uses [Hugo Pipes](https://gohugo.io/hugo-pipes/scss-sass/) to compile SCSS and minify assets which means if you not using the Hugo extended version this theme will not work. To check your version of Hugo, run  `hugo version`. Make sure you see `extended` after the version number, for example `hugo v0.106.0-e08ce30fe4779e7d8a8395d7021314b915648cb4+extended windows/amd64 BuildDate=2022-11-17T18:33:40Z VendorInfo=gohugoio` You do not need to use version v0.106.0 specifically, it just needs to have the `extended` part.

**2. Read the Hugo documentation**

If you havent used hugo before it's worth reading the [documentation](https://gohugo.io/documentation/) to understand how everything works, but the next few steps act as a quick start guide. You may be able to get away with just those for basic changes.


**3. Running Hugo**

For local development run Hugo's built-in local server.

```
hugo server
```

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser to see the site as it stands.

**4. Building the Site**

To build the site and publish to the `docs` directory

```
hugo -D
```

**5. Push your Changes to your Fork, create a Pull Request**

Add, commit and push your changes to your fork. 

```
git add -A
git commit -m "<description of my change>"
git push
```

When your changes are ready for review, create a [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork). Ping Eoghan on Slack if you want him to see it quickly.



