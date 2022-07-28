---
title: Setup and settings
date: 2022-07-28T02:53:51.218Z
url: "{{title.slug}}"
cover:
  alt: "{{title.slug}}"
  caption: "{{title.slug}}"
  image: /images/hero2.jpg
services:
  - title: Setup and settings
  - title: Setup and settings
  - title: Setup and settings
  - title: Setup and settings
---
You can change the settings as follows:

* **Repository:** indicates which repository the Gateway will access (the site’s connected repository). Works with repositories hosted on GitHub.com or GitLab.com only. Self-hosted Git instances aren’t supported. This setting is not directly editable.
* **Roles:** limits Gateway access to Identity users assigned a matching role (in [individual Identity user data](https://docs.netlify.com/visitor-access/identity/manage-existing-users/)). Accepts multiple values. Leaving this field blank will give access to all Identity users on the site.
* **GitHub access token:** grants permission to the linked repository. Use the link to generate a token, or you may supply your own [Personal Access Token](https://github.com/blog/1509-personal-api-tokens). Be sure the token is generated for a user with sufficient permission on your linked repository to perform the actions you want to pass through the Gateway.
* **GitLab access token:** grants permission to the linked repository. You must create a [personal access token in GitLab](https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html) with the necessary scopes for Git Gateway to act on users’ behalf. For example, if you set up Git Gateway to allow users to edit site content without write access to the GitLab repository or even a GitLab account, then your access token needs these scopes: `api`, `read_api`, `read_repository`, and `write_repository`