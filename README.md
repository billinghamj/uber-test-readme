# Uber Coding Test

Due to its modular nature, my code is split across a number of repositories:

- [`resilient-mailer`](//github.com/billinghamj/resilient-mailer) - a NPM package providing fault-tolerant email services
- [`mailer-service`](//github.com/billinghamj/mailer-service) - an Express app exposing `resilient-mailer` as a RESTful API
- [`mailer-app`](//github.com/billinghamj/mailer-app) - a tiny Bootstrap front-end allowing submission of emails

API docs are available for the `mailer-service` here:

- [billinghamj.github.io/mailer-service](//billinghamj.github.io/mailer-service/)

The Express apps are running on Heroku:

- `mailer-service` - [jb-mailer-service.herokuapp.com](//jb-mailer-service.herokuapp.com)
- `mailer-app` - [jb-mailer-app.herokuapp.com](//jb-mailer-app.herokuapp.com)

I strongly recommend using email addresses ending with `@jamesbillingham.com`
as the 'from' address during testing, as this domain has SPF & DKIM set up.

## Project

I chose the Email Service project, working on the back-end track.

## Choices

I have used Node JS - along with some lightweight frameworks - for the entirety
of this project. My main reasoning for this is because I have not used it to any
great degree before, and it shows well my ability to be able to effectively &
efficiently use languages within a few days of starting with them. I do this
primarily through learning by example - searching GitHub, etc.

The approach I took to this project was a bit over-engineered, given the spec -
with code spanning across 7 repositories. I decided to do this on the basis that
it demonstrates clearly how I approach & think about problems - when
architecting systems - modularity, flexibility, testing & reuse are all key.

## Trade-offs

Presently, the system I've created is very basic: it sends emails, and that's
it. Given more time, I would create a better queuing system, ways to notify
failures later in time (e.g. after failed delivery), statistics, etc.

I have detailed a number of
[improvements](//github.com/billinghamj/resilient-mailer#future-improvements)
which I would make to the `resilient-mailer` library.

## Resources

Resume: [jamesbillingham.com/resume](http://www.jamesbillingham.com/resume)

Unfortunately, very little of my code is open source - most of the OSS
contributions I make are to existing projects, rather than my own. As such, I am
not able to link to other code samples.