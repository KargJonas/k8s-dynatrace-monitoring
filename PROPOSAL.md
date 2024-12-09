# Monitoring a Kubernetes application with Dynatrace

Our goal for this project is:
1. Take the frontend and backend of an existing project and host it using Kubernetes.
2. Monitor the application.
3. If time permits, we might try to add CI/CD pipelines to some parts of the project (all three components require a build step and both frontend and backend need to be hosted somewhere).

Our cloud service provider will be Google Cloud and we will be using Dynatrace for the application monitoring part.
Additionally we will try to simulate stress conditions by artificially degrading the health of the application or creating some synthetic traffic to generate some interesting data.

## Team
- Samuel Grünbacher (K12213653)
  - Set up Kubernetes on Google Cloud
- Tobias Müller (K12209522)
  - Containerize/host frontend
  - Set up Dynatrace and monitor Project
- Jonas Karg (K12213152)
  - Containerize/host backend
  - Simulate system degradation/high load

## Milestones
- Set up Kubernetes on Google Cloud
- Containerize/host backend
- Containerize/host frontend
- Set up Dynatrace and monitor Project
- Simulate system degradation/high load
- (Set up CI/CD pipelines)

## Info about the base project
The project this will be based on is a multiplayer snake game called "Multisnake" that consists of a frontend, a backend and a mobile application for IOS and Android.

The backend and frontend can already be run independently of one another so it should be relatively easy to run them in containers using Kubernetes.

## Current Architecture
![Multisnake architecture](multisnake-architecture.png)