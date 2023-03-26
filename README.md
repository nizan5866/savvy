# savvy
created the runner by https://github.com/actions/actions-runner-controller/blob/master/docs/quickstart.md

#

I had a problem:

  /usr/local/bin/docker buildx create --name builder-3367d142-667f-46da-9e5a-56a8706f3c86 --driver docker-container --buildkitd-flags --allow-insecure-entitlement security.insecure --allow-insecure-entitlement network.host --use
  error: could not create a builder instance with TLS data loaded from environment. Please use `docker context create <context-name>` to create a context for current environment and then create a builder instance with `docker buildx create <context-name>`
  Error: The process '/usr/local/bin/docker' failed with exit code 1

this fixed my problem : https://github.com/mumoshu/actions-runner-controller-ci/commit/e91c8c0f6ca82aa7618010c6d2f417aa46c4a4bf
