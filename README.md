Show your **React** App to the world for FREE Using [GitHub Pages](https://pages.github.com/) in 6 Easy Steps.

## 1. Create a Github Repository.
Create a Public GitHub Repository for your **React** App.

>You need to create a GitHub account if you don't have it yet.

![Creating Repo](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xkm4u5fv7h4i1qqqy55h.png)

> Make a note of your **"Owner Name"** and **"Repository Name"** in GitHub.


## 2. Adding homepage key.

Go to `package.json` and make a new **key** named `homepage` and put its value something like the following
`http://<owner-name>.github.io/<app-name>/`

In my case it will be:

package.json

```json
{
  "homepage": "http://youssefzidan.github.io/gh-pages-app/",
  "name": "gh-pages-app",
  "version": "0.1.0"
  //...
}
```

## 3. wrap your **Routes** inside `<HashRouter basename="/">`

If your app has routing wrap your **Routes** inside `<HashRouter basename="/">`

> We need this step to prevent GitHub to redirect your app to 404 in case you refresh teh page.

## 4. Build Your app

Run the build command

```
npm run build
```

You will find a newly created folder named **build**.

![Build Folder](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/hzym3zmjddsa1w0hd4ap.JPG)



## 5. Change the **build** folder name to be **docs**.

Rename the **build** folder to be **docs**

![Docs Folder](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fo4eh6annau8utoqsrfw.JPG)

## 6. Change Repo Settings.

Go to repo settings => Pages section, and change the `/(root)` option to be to `/docs`


Now wait a few minutes and you will see your app published in a URL like this

```terminal
https://youssefzidan.github.io/react-gh-pages/
```

## Thank You.
