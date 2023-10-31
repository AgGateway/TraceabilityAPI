# AgGateway Traceability API – The Foundation to Track Raw Agricultural Commodities

## Authors:
- Nieman, Scott; Digital Ag Architect – Land O’Lakes
- Wallace, Evan; Research Scientist – NIST
- Tevis, Joe; Agriculture Consultant – Vis Consulting
- Craker, Ben; Digital Portfolio Manager – AgGateway
- Oh, Hakju; connectCenter Software Architect - NIST

## Abstract

There is increasing demand for food traceability, ranging from consumers wanting to know where their food comes from (GMO, organic, climate-smart commodities), to manufacturers of agricultural inputs wanting to know the effectiveness of their products as used by farmers. Existing traceability requirements focus on the supply chain of goods packaged from their origin to retail grocery stores, with regulations provided by the Food Safety Modernization Act (FSMA) from the US Food and Drug Administration which suggests used of Critical Tracking Events and Key Data Elements to manage this challenge. Excluded from the list of foods, the Food Traceability List, for which additional information is required by FSMA are Raw Agricultural Commodities (RACs) such as grains and milk, which due to comingling, were viewed as a daunting effort to manage. AgGateway members studied this challenge since the FSMA's introduction, and introduced new types of Critical Tracking Events including the Transfer Event, when used with the Traceable Resource Unit, have become a foundation model to confidently manage RACs. This model is only limited by existing farm equipment design with regard to what can be accurately logged on a machine. However use of emerging AI-based grain and fluid flow models, and farm and field practice changes are supported by this model to improve the confidence in tracking RACs. Taking it a step further, the foundational model leveraged new and existing standards-based 'core components' assembled in a NIST developed software tool called 'connectCenter'. Utilizing connectCenter a general Traceability API was created as an OpenAPI specification describing endpoints to manage these resources, allowing software developers to generate code in the programming language of their choice and embed these capabilities into OEM platforms, farm management information systems, and retailer ERPs. This OpenAPI specification of the core concepts of the CTE, KDE, TRU and Containers are intended to simplify implementation, thus accelerating adoption making it easier for the farmer to meet the increasing traceability demands. 


# CART introduction of the Transfer Event
- The effort was formed ten (10) years ago as a collaboration between the Precision Ag Council and the Grain and Feed Council.
- Detailed business processes in BPMN.
- Concept of containers as an abstract object where a field could also be a container.
- Transfer between containers.
- Details listing of key data elements across business process areas
- Bluetooth experiments
# Origin of the Critical Tracking Event (CTE) and Key Data Elements (KDEs)
- Institute of Food Technologists
- Focus on Tracking in the Supply Chain
  -- external e(shipping, receiving) and
  -- internal tracking (manufacturing, food processing,batch, packaging)
- Key Data Elements
# Origin of Traceable Resource Unit (TRU) 
- Reference where TRU and CTE came from
- Summarize TRU University of Toronto
- Summarize “Fish/salmon paper” on TRU management
# Commingling of Commodities
- seed flow, grain flow modeling- reason this was lobbied to be out of scope
- informs equipment design considerations to capture better data with new equipment designs; e.g. planter mini-bulk boxes, storage bins, combine hoppers, tender systems - opportunity for innovation
- Lack of implementation of process control systems at grain elevators (dump pit to bin, bin to bin, dump pit to dryer, etc.)
- New combines may have the capability to shut off floor auger then clean out unload auger when the unload auger is “shut off”
# Reference to ontology work with Pascal Hitzler and Cogan KSU
- Ontology work presented a AgGateway, research work funded by NIST.  
- Quantity of Stuff
- Not only TransferEvent, but added Observation Event, Maintenance Event, Identification Event.  
# AgGateway Advancements 
- Transfer between source and target TRUs, where containers are part of it.  
- Leveraging of the Item Instance which is the quantity of Stuff.
- Data Link, add table to show these linkages; premise, if you know what you planted, you will know what you are harvesting
- Dataset Metadata-
  -- links between raw, processes and summarized datasets
  -- FAIR principles
  -- Dublin Core specialization,
- Links between datasets and business transactions
  -- Scale Ticket
  -- ASN from farmer is ideal, but few if any farmers have ERPs that can do that (open source ERPs would be great)
  -- Mix Ticket
- Could be represented in terms of a graph view
# Reference and Response to CAST work 
- GS1 centric, Institute of Food Technologists, Cornell.  
- Raw Ag Commodities as out of scope.
- We claim this is possible with a degree of accuracy
- The level of accuracy is study for future work, to define a confidence level in statistical terms, based on models and mathematical equations.
  

# A real Open API that can be used  
- V1 for as-planted
- Leverage an open source tool called connectCenter (formerly SCORE)
- model properies, relationships, definitions, examples
- visually create 'BIEs' pick and choose properties needed from existing components, most often identifiers, names, descriptions, quantities, classifiers, etc. based on the business context where it will be used in this case as-planted
- generates/expresses YAML document to open in Swagger Editor
- assembles multiple BIEs into endpoints for CRUD behavior based on anticipated uses; v3.2
- enables code generation for faster implementation in FMIS, ERP, process control systems, OEM platforms
- modern technology
# Standards-based Library from OAGi
- question on how to license API work?
- Reused components
- Other standards are manual maintenance slow to react
- Agile standard process, turnaround for changes within the month with regular release cycles
- connectCenter is used to manage the lifecycle of the standard itself, not just the implementation guidelines
# Future AgGateway and Affiliate Work Efforts
- More business contexts, refined BIE profiles
- Anticipate reuse as many capabilities for planting (transfers between TRUs)
- Transport to Grain Elevator
- Models internal to Elevator (collaboration with Universities)
- Reuse of components for improved generated code quality
- Improvements to NIST connectCenter;
  -- endpoint detail 3.3 with query and path parameters, HTTP headers, and
  -- example composition
- Retailer engagement
- OEM engagement (manufactured implements, monitors and platform APIs)
- Manufacturer engagement
- Response to Climate Smart Commodities and Organic asks
- ABABE paper for Planting, similar to Harvesting providing ISOXML mapping recommendations
# Need help - Opportunities for innovation would
- enable capturing better, more accurate data without putting extra work on the farmer to document everything
- In-Field Product Identifiation; QR code on delivery document, upload into tractor display; scenario
-- Seed as-filled, as-planted
-- Crop Protection as-mixed, as-applied
-- Crop Nutrition as-mixed, as-applied
- Container design; shouldering effects, remaining product between transfers
- Retrofit monitors for older equipment, smaller producers
# Summary
- Ten years of work, research on these challenges
- Need engagement
- Refinement will happen as we are focusing on Grain now
- Other business contexts/ scenarios
- 
