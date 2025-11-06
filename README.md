# omlox Hub by sensalytics – Quickstart Guide

Welcome to the **omlox Hub by sensalytics**! This guide will walk you through the steps required to get your own omlox
Hub instance up and running in just a few minutes.

## What is an omlox Hub?

The [omlox Hub](https://omlox.com/omlox-explained/omlox-hub-and-api) is a core component of the omlox ecosystem — a
location middleware that brings interoperability and flexibility to various tracking technologies, including UWB, RFID,
5G, BLE, Wi-Fi, and GPS.

The **omlox Hub by sensalytics** is a containerized implementation of the official omlox Hub API specification, making
it easy to deploy and integrate into your infrastructure.

# Basic Setup

## Prerequisites

Before you begin, make sure the following tools are installed on your system:

- [Docker](https://docs.docker.com/engine/install/)
- [Docker Compose](https://docs.docker.com/compose/install/)

> [!IMPORTANT]
> To use the omlox Hub, you’ll need a valid **trial license key**. You can request one by emailing us at
> `contact@sensalytics.io` or by filling out our [contact form](https://www.sensalytics.io/kontakt).

## Running the application

Follow these steps to get your omlox Hub instance up and running:

1. Clone the repository to your machine:
   ```bash
   git clone https://github.com/sensalytics-io/omlox-hub-setup.git
   cd omlox-hub-setup
   ```
2. Obtain your license file (.slyc) and place it in the `license` directory of the project.
3. Edit the `docker-compose.yml` file:
    - Replace `YOUR_LICENSE` with the actual filename of your `.slyc` license file.
4. Start the services using Docker Compose:
   ```bash
   docker-compose up -d
   ```
   This command will download the necessary images, create the containers, and start the omlox Hub in detached mode.

## Accessing the application

Once the containers are up and running, you can interact with your omlox Hub instance in the following ways:

- **API Endpoints:**  
  Test the API with a simple curl command:
  ```
  curl http://localhost:5000/v2/zones
  ```
- **Interactive API Documentation (Swagger UI):**  
  Open your browser and navigate to: http://localhost:5000/swagger-ui/index.html

> [!NOTE]
> The source code for omlox Hub is not included in this repository. It is maintained separately in a private repository.