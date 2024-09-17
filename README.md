# DAO-Bitat Recommendation Service

## Overview

The DAO-Bitat Recommendation Service is a microservice designed to provide property recommendations based on user preferences. This service integrates with the DAO-Bitat platform, a decentralized property listing application built on React, Firebase, and Ethereum. The recommendation engine uses data from the Firestore database to suggest properties that users may be interested in.

## Features

- Fetches user data and favorite properties from Firestore.
- Implements a basic recommendation algorithm to suggest properties.
- Provides REST API endpoints for retrieving recommendations.

## Architecture

- **Technology Stack**: Go (Golang), Firebase Firestore
- **Database Structure**: 
  - `/users/userId`:
    - `name`: string
    - `email`: string
    - `role`: string
    - `profilePicture`: string
    - `contactInfo`: map
    - `createdAt`: timestamp
    - `/favorites/propertyId`:
      - `addedAt`: timestamp

## Setup

### Prerequisites

- Go 1.18 or higher
- Firebase account and Firestore setup

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/daoBitat-recommendation-engine.git
   cd daoBitat-recommendation-engine
