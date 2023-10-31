# AgGateway Traceability API – The Foundation to Track Raw Agricultural Commodities

## Authors:
- Nieman, Scott; Digital Ag Architect – Land O’Lakes
- Wallace, Evan; Research Scientist – NIST
- Tevis, Joe; Agriculture Consultant – Vis Consulting
- Craker, Ben; Digital Portfolio Manager – AgGateway
- Oh, Hakju; connectCenter Software Architect - NIST

## Abstract

There is increasing demand for food traceability, ranging from consumers wanting to know where their food comes from (GMO, organic, climate-smart commodities), to manufacturers of agricultural inputs wanting to know the effectiveness of their products as used by farmers. Existing traceability requirements focus on the supply chain of goods packaged from their origin to retail grocery stores, with regulations provided by the Food Safety Modernization Act (FSMA) from the US Food and Drug Administration which suggests used of Critical Tracking Events and Key Data Elements to manage this challenge. Excluded from the list of foods, the Food Traceability List, for which additional information is required by FSMA are Raw Agricultural Commodities (RACs) such as grains and milk, which due to comingling, were viewed as a daunting effort to manage. AgGateway members studied this challenge since the FSMA's introduction, and introduced new types of Critical Tracking Events including the Transfer Event, when used with the Traceable Resource Unit, have become a foundation model to confidently manage RACs. This model is only limited by existing farm equipment design with regard to what can be accurately logged on a machine. However use of emerging AI-based grain and fluid flow models, and farm and field practice changes are supported by this model to improve the confidence in tracking RACs. Taking it a step further, the foundational model leveraged new and existing standards-based 'core components' assembled in a NIST developed software tool called 'connectCenter'. Utilizing connectCenter a general Traceability API was created as an OpenAPI specification describing endpoints to manage these resources, allowing software developers to generate code in the programming language of their choice and embed these capabilities into OEM platforms, farm management information systems, and retailer ERPs. This OpenAPI specification of the core concepts of the CTE, KDE, TRU and Containers are intended to simplify implementation, thus accelerating adoption making it easier for the farmer to meet the increasing traceability demands. 


CART introduction of the Transfer Event
Reference to ontology work with Pascal
Reference to CAST work that has raw ag commodities as out of scope
Details of TRU and additional CTE types
Reference where TRU and CTE came from
TRU University of Toronto
“Fish/salmon paper” on TRU management
CTE came from institute of food technologists
Co-mingling, seed flow, grain flow modeling out of scope but may inform equipment design considerations to capture better data with new equipment designs
e.g. planter boxes, storage bins, combine hoppers, tender systems - opportunity for innovation
New combines may have the capability to shut off floor auger then clean out unload auger when the unload auger is “shut off”
Opportunities for innovation would enable capturing better, more accurate data without putting extra work on the farmer to document everything
Concrete v1 API using a tool to generate based on reflections of the model and how that enables code generation for faster implementation
Open source tool
Library from OAGi, question on how to license API work?
Reused components
