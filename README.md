# Github User Search
Search and view users via the Github API - http://ec2-13-54-222-34.ap-southeast-2.compute.amazonaws.com:3001/github-user-search/

Requests are cached in session storage to limit the use of the API.

## What is this?

A personal project built with React, Redux and other tools to search users and
view their profiles on Github. 


## Running on AWS

1. Create an instance on EC2
1. install nodejs, npm, yarn
1. Clone the repository with git command
1. Install dependences `yarn`
1. Run the server `yarnpkg run start`
1. Visit `http://localhost:3001/github-user-search/` (note the trailing slash)

## Running locally

1. Clone the repository
1. Open dev.config.js and Remove line 12host : '0.0.0.0',)
1. Install dependences `yarn`
1. Run the server `yarnpkg run start`
1. Visit `http://[aws public DNS that you create]:3001/github-user-search/` (note the trailing slash)



### API limit

When running the app, you can export a [personal
access token](https://github.com/blog/1509-personal-api-tokens) and this will be
sent along in any API calls to increase the limit:

```
export USER_SEARCH_OAUTH=<your token>
yarnpkg run start
```
