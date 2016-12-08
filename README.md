# Jekyll Starter Kit

This is a starter kit built for someone who wants a Rails-like feel while using Jekyll. I love the Ruby programming language and using the Rails framework which is why I built this starter kit, to give me a more familiar and structured feel when I use Jekyll.

Unfortunately, because GitHub Pages does not support jekyll-assets (see [issue #189](https://github.com/github/pages-gem/issues/189)), this starter kit is for [GitLab Pages](https://pages.gitlab.io) (which is free also) or a self-hosted solution such as [Digital Ocean](https://m.do.co/c/9f7ca951912e).

## So...what's included?

I tried to provide general tools that help you develop quicker, manage your project easier, and be compatible with older browsers. I tried not to make too many assumptions about what will be built since this should be a starting point.

 - [jekyll-haml](https://github.com/samvincent/jekyll-haml) - A templating engine for HTML.
 - [sass](https://github.com/sass/sass) - Sass makes CSS fun again.
 - [coffee-script](https://github.com/rails/ruby-coffee-script) - A little language that compiles into JavaScript.
 - [normalize.css](https://necolas.github.io/normalize.css/) - Makes browsers render all elements more consistently and in line with modern standards.
 - [bourbon](https://github.com/thoughtbot/bourbon) - A Lightweight Sass Tool Set.
 - [neat](https://github.com/thoughtbot/neat) - A lightweight, semantic grid framework built with Bourbon.
 - [bitters](https://github.com/thoughtbot/bitters) - Add a dash of pre-defined style to your Bourbon.
 - [modernizr](https://github.com/Modernizr/Modernizr) - JavaScript library that detects HTML5 and CSS3 features in the user’s browser.
 - [font-awesome-sass](https://github.com/FortAwesome/font-awesome-sass) - Scalable vector icons that can instantly be customized.
 - [uglifier](https://github.com/lautis/uglifier) - JavaScript compressor.
 - [octopress-autoprefixer](https://github.com/octopress/autoprefixer) - Automatically adds CSS vendor prefixes for all CSS and Sass files.
 - [turbolinks](https://github.com/turbolinks/turbolinks) - Makes navigating your web application faster.
 - [jekyll-assets](https://github.com/jekyll/jekyll-assets) - Asset pipelines for Jekyll.
 - [therubyracer](https://github.com/cowboyd/therubyracer) - Embed V8 Javascript Interpreter into Ruby. Required to make jekyll-assets work.
 - [jekyll-feed](https://github.com/jekyll/jekyll-feed) - Generates an Atom (RSS-like) feed of your posts.
 - [google analytics](https://analytics.google.com/analytics/web/) - Provide statistics for who visits your site. Just place your site ID code into the config file to activate it.

## Installing & Deploying with GitLab Pages

1. Clone repo down locally
  ```
  $ git clone https://github.com/eugenetriguba/jekyll-starter-kit.git my-awesome-site
  ```

2. Change directory into repo
  ```
  $ cd my-awesome-site
  ```

3. Remove previous git history
  ```
  $ rm -rf .git
  ```

4. Initialize new git file
  ```
  $ git init
  ```

5. Add all files in directory to staging area
  ```
  $ git add .
  ```

6. Commit files
  ```
  $ git commit -m "Initial Commit"
  ```

7. Create a new GitLab repo with a name of username.gitlab.io (where username is your GitLab username)

8. Add that repo as a remote to your project
  ```
  $ git remote add origin https://gitlab.com/username/username.gitlab.io.git
  ```

9. Push up your commit
  ```
  $ git push -u origin master
  ```

That's it. GitLab will start building your site and it will be live at username.gitlab.io.

If you didn't name your repo 'username.gitlab.io', you will need to add a domain for GitLab to build your repo.

## Connecting a domain to GitLab

To point your domain at GitLab, go to your domain registrar.
You will need two records for this to work.

1. An A record with @ as the host and 104.208.235.32 as the IP.

2. A CNAME record with www as the host (if you're connecting the root domain, 'blog' or whatever else, if you wish to use a subdomain. e.g. blog.example.com) and username.gitlab.io as the IP (even if your repo isn't called username.gitlab.io).

Now go back to GitLab and to your repo → settings (gear icon on the right side) → pages → new domain, type in your domain in the first field, click save.


## Looking to contribute?

It would be best to submit an issue, or contact me at [eugenetriguba@gmail.com](mailto:eugenetriguba@gmail.com), detailing what you were looking to add, change, or fix. If you just have some suggestions on things that could be improved or bugs that need fixing, I'd love to hear it also!
