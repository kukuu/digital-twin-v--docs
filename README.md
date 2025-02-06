# Digital Twin Development Documentation

Digital Twin
Digital twin is a dynamic, virtual representation of a physical object, process, or system. It mirrors the real-world entity by continuously collecting data from sensors, IoT devices, and other sources. This data is then processed and analyzed to create a digital replica that accurately reflects the behavior, status, and condition of its physical counterpart. By leveraging advanced technologies such as artificial intelligence, machine learning, and predictive analytics, digital twins can simulate various scenarios and predict future outcomes. This enables stakeholders to monitor performance, diagnose issues, optimize processes, and make data-driven decisions in real-time.  

## V2
Hosted by Render on AWS Computing Service.

### Production: 

https://digital-twin-v2-chi.vercel.app/
 
### Code Repository (*Private) : 

https://github.com/kukuu/digital-twin-v2

### Summary:

Cloud deployment and hosting to AWS computing services Render for interfacing.
Superbase as ORM to host connection to Database and store environmental variables.
Vercel to host connection and configuration to versioning and source control of code repository in GitHub.
Updated UI to dynamically calculate the cost of Meter Reading cumulatively.
[Video is coming soon]

## Execution steps

Manually Create the Table: Go to your Supabase project, navigate to SQL Editor, and run the following SQL to create the readings table:



```
CREATE TABLE readings (
  id SERIAL PRIMARY KEY,
  meter_id VARCHAR(255),
  reading FLOAT,
  timestamp TIMESTAMP
);

```



First open two terminals:

i. cd into frontend and then into backend 

ii. Start the service by running : 

```
node server2.js


```

in the  backend

iii. Then start the react app by running : 

```
npm run start

```

In the frontend.

## V3

1. Clerk or Kinde based Authentication workflows. Login prompt when the user is not signed-in. Before selecting the meter or when he clicks on the user.
2. Calculation modal when Meter is selected. And then send the calculated data to the logged-in user.
3. Ingestion of user custom data
4. Processing of user data

## V4
https://github.com/kukuu/digital-twin-PV4-/blob/digi-twin-v1/README.md
  

