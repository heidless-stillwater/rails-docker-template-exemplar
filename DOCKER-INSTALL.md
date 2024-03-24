
# INSTALL

```
sudo chmod 666 /var/run/docker.sock

sudo apt install net-tools
ipconfig /flushdns

sudo apt install apt-utils

#########################
```

# SSL Connection Error

### [HTTP parse error, malformed request - Ruby on Rails](https://stackoverflow.com/questions/42750685/http-parse-error-malformed-request-ruby-on-rails)

```
# config/environments/production.rb

# Force all access to the app over SSL, use Strict-Transport-Security, and use secure cookies.

config.force_ssl = true   # change to 'false'

```

# docker

```

RAILS_ENV='development'
echo $RAILS_ENV

docker build -f Dockerfile -t rails-proto-0 .

docker run -p 3000:3000 -v $(pwd):/rails rails-proto-0

docker rm /busy_joliot    # remove container

docker rmi image rails-proto-0:latest

---

gcloud builds submit --tag gcr.io/heidless-pfolio-deploy-5/rails-proto-0 .

---


```



# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...
