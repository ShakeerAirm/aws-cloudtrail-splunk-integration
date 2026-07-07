# Failed AWS Console Login

## Description

Detects failed AWS Management Console login attempts.

## SPL

```spl
index=aws sourcetype=aws:cloudtrail

eventName=ConsoleLogin

errorMessage="Failed authentication"

```

## Alert

Trigger if more than 5 failed logins occur within 15 minutes.

## Severity

Medium
