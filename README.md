# OpenSky Network – Real-Time Flight State Data Pipeline

 ### Overview

This project demonstrates how to consume, process, and analyze real-time aircraft state vector data from the OpenSky Network REST API, specifically the states/all endpoint. 
The API provides live air traffic surveillance data collected from a global network of ADS-B and Mode S receivers.

The repository is designed to support data engineering, analytics, and data science use cases, including API ingestion, data transformation, storage, and exploratory analysis.

Data Source API Provider: <OpenSky Network>.The *states/all* endpoint returns a snapshot of all aircraft currently tracked by the OpenSky sensor network at a given time.

A state vector represents the instantaneous state of an aircraft at a specific timestamp. Each aircraft is represented as an array of values describing its identity, position, and movement.

The API response includes: 
  ## A global timestamp
  ## A list of aircraft state vectors


