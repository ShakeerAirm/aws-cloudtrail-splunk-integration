# Root Account Usage Alert

## Desciprtion

Detects whenever the AWS account is used

##Risk

Root account usage should be extremely rare.Any activity should be investiaged

## SPL

index=aws sourcetype=aws:cloudtrail

userIdentity.type=Root

| table _time eventName eventsource sourceIPAddress

##Alert Condition 

Trigger when:

- Number of Results > 0

## Severity

High

## MITRE ATT&CK

TA0005 - Defense Evasion



