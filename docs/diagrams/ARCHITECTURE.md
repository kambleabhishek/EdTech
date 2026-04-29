# Architecture

## Overview
Monolithic Spring Boot backend serving REST APIs for Web and Mobile clients.

## Components
- Frontend: React (Web), React Native (Mobile)
- Backend: Spring Boot (single deployable unit)
- Database: MySQL
- Storage: AWS S3 (videos)
- CDN: CloudFront
- Payment: Razorpay

## Flow
Client → REST API → Service Layer → DB  
Client → S3 (via signed URL for video streaming)

## Scaling Plan
- Start: Single EC2 instance
- Later: Add load balancer + multiple instances
- DB: Move to AWS RDS
