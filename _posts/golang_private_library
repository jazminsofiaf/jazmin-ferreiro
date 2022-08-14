In order to be able to import private Golang repositories from Github, you must follow these steps:

1. Generate Github access token and export in environment variable on your system:
`GITHUB_TOKEN=ghp_AAAAAAAAAAAAAAAAA…`
When set, will use "https://${GITHUB_TOKEN}:x-oauth-basic@github.com/" to download dependencies from github. Allowing access to private repos.
2. Change access method to Github repositories:
`git config --global [url.git@github.com](mailto:url.git@github.com):.insteadOf [https://github.com/](https://github.com/)`
3. Add private repository to GOPRIVATE environment variable (comma separated list):
`export GOPRIVATE="[github.com/getritmo/](http://github.com/getritmo/country)"`
4. Get dependencies with `go mod tidy` or `go get`.

# Install lib with go install

```jsx
*export GOPATH=$HOME/go*
```

```jsx
*export PATH=$PATH:$GOPATH/bin*
```

```jsx
go install github.com/golangci/golangci-lint/cmd/golangci-lint@v1.42
```
