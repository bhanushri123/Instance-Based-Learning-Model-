

**Title: Multi-Human Intelligence in Instance-Based Learning for Robot Decision Making**

**Overview:**
This project focuses on developing an intelligent decision-making system for robots using a concept called Instance-Based Learning (IBL). The primary goal is to enable robots to learn from past experiences and mimic human behavior in various scenarios. The project involves the following key steps:

**Training and Knowledge Feeding:**
- In IBL, past experiences are stored as <situation, decision, utility> (SDU) triplets, known as instances.
- Each instance represents a unique scenario where a decision was made by a human or robot.
- Instances are used to train the robot's memory, allowing it to learn from historical data.

**Similarity Function:**
- To find past experiences similar to the current situation, a similarity function is employed.
- This function calculates the distance between two vectors, typically the current situation vector and memory experience vectors.
- Different methods like Cosine distance and Euclidean distance are used, with Cosine distance being the current choice.

**Activation and Probability of Retrieval:**
- Instances are assigned activation values, which represent their relevance, frequency, recency, and similarity to the current situation.
- Probability of retrieval is determined based on the weightage of each instance.
- The higher the activation, the more likely an instance will be retrieved.

**Blended Value and Decision Making:**
- Blended Value is a scoring mechanism used to evaluate decision alternatives.
- The decision with the maximum Blended Value is chosen as the optimal action.
- This enables the robot to make informed decisions in complex scenarios.

**Application to a Search-and-Retrieval Game:**
- The project includes the development of a single-player search-and-retrieval game.
- The game simulates a scenario where the robot collects target objects while avoiding distractors.
- Player actions, rewards, and situation vectors are recorded during the game.
- The robot uses this data to learn and improve its decision-making abilities.

**Main Work and References:**
- The main work is based on the research paper titled "Multi-human intelligence in Instance-Based Learning," which can be found [here](https://www.researchgate.net/publication/364348448_Multi-human_intelligence_in_Instance-Based_Learning).
- Additional resources, including presentations and related papers, are also available for further understanding.

**Supplementary Information:**
- You can find more details about IBL theory and its practical applications in the provided supplementary materials, including videos and articles.

**Project Purpose:**
The purpose of this project is to develop an intelligent decision-making system for robots using Instance-Based Learning. By mimicking human behavior and learning from past experiences, the robot can make informed decisions in complex and dynamic environments.

**Note:**
Please refer to the provided resources and research paper for in-depth technical details and implementation specifics.
