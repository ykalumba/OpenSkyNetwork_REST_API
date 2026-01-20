# OpenSky Network – Real-Time Flight State Data Pipeline

 ### Overview

This project demonstrates how to consume, process, and analyze real-time aircraft state vector data from the OpenSky Network REST API, specifically the states/all endpoint. 
The API provides live air traffic surveillance data collected from a global network of ADS-B and Mode S receivers.

The repository is designed to support data engineering, analytics, and data science use cases, including API ingestion, data transformation, storage, and exploratory analysis.

Data Source API Provider: <OpenSky Network>.The *states/all* endpoint returns a snapshot of all aircraft currently tracked by the OpenSky sensor network at a given time.

A state vector represents the instantaneous state of an aircraft at a specific timestamp. Each aircraft is represented as an array of values describing its identity, position, and movement.

The API response includes both A global timestamp and A list of aircraft state vectors.
Index	Field	Description
0	icao24	           – Unique 24-bit ICAO aircraft address (hexadecimal)
1	callsign	         – Aircraft callsign (may be null)
2	origin_country	   – Country inferred from ICAO address
3	time_position	    –  Timestamp of last known position
4	last_contact	     – Timestamp of last received signal
5	longitude	        – Longitude in degrees
6	latitude         	– Latitude in degrees
7	baro_altitude	    – Barometric altitude (meters)
8	on_ground	        – Boolean indicating if aircraft is on the ground
9	velocity	         – Ground speed (m/s)
10	true_track	      – Heading in degrees
11	vertical_rate    –	Vertical speed (m/s)
12	sensors	         – Sensor IDs (may be null)
13	geo_altitude	    – Geometric altitude (meters)
14	squawk	          – Transponder squawk code
15	spi	             – Special Purpose Indicator
16	position_source	– Position source (0 = ADS-B, 1 = ASTERIX, 2 = MLAT)





