# Github releases Slack notificcations

## Development(Docker)

### Installation

#### 1. Init

```bash
git clone --recursive git@github.com:luongvietdung/github_releases_slack_notifications.git
cd github_releases_slack_notifications
```

#### 2. Create database

```bash
docker-compose up
docker-compose exec web bundle install
docker-compose exec web bundle exec rails db:setup
```

### Usage

#### Start Docker

```bash
docker-compose up
```

#### Bundle Install

```bash
docker-compose exec web bundle install
```

#### Start Server

```bash
docker-compose exec web bundle exec rails s -b 0.0.0.0
```

### Endpoints

- http://localhost:81

#### Remove Docker

```bash
docker-compose down
docker-compose down --rmi all # If you also want to delete container image
```
