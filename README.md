# Digital Twin Development Documentation

Digital Twin
Digital twin is a dynamic, virtual representation of a physical object, process, or system. It mirrors the real-world entity by continuously collecting data from sensors, IoT devices, and other sources. This data is then processed and analyzed to create a digital replica that accurately reflects the behavior, status, and condition of its physical counterpart. By leveraging advanced technologies such as artificial intelligence, machine learning, and predictive analytics, digital twins can simulate various scenarios and predict future outcomes. This enables stakeholders to monitor performance, diagnose issues, optimize processes, and make data-driven decisions in real-time.  

## Production:

https://digital-twin-v2-chi.vercel.app/

## Repository (*Private) 
 
Code Repository:
 
https://github.com/kukuu/digital-twin-v2

This development covers:

Cloud deployment and hosting to AWS computing services Render for interfacing.
Superbase as ORM to host connection to Database and store environmental variables.
Vercel to host connection and configuration to versioning and source control of code repository in GitHub.
Updated UI to dynamically calculate the cost of Meter Reading cumulatively.
[Video is coming soon]


Production (Hosted by Render on AWS Computing Service):
https://digital-twin-v2-chi.vercel.app/


Manually Create the Table: Go to your Supabase project, navigate to SQL Editor, and run the following SQL to create the readings table:

 
CREATE TABLE readings (
  id SERIAL PRIMARY KEY,
  meter_id VARCHAR(255),
  reading FLOAT,
  timestamp TIMESTAMP
);
First open two terminals. Then CD into frontend and backend First you need to start the service by running : node server2.js Then start the react app by running : npm run start
