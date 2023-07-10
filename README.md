# auth-examples

This repository contains submodules for Arcana Auth SDK usage examples. It covers different app types such as vanilla HTML/CSS/JS, React, NextJS, Wagmi, Rainbowkit, Web3-react, etc. It also has a sample that demonstrates custom login UI for supporting multiple social logins.

In this repo, you will see several git projects added as submodules.  Due to complexities involved, monorepo may not be required, at least for now.

## Pre-requisites:
Use Arcana Developer Dashboard, register the app and obtain Arcana Network ClientId for Testnet / Mainnet deployment. This is required before building/deploying the samples.

## Features demonstrated:
* App integration
* Using built-in, plug-and-play login UI to onboard users via configured social login such as Google, GitHub, Twitch, Twitter, Discord, Steam, etc.
* Using a custom login ui to onboard users
* Using passwordless login option for onboarding
* Using Custom IAM providers such as AWS Cognito, Firebase, etc., to onboard users
* Get User and account information, check login status, available login options
* Issue Web3 wallet operations such as add/switch networks and more for authenticated users, via the default embedded, non-custodia Arcana wallet UI or programmatically

## Git References for Submodules

If you wish to use these examples, use the git commands for repos with submodules. You can clone this repo using the command:

```sh
git clone --recurse-submodules https://github.com/arcana-network/auth-examples.git
```

Fetch latest updates in the example `sample-auth-cognito`:

```sh
git submodule update --remote sample-auth-cognito
```

Update the changes in all the submodules in the main project:

```sh
git submodule update --init --recursive
```
 
See these references for more details:
1.  https://git-scm.com/book/en/v2/Git-Tools-Submodules
2. https://github.blog/2016-02-01-working-with-submodules/

## Build and Deploy
To build and deploy individual samples, refer to the README.txt file in each example for specific instructions. Note that the default port is 3000 for some and 1234 for others.
