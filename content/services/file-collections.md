---
title: File collections
layout: services
image: /images/hero2.jpg
services: []
---
A `files` collection contains one or more uniquely configured files. Unlike items in `folder` collections, which repeat the same configuration over all files in the folder, each item in a `files` collection has an explicitly set path, filename, and configuration. This can be useful for unique files with a custom set of fields, like a settings file or a custom landing page with a unique content structure.

When configuring a `files` collection, configure each file in the collection separately, and list them under the `files` field of the collection. Each file has its own list of `fields` and a unique filepath specified in the `file` field (relative to the base of the repo).

**Note:** Files listed in a file collection must already exist in the hosted repository branch set in your Netlify CMS [backend configuration](https://www.netlifycms.org/docs/backends-overview). Files must also have a valid value for the file type. For example, an empty file works as valid YAML, but a JSON file must have a non-empty value to be valid, such as an empty object.