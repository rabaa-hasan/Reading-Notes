# HEROKU

Heroku is a cloud platform that lets companies build, deliver, monitor and scale apps — we're the fastest way to go from idea to URL, bypassing all those infrastructure headaches.

![her](https://th.bing.com/th/id/R152914b4af2960f05235e695a2d53852?rik=mbOoeZFLazS7NQ&riu=http%3a%2f%2flogz.io%2fwp-content%2fuploads%2f2016%2f04%2fheroku-logo.png&ehk=CTqIfJ4HVUudzSJC6fIYQso8VazAlAC3p4JUClUN5fA%3d&risl=&pid=ImgRaw)

## focus on apps
Heroku is the quickest way for a company to become an apps company. Heroku is a service that enables companies to spend their time developing and deploying apps that immediately start producing value.

## Trusting Heroku with success
Heroku is a company built on trust and security. Trust is the responsibility of each and every employee, and one we take very seriously.

![h](https://www2.assets.heroku.com/assets/what/what-metrics-e116ce51b227b045bd5334986a46fcbf5b1a7cde92fdd6418d5914e84cd19334.png)

#### 26+ Billion Requests per Day

![h](https://www0.assets.heroku.com/assets/what/what-apps-88aa1cc8c4df1d278ddab8902a9aacc7045c0190aa2c5229fd0c8e2a0c9b53b6.png)

#### 9+ Million Apps Created

![h](https://www2.assets.heroku.com/assets/what/what-addons-60420a98dde646c253b51e4224cc8b762e1a2dbe0d2f253449e1b1001b7f7d47.png)

#### 175+ Add-on Services

![h](https://www3.assets.heroku.com/assets/what/what-data-ccb6658bfd0d7296200868724383bf7ce99def443c4fb248429d2d2ffbf793c3.png)

#### 2+ Million Managed Data Stores

## Heroku and data
![d](https://www0.assets.heroku.com/assets/home/hero/data-a4eeceb4fc7926c678eb97c570037dc83f75a052f523f1c3014b1c0b1d505bf6.png)

Data lies at the heart of any significant app — whether it's customer data or data about the service it provides — an app and its data go hand in hand. Heroku's rich ecosystem of managed data services includes Heroku Postgres, Heroku Redis and Apache Kafka on Heroku.

Developers shouldn't need to discover how to optimally provision a database through trial and error - but instead have immediate access to a scalable, highly available database with rollback - one that supports their apps and development style.

## An ecosystem of services
Using an existing, high-quality service is something that empowers developers - they can build more, faster, by using trusted services that provide the functionality that they require.


## Deploying Heroku with Git
Heroku manages app deployments with Git, the popular version control system. You definitely don’t need to be a Git expert to deploy code to Heroku, but it’s helpful to learn the basics.

## Prerequisites: Install Git and the Heroku CLI
* Git installation instructions

* Heroku CLI installation instructions

## Tracking your app in Git
Before you can deploy your app to Heroku, you need to initialize a local Git repository and commit your application code to it.

```
$ cd myapp
$ git init
Initialized empty Git repository in .git/
$ git add .
$ git commit -m "My first commit"
Created initial commit 5df2d09: My first commit
 44 files changed, 8393 insertions(+), 0 deletions(-)
 create mode 100644 README
 create mode 100644 Procfile
 create mode 100644 app/controllers/source_file
...
```

## Creating a Heroku remote
```
$ heroku create
Creating app... done, ⬢ thawing-inlet-61413
https://thawing-inlet-61413.herokuapp.com/ | https://git.heroku.com/thawing-inlet-61413.git
```

```
$ git remote -v
heroku  https://git.heroku.com/thawing-inlet-61413.git (fetch)
heroku  https://git.heroku.com/thawing-inlet-61413.git (push)
```

### Renaming remotes
`$ git remote rename heroku heroku-staging `

### Deploying code
```
git push heroku master
Initializing repository, done.
updating 'refs/heads/master'
...

```

After you initiate a Heroku deploy with `$ git push`, you can detach from the resulting build process by pressing (Ctrl + C).

 This does not cancel the build or the deploy. The build will continue in the background and will create a new release as soon as it completes.

