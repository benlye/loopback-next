---
lang: en
title: 'Migrating OAuth2 provider'
keywords: LoopBack 4.0, LoopBack 4, LoopBack 3, Migration
sidebar: lb4_sidebar
permalink: /doc/en/lb4/migration-auth-oauth2.html
---

[`loopback-component-oauth2`](https://github.com/strongloop/loopback-component-oauth2)
is used to setup a LoopBack application as an [OAuth 2.0](https://oauth.net/2/)
server. It can be applied when people implement their LoopBack application as an
OAuth 2.0 provider. For example, the API gateway application.

At this stage, authentication and authorization in LoopBack 4 focus on the
communication to third-party servers like
[google](https://developers.google.com/identity/protocols/oauth2) or
[facebook](https://developers.facebook.com/docs/facebook-login/), instead of
turning itself into an OAuth 2.0 provider. And given the complexity of
[`loopback-component-oauth2`](https://github.com/strongloop/loopback-component-oauth2),
we decide to postpone the migration guide to next stage.

We have a simplified OAuth 2.0 server implementation in example
[passport-login](https://github.com/strongloop/loopback-next/tree/master/examples/passport-login)'s
test fixtures, which sets up an express application as an OAuth 2.0 provider.
You can find the code in file
[mock-oauth2-social-app.ts](https://github.com/strongloop/loopback-next/blob/master/extensions/authentication-passport/src/__tests__/acceptance/fixtures/mock-oauth2-social-app.ts).
At this moment people who are interested to create such a provider can use it as
a reference.
