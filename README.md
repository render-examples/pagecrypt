# PageCrypt Example on Render

This project is a static site that demonstates using [PageCrypt](https://github.com/Greenheart/pagecrypt) to password protect the site.

An example deployment of this repository is at [https://pagecrypt.onrender.com](https://pagecrypt.onrender.com). Use the password `s3cr3t` to view it.

## Deployment

See the [blog post](https://render.com/blog/static-site-auth-pagecrypt) that uses this repository or follow the steps below:

1. [Create a new repository](https://github.com/render-examples/pagecrypt/generate) from this template repository.
2. [Create a new static site](https://dashboard.render.com/select-repo?type=static) on Render from that repository using the following values:
  * **Build Command**: `yarn && yarn run build`
  * **Publish directory**: `dist`
  * **Advanced** ➡️ **Add Environment Variable** ➡️ Create an environment variable named `PASSWORD`. Its value will be used to encrypt your site and used by visitors to decrypt and view the site.

That's it! Your static site will be live on your Render URL as soon as the build finishes.
