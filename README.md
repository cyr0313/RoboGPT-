# RoboGPT-
RoboGPT: an intelligent agent of making embodied long-term decisions for daily instruction tasks

We develop a verification system based on the Ai2Thor simulation system. You can input arbitrary natural language commands and use the RoboGPT agent to interact with the environment to accomplish the task.
https://github.com/cyr0313/RoboGPT-/assets/56755367/6aca1736-4d2a-4b10-b2ac-b53e562e2752

Prompter/FILM may misjudge the task type, parent goal, and target object when planning a task, potentially disregarding valuable information. For instance, in the instruction `put the apple from the fridge on the table', Prompter may overlook the crucial detail that the apple is located inside the fridge. Furthermore, Prompter utilizes a predefined template, which is limited to specific types of tasks. LLM-Planner employs ChatGPT as its planner, which can be confused in logic, miss some actions, ignore robot's constraints, etc.. In contrast to RoboGPT, LLM-Planner is less intelligent, when instructed to clean three apples and put them on the table, LLM-Planner cleans each apple separately, but RoboGPT cleans them together. RoboGPT demonstrates a high level of cognitive ability, as it is capable of comprehending prefix content, discerning object amounts, understanding object dependencies, and making long-term decisions. Here we show some mistake cases of these methods. 
![imgae](mistake/GT_mistake.png)
![imgae](mistake/FILM_mistake.png)
![imgae](mistake/LLM_mistake.png)


