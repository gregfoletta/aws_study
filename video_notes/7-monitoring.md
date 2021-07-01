---
title: AWS Cloud Practicioner - Monitoring and Analytics
author: Greg Foletta
date: 7/6/2021
---

# CloudWatch

A web service that enables you to monitor and manage various metrics and cofigure alarm actions.

Uses metrics to represent the data points for resoures. The services send metrics to CloudWatch, and it uses these to create graphs that show how performance has changed over time.

## Alarms

Create alarms that automatically perform actions if the value of a metric goes above or below a predefined threshold.

As an example, create a CloudWatch alarm that stops EC2 instances when the CPU utilisation percentage has remained below a certain threshold.

# CloudTrail

Records API calls for your account. Events are typically updasted in CloudTrail within 15 minutes after an API call. Filter events by specifying the time and date a call was made, who made it, and the type of resource that was involved.

## Insights

Within CloudTrail you can also enable CloudTrail Insights. This allows CloudTrail to automatically detect unusual API activities within your AWS account.

# Trused Advisor

A web service thast inspects your AWS environment and provides real-time recommendations in accordance with AWS best practices.

Findings are broken down into five categories:

- Cost
- Optimisation
- Performance
- Security
- Fault Tolerance
- Service Limits

The dashboard shows recommendations broken down into these categories. Green indicates no problems, orange indicates recommended **investigations**, and red represents recommended **actions**.


