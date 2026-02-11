# FlashLearn Card Service

## Overview

The FlashLearn Card Service is a serverless backend microservice responsible for managing flashcards within decks in the FlashLearn platform.

It enables users to create, update, retrieve, and delete flashcards while enforcing secure access using Amazon Cognito JWT authorization.

This service operates fully within the AWS Always Free Tier.

---

## Architecture

- AWS Lambda (Card business logic)
- Amazon API Gateway (REST API endpoints)
- Amazon DynamoDB (Card persistence)
- Amazon Cognito (Authentication and JWT validation)
- IAM roles with least privilege access

---

## Responsibilities

- Create flashcards within decks
- Retrieve cards by deck
- Update card content
- Delete flashcards
- Enforce deck ownership validation

---

## Security

- Cognito User Pool integration
- JWT-based authorization via API Gateway
- User identity extraction from token claims
- User-scoped data isolation
- IAM least privilege permissions

---

## Deployment Model

Deployed independently within a distributed serverless microservices architecture.

All API requests require a valid Cognito access token in the Authorization header.

---

## Tech Stack

- Node.js
- AWS Lambda
- DynamoDB
- API Gateway
- Amazon Cognito

---

## Status

Initial card service scaffolding and architecture setup.
