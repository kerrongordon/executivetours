---
title: GitLab GraphQL API
date: 2022-07-28T11:22:48.564Z
url: /services/{{.Title}}
cover:
  alt: "{{.Title}}"
  caption: "{{.Title}}"
  image: /images/hero2.jpg
---
Experimental support for GitLab's [GraphQL API](https://docs.gitlab.com/ee/api/graphql/) is now available for the GitLab backend.

**Note: not compatible with Git Gateway.**

GraphQL allows to retrieve data using less individual API requests compared to a REST API. The current implementation uses the GraphQL API in specific cases, where using the REST API can be slow and lead to exceeding GitLab's rate limits. As we receive feedback and extend the feature, we'll migrate more functionality to the GraphQL API.

You can enable the GraphQL API for the GitLab backend by setting `backend.use_graphql` to `true` in your CMS config: