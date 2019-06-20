# ec2-state-change-notification-to-slack

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/bf66aabcf19744bc9f0edd97941cf819)](https://www.codacy.com/app/mamori017/ec2-state-change-notification-to-slack?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mamori017/ec2-state-change-notification-to-slack&amp;utm_campaign=Badge_Grade)
[![CodeFactor](https://www.codefactor.io/repository/github/mamori017/ec2-state-change-notification-to-slack/badge)](https://www.codefactor.io/repository/github/mamori017/ec2-state-change-notification-to-slack)
[![BCH compliance](https://bettercodehub.com/edge/badge/mamori017/ec2-state-change-notification-to-slack?branch=master)](https://bettercodehub.com/)
[![Release](https://img.shields.io/github/release/mamori017/ec2-state-change-notification-to-slack.svg)](https://github.com/mamori017/ec2-state-change-notification-to-slack/releases/latest)
[![License](https://img.shields.io/github/license/mamori017/ec2-state-change-notification-to-slack.svg)](https://github.com/mamori017/ec2-state-change-notification-to-slack/blob/master/LICENSE)

![201906201800](https://user-images.githubusercontent.com/7507701/59831588-0e341480-937d-11e9-8262-a817f24178be.png)

## Overview

Amazon EC2 state change notification to Slack.

## Requirement

Runtime : Node.js 10.x

## Usage

1. Enable AWS CloudTrail.

2. Create Amazon CloudWatch event rule.
    | Event pattern |  |
    |:-----------|:------------|
    | Service Name | EC2 |
    | Event type | EC2 Instance State-change Notification  |
    | State | Any *1 |
    | Instance | Any *1 |
    | Target | Lambda function |

    *1 : Change when specifying a specific state or instance.

3. Create Lambda function with this code.

## Licence
[MIT](https://github.com/mamori017/ec2-state-change-notification-to-slack/blob/master/LICENSE)

## Author
[mamori017](https://github.com/mamori017)
