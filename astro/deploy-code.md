---
sidebar_label: 'Overview'
title: 'Deploy code to Astro'
id: deploy-code
description: Learn about the different ways you can deploy code to Astro.
---

To run your code on Astro, you need to deploy it to a Deployment. You can deploy part or all of an Astro project to an Astro Deployment.

There are two options for deploying code to a Deployment:

- **Image deploys**: Run `astro deploy` to build every file in your Astro project as a Docker image and deploys the image to all Airflow components in a Deployment. This includes your `Dockerfile`, DAGs, plugins, and all Python and OS-level packages. See [Deploy an image](deploy-project-image.md).
- **DAG-only deploys**: Run `astro deploy --dags` to deploy only your DAG files to Astro. If you only need to deploy DAG changes, running this command is faster than running `astro deploy` since it does not require installing dependencies. See [Deploy DAGS](deploy-dags.md).

For each deploy option, you can either trigger the deploy manually or through CI/CD. CI/CD pipelines can include both image deploys and DAG-only deploys, and they can deploy to multiple different Deployments based on different branches in your git repository. See [CI/CD overview](set-up-ci-cd.md).


## See also

- [Create an Astro project](develop-project.md#create-an-astro-project)
- [Develop your Astro project](develop-project.md)
