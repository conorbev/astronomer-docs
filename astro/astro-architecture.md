---
sidebar_label: 'Architecture'
title: 'Astro architecture'
id: astro-architecture
description: Learn about how Astro is structured to maximize the power of Apache Airflow.
---

Astro is a managed service for data orchestration that is built for the cloud and powered by Apache Airflow. Your Airflow infrastructure is managed entirely by Astronomer, enabling you to shift your focus from infrastructure to data. 

There are two ways to run Astro:

- _Astro Hosted_ is a version of Astro that's hosted and managed on Astronomer's Cloud. This version of Astro is ideal if you want to run Airflow with as little friction as possible.
- _Astro Hybrid_ is a version of Astro that's managed by Astronomer, but your Airflow infrastructure is hosted in your company's cloud. This version of Astro is ideal for companies that want more control over their cloud infrastructure. 

Astro Hosted consists of three core components for managing Airflow, all hosted on Astronomer's cloud:

- The _Astro control plane_ is Astronomer's interface for managing your Airflow environments in the cloud. It includes the Cloud UI, the Astro CLI, and Cloud API.
- An _Astro cluster_ comprises all the components necessary to host multiple Airflow Deployments, including the network, database, and compute resources.
- A _Deployment_ is an Airflow environment running on Astro. Each Deployment includes all of the core Airflow components, plus additional Astronomer tooling that help you optimize resource usage, observability, and security.

Astro Deployments can securely connect to external data services so that you can place Airflow at the heart of your data ecosystem. 

![Astro Hosted overview](/img/docs/architecture-overview.png)

To learn more about Astro Hybrid architecture and features, see [Astro Hybrid overview](hybrid-overview.md)

