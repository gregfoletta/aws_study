---
title: AWS Cloud Practicioner - Networking
author: Greg Foletta
date: 26/5/2021
---

# Connectivity

## VPC

VPC is a logically isolated section of AWS where AWS resources can be launched. Different subnets exist within a VPC.

## Internet Gateway

To allow public traffic from the internet to access the VPC, you attach an internet gateway to the VPC.

## Virtual Private Gateway

Used to access private resources in a VPC. An IPSEC tunnel is set up between the VPG and and an on-prem device.

## Direct Connect

This is a service that enables the establishment of a dedicated private connection between a data centre and a VPC.

# Subnets and ACLs

## Subnets

Section of a VPC in which shared resources can be grouped. Public subnets contain resources accessible from the internet, private subnets are only accessible through the private network. Subnets can communicate with each other.

## Network Access Control Lists

An access control list is a virtual firewall that controls inbound and outbound traffic at the subnet level.

By ddefault the network ACL is configured to allow all inbound and outbound traffic. This can be modified by adding your own rules. Network ACLs are **stateless**.

## Security Group

A security group is a virtual firewall that controls inbound and outboujnd traffic for an EC2 instance. By default it denies inbound and allows outbound. Multiple EC2 instances can be associated with the same security group. Security groups are **stateful**.

# Global Networks

## DNS

Route 53 is a DNS web service, as well as a registrar. CloudFront CDN ties in with DNS as well. Here's an example flow:

1. Request comes to Route 53
1. Route 53 responds
1. Customer request is sent to the nearest edge location
1. CloudFront connects to the **Application Load Balancer**, which sends it to an EC2 instance.

