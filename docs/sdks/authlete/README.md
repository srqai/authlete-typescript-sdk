# Authlete SDK

## Overview

Authlete API: Authlete API Explorer

Welcome to the Authlete API documentation. Authlete is an API-first service where every aspect of the platform is configurable via API. This explorer provides a convenient way to authenticate and interact with the API, allowing you to see Authlete in action quickly.

At a high level, the Authlete API is grouped into two categories:
- Management APIs: Enable you to manage services and clients
- Runtime APIs: Allow you to build your own Authorization Servers or Verifiable Credential (VC) issuers

All API endpoints are secured using access tokens issued by Authlete's Identity Provider (IdP). If you already have an Authlete account, simply use the Get Token option on the Authentication page to log in and obtain an access token for API usage. If you don't have an account yet, sign up at https://console.authlete.com/register to get started.

API Servers:
Authlete is a global service with clusters available in multiple regions across the world. Currently, our service is available in the following regions:
- US Cluster
- Japan Cluster  
- Europe Cluster
- Brazil Cluster

Our customers can host their data in the region that best meets their requirements.

Authentication:
The API Explorer requires an access token to call the API. You can create the access token from the Authlete Management Console and set it in the HTTP Bearer section of Authentication page. Alternatively, if you have an Authlete account, the API Explorer can log you in with your Authlete account and automatically acquire the required access token.

Important Note: When the API Explorer acquires the token after login, the access tokens will have the same permissions as the user who logs in as part of this flow.

Tutorials:
If you have successfully tested the API from the API Console and want to take the next step of integrating the API into your application, or if you want to see a sample using Authlete APIs, follow the links below. These resources will help you understand key concepts and how to integrate Authlete API into your applications.

- Getting Started with Authlete: https://www.authlete.com/developers/getting_started/
- From Sign-Up to the First API Request: https://www.authlete.com/developers/tutorial/signup/

Contact Us:
If you have any questions or need assistance, our team is here to help. Visit our Contact Page at https://www.authlete.com/contact/

### Available Operations
