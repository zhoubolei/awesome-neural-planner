 # Papers on neural motion planner and controller

## Autonomous Driving

arXiv: **A Survey of End-to-End Driving:Architectures and Training Methods**. [paper](https://arxiv.org/pdf/2003.06404.pdf) <br>
*comment*: a recent survey on end-to-end driving pipeline, compared to conventional modular pipeline.

ECCV20: **Perceive, Predict, and Plan: Safe Motion Planning Through Interpretable Semantic Representations**. [paper](http://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123680409.pdf) <br>
*comment*: A follow-up for the CVPR19 work below, a semantic occupancy representation is introduced between perception and motion planning. Cost function incorporates comfort driving.

CVPR19: **End-to-end Interpretable Neural Motion Planner**. [paper](https://1fykyq3mdn5r21tpna3wkdyi-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/End-to-end-Interpretable-Neural-Motion-Planner.pdf) <br>
*comment*: Like inverseRL, a cost function is learned from human demonstration when input LiDAR and roadmap, output perception detection result (bounding boxes) as well as cost volume. Then learned cost function is used to select the sampled candidate trajectories. Pay attention to its trajectory parameterization and the trajectory sampler for plausible trajectories. Planning horization is of 3 seconds. Interpretability cames from the joint output of 3D LiDAR detection result. 

coRL20sub: **Super-Human Performance in Gran Turismo Sport Using Deep Reinforcement Learning**. [paper](https://arxiv.org/pdf/2008.07971.pdf) [video!](https://www.youtube.com/watch?v=Zeyv1bN9v4A&feature=youtu.be) <br>
*comment*: pure deep RL approach for car-racing. Pay attention to its reward design and policy input and output. the side-by-side comparison between human expert and RL algorithm is interesting. The system architecture is also interesting, by using 4 PlayState 4 game consoles and a single desktop PC through ethernet connection. 

## Indoor navigation

coRL19: **Combining Optimal Control and Learning for Visual Navigation in Novel Environments**. [paper](http://proceedings.mlr.press/v100/bansal20a/bansal20a.pdf) [page](https://vtolani95.github.io/WayPtNav/) <br>
*comment*: learning-based perception + model-based control. waypoints are output from the perception, then fed into the model-based planner to generate smoonth feasible trajectory. strong assumption that map is known and odometry is perfect and environment is static

## Mobile manipulation

coRL20sub: **ReLMoGen: Leveraging Motion Generation in Reinforcement Learning for Mobile Manipulation**. [paper](https://arxiv.org/pdf/2008.07792.pdf) [page](http://svl.stanford.edu/projects/relmogen/) <br>
*comment*: a hybrid system integrating traditional motion planner and RL learning. Rapidly-exploring random tree (RRT) and probabilistic raod-maps (PRM) have been adopted in the motion planner. RL policy output a subgoal (desired 2D loction/end-effector 3D location). The policy has different parameterization. Experimental platform [iGibson](http://svl.stanford.edu/igibson/)

## Robot manipulation

## Algorithms

IROS20: **Learning High-Level Policies for Model Predictive Control**. [paper](http://rpg.ifi.uzh.ch/docs/IROS20_Yunlong.pdf) [code](https://github.com/uzh-rpg/high_mpc) <br>
*comment*: loop high-level policy learning into MPC

## Relevant Researchers

[Davide Scaramuzza](http://rpg.ifi.uzh.ch/research_learning.html): ETH badass researcher. 

[Silvio Savarese](http://cvgl.stanford.edu/silvio/): Stanford faculty, focusing on indoor navigation

[Raquel Urtasun](http://www.cs.toronto.edu/~urtasun/): Utoronto, Uber ATG toronto head, autonomous driving leading researcher.

[Saurabh Gupta](http://saurabhg.web.illinois.edu/): UIUC, vision+navigation.
