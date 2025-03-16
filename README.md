# Manus-Sentiment

# Sentiment Analysis Tool Deployment Guide

## Overview

This project has been restructured and configured for serverless deployment on Vercel. The following sections outline the necessary configuration files, application restructuring, and deployment instructions.

## Configuration Files

- **vercel.json**: Configures how Vercel should build and serve your application.
- **requirements.txt**: Lists all Python dependencies needed for deployment.

## Application Restructuring for Serverless Deployment

- Created an **api** directory with `index.py` as the entry point.
- Modified the Flask application to work in a serverless environment.
- Added automatic NLTK resource downloads during cold start.
- Created a detailed deployment guide in `docs/vercel_deployment.md`.

## Deployment Instructions

The project is now ready for deployment to Vercel. To complete the deployment, follow these steps:

1. **Login to your Vercel account using the Vercel CLI:**

   `vercel login`

2. **Deploy the project by running:**

   `vercel`

3. **Follow the interactive prompts to complete the deployment.**

After deployment, Vercel will provide you with a URL where your Sentiment Analysis Tool is accessible.

**Note:** The first request might be slow due to cold start and NLTK resource downloads, but subsequent requests will be faster.

If you need any adjustments or further clarification, just let me know!
