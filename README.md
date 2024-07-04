# Tire Tread Scanner for the Web

## Overview

The Tire Tread Instant App SDK project repository is a structured codebase demonstrating the usage of Anyline's Tire Tread Instant App SDK. The SDK provides the funtionality to use Anyline's Tire Tread scanner as Instant App/App Clip from a web page. This document provides an overview of the repository structure and explaining the purpose of each folder and key files. 

## Repository Structure

- `README_SDK.md`: A detailed README file specific to the Tire Tread Instant App SDK, explaining its usage, features, and integration.

##### Public Directory: `/public` This directory contains all the frontend assets and HTML files for the demo web application.

- `/public/index.html`: The starting point of the demo integration of the Tire Tread Instant App SDK.
- `/public/sdk/ttr_sdk.js`: The Tire Tread Instant App SDK JavaScript file.

##### Result Directory: `/public/result` This directory holds files related to displaying the results of the tire tread scan.

- `/public/result/result.html`: HTML file displaying the outcome of the tire tread scanning process.

##### Error Directory: `/public/error` Includes files for error handling in the web application.

- `/public/error/index.html`: HTML file that displays error messages or information.

##### API Directory `/api` This directory contains an example implementation of the backend API end-points.
We strongly recommend implementing this functionality in the backend so that the license key is not exposed on the frontend. This is an example implementation in JavaScript for a serverless infrastructure. However, the choice of backend technology is not relevant; you can rebuild the rather simple end-points in any language/framework of your choice, or integrate them into your existing backend. We also recommend securing the communication between the frontend and backend (depending on your use-case using CORS, CSRF protection, authentication, rate limiting, etc.).

- `/api/getToken.js`: Backend script for generating and providing a scanning token.
- `/api/getResult.js`: Backend script for processing and returning the results of the tire tread scan.
