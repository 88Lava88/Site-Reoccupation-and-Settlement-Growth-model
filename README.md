# Site-Reoccupation-and-Settlement-Growth-model
A NetLogo agent-based model created for a course on Agent-Based Modelling for Archaeologists  https://codarchlab-abm.github.io/course-guide/ 

## Context:
Although the idea of modelling settlement dynamics is not new, I created my own simplified model from scratch that focuses specifically on site reoccupation. The model simulates the processes of habitation, abandonment and reoccupation of places. Inspired by patterns observed in some of the world’s longest-inhabited cities, including Jericho (11,000 years), Damascus (8,000 years), and Aleppo (5,000 years), where rebuilding on the same locations has maintained urban continuity for  many thousands years despite extreme changes in population and culture. 

## Conceptual Model
### Core Process
Agents arrive at the settlement, occupy patches for a limited time, and then leave or die. When a patch becomes unoccupied, it begins to decay. Reoccupation increases the patch’s building level, which reduces its rate of decay. Through these cycles, the model investigates how long-term spatial persistence can emerge despite continuous population turnover. 

- Agent Arrival (+) → Occupied Patches
- Agent Death (+) → Vacant Patches
- Vacant Patches (+) → Probability of Reoccupation
- Reoccupation (+) → Building Level
- Building Level (−) → Decay Rate


## Elements
- **Red Agents (people):** Represent individuals who arrive in the settlement, occupy and build on it, stay for a limited lifespan, and then leave or die.
- **Patches (Buildings):** Represent locations that can be occupied.

### Building Levels

- Each patch in the settlement stores a building level  
- The building level increases each time an agent occupies the patch. The more frequently a spot is reoccupied, the higher its level becomes.  
- Patches with higher building levels decay more slowly, representing the long-term persistence of heavily used locations.  
- Color Code: The color scale visually encodes the history of occupation 
  - **Green patches:** Empty areas  
  - **White:** First-time occupation  
  - **Light to medium grey:** reoccupied areas    
  - **Dark grey:** Heavily reoccupied areas  
  - **Black:** Continuously occupied areas that decay much slower
 
## Key Mechanisms
 - Settlement Size: Determines the radius of habitable patches. Larger settlements provide more space for agents.
 - Lifespan: Determines how long each agent remains on a patch.
 - Spawn Rate: Controls how often new agents arrive.
 - Social Settlement Preference: New agents settle on empty location, preferentially next to already occupied areas to simulate realsitic social clustering.






