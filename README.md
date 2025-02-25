# Digital Twin Development Documentation

Digital Twin
Digital twin is a dynamic, virtual representation of a physical object, process, or system. It mirrors the real-world entity by continuously collecting data from sensors, IoT devices, and other sources. This data is then processed and analyzed to create a digital replica that accurately reflects the behavior, status, and condition of its physical counterpart. By leveraging advanced technologies such as artificial intelligence, machine learning, and predictive analytics, digital twins can simulate various scenarios and predict future outcomes. This enables stakeholders to monitor performance, diagnose issues, optimize processes, and make data-driven decisions in real-time.  

## V2 (Node/TypeScript) - POC
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


### Execution steps

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

## V3 (Node/TypeScript)

1. **Clerk or Kinde based Authentication workflows**. Login prompt when the user is not signed-in. Before selecting the meter or when he clicks on the user.
2. **Modal** to show selected Meter for updating/inserting consumed energy reading.
3. **TOTAL updates dynamically**
4. All fields in the MODAL are **read only except for the READING field which is READ/WRITE**
5. Send the calculated data to the logged-in user/Energy Supplier. For now set it to **alex@azzotto.com**
6. Add **PAYMENT GATEWAY** to supplier. For now lets use c**onfigurations and USER requirement details from lovejoint.store** - https://www.lovejoint.store/

   **Staging** - https://digital-twin-neon.vercel.app/

## V4 (Python/Node/TypeScript)

Enabling real-time monitoring, optimisation, and predictive insights, improving efficiency, reducing costs, and enhancing decision-making.

This high-volume throughput system exemplifies real-time asynchronous data processing capability ensuring scalability, reliability, flexibility, observability, security and addresses challenges like schema evolution and fault tolerance.

https://github.com/kukuu/digital-twin-PV4-/blob/digi-twin-v1/README.md

## Boiler 

#### Problem Statement - Gathered & Found

Here is a clearer insight into this particular engagement.

- Phase One: Mobilise a small team to collate all data that the client has from the past 4 years to build a model and simulation of previous damage caused to their boiler and physical products. Once this is done, we can then look to create a predictive model to estimate when damage begins to occur, and when they should start to look at repairs or changing parts of the system.

Additionally, we will build a (3D Digital) Twin of their physical product, which will digest the data produced by the testers to create easily viewed images to show where the biggest causes for concern are, and where they need to act. A big issue for the tech org is that the board are non-technical, so spreadsheets don’t cut it. Even having a basic, but aesthetically pleasing image, would make for better board understanding and therefore potential future investment.


- Phase Two: Once this is delivered and lands well, look to scale this solution across their other 4 UK sites (brand new projects), and bring the rest of the business into the new venture.
 
- Phase Three: scale the product further past the boiler (biggest issue) and into their pressure tanks (second biggest issue) and then into the physical pipelines that produce the energy (third biggest).

- Aspirational Target: Build alerting system across their UK sites to alert the maintenance and engineering teams when human error has occurred, and when there are major issues that may have gone unidentified.


#### High-level Solution Design

As part of the requirement-gathering process, I have identified key areas that need to be addressed with stakeholders. While the list below is not exhaustive, it serves as an initial framework that will continue to evolve as we progress through the discovery and requirement-gathering phases:
1. _Key parameters that are being monitored._

2. _Features/labels on their data._

3. _What are the metrics that need to be optimized?_
4. _Reports/charts they are interested in._
5._ Operational workflows ( if possible) so that we can suggest for improvements_

If we get the above requirements then we can proceed like this:

1. _We will use python for data ingestion and exploratory data analysis.(EDA)_
2. _For EDA we use Matplotlib and Seaborn plots for graphs and charts that will give some insights into our data sets._
3._ We will then be able to identify important features and labels._
4. _We can use Regression to perform predictions._
5. _Assuming huge data sets we can also generate custom ML models to perform prediction._
6. _In the Frontend we can show Charts/ Graphs._
7. _We can develop a UI that will enable technicians to see simulation results for input parameters._
8._ We will use Streamlit (python library best suited to showcase AI models-based simulations)._


  

