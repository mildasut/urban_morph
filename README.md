# Optimizing City Form: Building Parameters Across Urban Morphotypes and City Sizes

![My Image](Urban.png)


## Summary

This project focuses on identifying the ideal urban parameters – such as floor-to-plot area ratio, building-to-plot area ratio, building height, population density, etc. – based on urban morphotype and city size, driving data-based planning for more livable and efficient cities. 


## Background

I am an architect and urban planner, and this is a real task I have in my job. My task is to update territory planning norms in my country that were created mostly intuitively 10 – 15 years ago. These territory planning norms looked somewhat ok at the time, but never became really integrated in real territory planning, as they lack the precision required to solve real problems and often raise more questions than gives answers. The problem I am seeking to solve is the gap between these outdated norms and the wealth of data and tools now available to acquire better decision-making.

This issue is highly prevalent in urban planning today. Many city planners still rely on their intuitive expertise, while the data is still hardly reachable and the goals in the outdated norms are somewhat sketchy. This result in cities that lack efficiency, livability and sustainability. By updating norms for territory planning and integrating evidence-based decision-making into it, we could create urban spaces that are more adaptable, equitable, and responsive to the needs of modern societies, while being gentle with surrounding nature.

My personal motivation comes from the desire to find a right balance between cities and nature, work and free-time, social and individual spaces. As a professional in this field, I see how outdated planning processes can lead to inefficient land use, poor environmental outcomes, and less desirable living conditions. On a larger scale, these issues affect not only the residents’ well-being but also economic vitality and environmental sustainability.

The importance of this topic cannot be overstated. By modernizing territory planning norms and making them more data-driven, we can work toward creating more livable cities – places where people want to live, work, and interact with their surroundings. This aligns with modern urban planning concepts like the "15-minute city," which focuses on designing cities where everything people need is within a 15-minute walk or bike ride. The benefits of such an approach include reducing pollution, fostering community interaction, and enhancing overall quality of life.

Ultimately, this project addresses a crucial need to rethink how we plan cities to make them more human-centric, economically viable, and environmentally sustainable.


## Data sources and AI methods

This project will rely heavily on Geographic Information Systems (GIS) technology, which will be used to analyze urban morphology and define key urban planning parameters. The work is divided into three major tasks, each leveraging different data sources and AI techniques.

1. Defining Urban Morphotypes:
The first part of the project aims to define an optimal number of urban morphotypes (likely up to 10) that would be representative at the country level and applicable to cities and towns of different sizes. To achieve this, the project will use orthophoto, satellite, or lidar imagery, along with the polygons of registered plots in urbanized areas (which I already have). The analysis will focus solely on urban areas. The challenge here lies in defining the morphotypes themselves. I plan to explore the use of Neural Networks (NN) and clustering algorithms to automate and enhance the classification process. By using AI, I hope to develop a data-driven classification that may provide more nuanced or efficient categories than what could be achieved through manual classification by experts. The use of clustering will help group similar urban morphologies, and NN techniques could assist in identifying patterns that are not immediately obvious to human analysis.

2. Finding Optimal Urban Parameters:
The second task involves identifying optimal urban parameters for each morphotype. Different parameters must be determined for two different polygons (plots and urbanized areas):
* Plot-level parameters: floor-to-plot ratio, building-to-plot ratio, building height (stories and meters), and dwelling density, which must be calculated for the polygons of registered plots.
* Urbanized-area-level parameters: population density, calculated for urbanized territory polygons based on statistical data.
Data for this analysis will come from government institutions, including polygons of plots and urbanized areas, population and dwelling data from state data agency, and real estate databases that contain information on plots, buildings, and premises from the state real estate registry. Regression models will likely be used to analyze these relationships and to find the optimal values for each parameter across different morphotypes. This step will involve a mix of supervised learning and traditional statistical analysis to predict the best-fit parameters for each urban form.

3. Categorizing Towns and Cities:
The third task involves categorizing cities and towns into different classes and assigning coefficients that reflect the varying urban parameters by city size. The goal is to account for the fact that smaller towns will have different optimal parameters compared to larger cities like the capital. This could be achieved through clustering techniques, which would group towns and cities based on shared characteristics, followed by regression models to adjust the parameters accordingly for each category.

Overall:
The availability of high-quality official data ensures a strong foundation for this analysis. However, one potential challenge is that some urbanized areas lack officially registered plots, particularly in certain morphotypes. This presents a challenge in evaluating territories consistently. The model will need to account for this discrepancy, possibly by developing alternative methodologies to estimate parameters for these areas.


## How is it used?

The solution will be used to modernize national territory planning norms, creating a more data-driven, evidence-based framework for urban planning. Once the norms are updated, they will serve as a benchmark for evaluating future territory planning documents.

The primary users of this solution include: municipalities (who initiate and oversee the development of territory planning documents for their regions), territory planners (who design and propose urban plans based on these updated norms), national territory planning supervisors (who will evaluate and ensure that local plans comply with the new standards). 

While the direct users are professionals in urban planning and governance, the impact of this solution will extend to the entire society. Improved territory planning leads to better-designed cities, benefiting residents through more livable, sustainable, and economically vibrant urban environments. This would affect people’s everyday lives, including how they move around the city, access services, interact with the environment, and enjoy the urban space. Considering these diverse stakeholders ensures that the solution not only meets professional requirements but also contributes to creating cities where people truly want to live.


## Challenges

The biggest challenge is that society and cities are evolving rapidly, often driven by shifts in political priorities. If political direction changes, the established norms may struggle to keep up. That’s why it’s crucial to develop a flexible, updatable model – one that can be regenerated every year or so, ensuring that regulations remain relevant.

Additionally, it’s important to acknowledge the complexity of cities and human behavior. Expecting a perfect model from the start in this case would be unrealistic. Instead, the focus should be on identifying potential weaknesses early on and being prepared to refine and optimize the model over time.


## What next?

The project could evolve into a dynamic, self-sustaining model capable of evaluating territory planning documents autonomously. This "live" model would not only identify flaws or inconsistencies in proposed plans but also offer data-driven recommendations for improvement. Over time, it could incorporate real-time data, continually learning and adapting to new urban trends and policies, making urban planning more efficient, responsive, and precise.


## Acknowledgments

I would like to acknowledge the key concepts that inspired this project, particularly the "15-minute city," "livable city," and "New Urbanism." The "15-minute city" emphasizes creating urban environments where all essential services and amenities are accessible within a 15-minute walk or bike ride, fostering community interaction and reducing dependence on cars. The "livable city" concept prioritizes the quality of life for residents, advocating for green spaces, sustainable infrastructure, and inclusive public areas that cater to diverse populations. "New Urbanism" further enriches this dialogue by promoting walkable neighborhoods, mixed-use developments, and a strong sense of community, all of which contribute to sustainable urban living. Together, these frameworks serve as guiding principles for my work, reinforcing the need for data-driven, adaptable planning norms that enhance urban livability and responsiveness to societal needs. Through their lens, I aim to contribute to the ongoing conversation about creating vibrant, sustainable cities for the future.
