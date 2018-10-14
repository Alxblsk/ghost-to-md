---
title: ${post.title}<% if (post.slug) { %>
slug: ${post.slug}<% } %>
date: ${post.publishedAt}
date_updated: ${post.updatedAt}<% if (post.tags.length) { %>
tags: ${post.tags.join(', ')}<% } %><% if (post.status === 'draft') { %>
draft: true<% } %><% if (post.feature_image) { %>
image: ${post.feature_image}<% } %>
---
${markdown}
