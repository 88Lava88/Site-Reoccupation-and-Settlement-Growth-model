# Site-Reoccupation-and-Settlement-Growth-model
A NetLogo agent-based model created for a course on Agent-Based Modelling for Archaeologists 

## Context:
Although the idea of modelling settlement dynamics is not new, I created my own simplified model from scratch that focuses specifically on site reoccupation. The model simulates the processes of habitation, abandonment and reoccupation of places. Inspired by patterns observed in some of the world’s longest-inhabited cities, including Jericho (11,000 years), Damascus (8,000 years), and Aleppo (5,000 years), where rebuilding on the same locations has maintained urban continuity for  many thousands years despite extreme changes in population and culture. 
## Conceptual Model

Key Relationships:
Agents arrive at the settlement, occupy patches, stay for a limited time, and then leave or die.  
Each patch gains a building level when occupied, Abandonment patches decay over time, lowering building levels.  

- **Building Level → Reoccupation Probability → Patch Occupation** (+)  
- **Patch Abandonment → Building Level** (−)  
- **High Building Level → Slower Decay** (+)  
- **Neighboring Agents → Patch Selection Probability** (+, social clustering to make the process more realstic)  
- **Overcrowding → Agent Moves to Another Patch** (−) 

## Elements
- **Red Agents (people):** Represent individuals who arrive in the settlement, occupy and build on it, stay for a limited lifespan, and then leave or die.
- **Patches (Buildings):** Represent locations that can be occupied.

### Building Level

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
- Social Settlement Preference: New agents preferentially settle on empty locations adjacent to existing inhabitants, promoting clustering and reuse of established areas.  
- Building Formation through Occupation: When a single agent occupies a location, the building level increases, representing maintenance, rebuilding, or incremental development.  
- Population Turnover: Agents have finite lifespans, ensuring continuous cycles of occupation and abandonment rather than permanent residency.  
- Decay and Persistence: Unoccupied buildings gradually deteriorate. More developed locations decay more slowly, making historically used areas more likely to be reused than unused land.  
- Reoccupation Feedback: Previously occupied locations retain higher building levels, increasing the probability of future settlement and reinforcing spatial persistence.





