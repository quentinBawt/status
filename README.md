# Valyte Data Status

Uptime monitor and status page for Valyte Data services, powered by [Upptime](https://github.com/upptime/upptime).

## Monitored Services

| Service | URL |
|---------|-----|
| NAVster App | https://console.valytedata.com |
| Backend API | AWS API Gateway |
| Supabase Auth | Auth endpoint |
| Netlify Staging | https://main--navster.netlify.app |

## How It Works

- GitHub Actions checks all endpoints every 5 minutes
- If a service goes down, a GitHub Issue is automatically created
- When the service recovers, the issue is automatically closed
- Response time and uptime history are tracked in the `history/` directory
- A static status page is deployed to GitHub Pages

## Incident Management

- **Automatic incidents**: Upptime detects outages and creates issues
- **Manual incidents**: Create an issue with the `incident` label
- **Scheduled maintenance**: Use the maintenance event issue template

## Status Page

The status page will be available at: https://quentinbawt.github.io/status

## Configuration

All monitoring configuration is in `.upptimerc.yml`. See [Upptime docs](https://upptime.js.org/docs/configuration) for details.
