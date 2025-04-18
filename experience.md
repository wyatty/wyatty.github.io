---
layout: default
title: "Work Highlights For Wyatt Makedonski"
---

Menu
* [Main](https://makedon.ski/)
* [Research](https://makedon.ski/research)
* [Writings](https://makedon.ski/writings)
* [Work Highlights](https://makedon.ski/experience)
* [Contact](https://makedon.ski/contact)

---

# Work Highlights For Wyatt Makedonski

## [Gradient Energy](https://www.gradient.energy/)
**Co-Founder & CEO**, Late 2022-Present

Gradient Energy optimizes electric vehicle charging using AI.

## Explained
We use AI to control electric vehicle charging (EV) to optimize for maximum savings on electricity costs. We can save as much as $700 per year on charging for a single EV (there are many variables in this calculation, it depends on what baseline is used, and this number is focused on residential consumers and not commercial & industrial consumers). Further, we enable EV owners to earn as much as $1,000 per year in addition to the savings. EV owners are able to earn money by contributing to the stability of the grid when it is under stress. We aggregate many EVs together into a [Virtual Power Plant (VPP)](https://www.gradient.energy/virtual-power-plants) and participate in Demand Response programs. Demand response (DR) programs are built to alleviate stress on the grid; they are meant to reduce power consumption on the *demand* side of the grid in *response* to supply constraints. DR programs pay owners to avoid consuming power during times when the grid is under stress and prices are at their peak. DR programs pay a premium for avoided power consumption. Our software is carefully designed and tested for a streamlined and seamless user experience.

### Impact
By saving owners a large portion on EV charging and allowing them to earn from VPP participation, we put more money in their pockets. This lowers the total cost of ownership of EVs. This makes EVs even more competitive with traditional gas and diesel consuming (ICE) vehicles. From the grid perspective, we provide a means for electric utilities and grid operators to manage EV power consumption at scale. This, along with other benefits, reduces the barriers from utilities and grid operators have from the significantly increased volatile load from EVs. All of this **accelerates the transition to electric vehicles**. What else can happen with this? What are other implications and opportunities? There’s a lot more, [ask me](https://makedon.ski/contact).

### Market
The Edison Electric Institute estimates that there will be [26 million EVs on the road in the US by 2030](https://www.eei.org/-/media/Project/EEI/Documents/Issues-and-Policy/Electric-Transportation/EV-Forecast--Infrastructure-Report.pdf). Estimates for EVs in the entire world vary considerably. The economics of EVs are rapidly improving, including falling costs with batteries, engines, frames, and other components. In addition to this, EVs already have a lower cost of ownership for their lifetime than comparable ICE vehicles. There are heavy government incentives around the world, not just in the US, to electrify transportation. Further, we think that our services reducing the total cost of ownership of EVs can further accelerate the transition. With all of this, we are on a path to electrify most of the 200 million vehicles on the road in the US in the coming decades. Want more information? [Ask me](https://makedon.ski/contact).

### AI
We use some of the same technology used in ChatGPT (explained below). According to all published benchmarks, our charging optimization AI system is state of the art and the best performing system in the world, meaning that it is the single best system in the world at its task. In addition to this, our system is capable of modeling and optimizing more diverse environments and charging situations than others. Our AI models consider several variables in their optimization process including a diverse array of [distributed energy resources (DERs)](https://www.indermediate.com/i/136492740/distributed-energy), including multiple EVs, stationary batteries, solar panels (PV), and EV charger constraints. Beyond this, we are able to model human behavior and adapt our models to learn it and optimize savings while incorporating human behavior, in addition to the various DERs. We usually optimize the cost according to some rate structure, including tiered, TOU (time-of-use), and C&I rate structures (demand charges, in KW, in addition to energy costs, in kWh). In certain circumstances for EV fleets, we can optimize for maximum availability of vehicles while trying to lower electricity costs as much as possible. Our AI systems are already the best in the world at their tasks, and we are continuing to improve them for increased savings, more diverse environments, more diverse scenarios, and more diverse human behavior.

When I say we use some of the same technology behind ChatGPT, I am obviously not referring to LLMs. I am referring to [deep reinforcement learning (RL)](https://rail.eecs.berkeley.edu/deeprlcourse/), specifically the use of [proximal policy optimization (PPO)](https://arxiv.org/abs/1707.06347). I try not to use buzzwords and marketing terms but I do have to sell the product, forgive me for I am aware of my sins. We have ran some experiments with the use of transformers (also like ChatGPT), but we do not use them ([LSTMs](https://dl.acm.org/doi/10.1162/neco.1997.9.8.1735) are not dead). When I say that we have surpassed the best published results in the field and have the state of the art system, we have searched for many benchmarks and have surpassed the most prominent one by [Cao et al.](https://arxiv.org/abs/2106.00854). We attempted to reproduce their work to get the best comparison, but we could not; we contacted them about this but they refused to cooperate. We have our own customized simulator to model environments (microgrids) and train RL agents in them. We are constantly improving this simulator to increase the capabilities of our agents.

I greatly benefited from my time at [Yize NRG](#yize-nrg). Many of the challenges in ML I faced there I now face here, but with much more experience and knowledge. At the core, the product I worked on then and now are very similar.

Here are some of the technical challenges I have and am tackling in deep RL at Gradient (I may write about them in the future):
* Debugging RL agent training (if you know, you know)
* Stabilizing agent behavior with a time-dynamic reward function
* Enforcing safety constraints on agent behavior
* Helping the agent learn human behavior reliably and without overfitting
* Incorporating human preferences into the agent’s actions
* Training a multi task RL agent
* Training a generalist agent from offline RL
* Curriculum learning
* Meta reinforcement learning
* Monitoring agents in production
* [Ask me](https://makedon.ski/contact)

### Integrations Engine
Gradient needs integrations to many DERs of various types and manufacturers, we have created our own standalone software system to handle all of this complexity for our other software systems. This system provides integrations to EVs (with more than 50 models supported), chargers, stationary batteries, and PV inverters. We already host our own custom-built OCPP server which means we have control over most EV chargers.

### Virtual Power Plants
Gradient owns software to operate and control DERs in virtual power plants. This software includes some AI-powered components for necessary functions of the VPP. Why is AI needed in a VPP? [Ask me](https://makedon.ski/contact).

### V2G Virtual Power Plants
Before focusing entirely on charging optimization, we worked on building V2G (vehicle-to-grid) virtual power plants for nearly a year. “V2G” is the pseudo buzzword term for when electric vehicles discharge power back into the grid. A V2G VPP is just an aggregation of EVs producing power together at certain times. It seems benign, right? Well, when used correctly, a single EV can generate as much as $3,000 per year if it is V2G compatible and has a bidirectional charger (as stated before, there are a lot of variables in this calculation). The microeconomics of V2G are enticing but the macroeconomics, the impact V2G can have at scale, are more interesting. We paused work on this avenue for a simple reason, there are not enough V2G chargers at this time. We were mostly aware of this but certain manufacturers *misrepresented* the state of their products and their sales. When we learned of this misrepresentation and had more knowledge, we paused work on this avenue.

Since we worked on V2G VPPs for a while, we put a lot of effort and research into them. Efficiently and reliably operating a V2G VPP is more challenging than one may think. I have found very little information and publications out there about them despite the fact that they have many unique needs and challenges, the impact they can have, and the fact that their presence will rapidly grow. I have written about them, and intend to eventually publish the paper. In this paper, I discuss V2G VPPs, and call them [Dynamic Optimizing Virtual Power Plants (DOVPPs)](https://makedon.ski/research) (pronounced “dah-vips”; sometimes, to make an acronym shorter, you have to make it longer).

![GE logo ](https://github.com/wyatty/wyatty.github.io/raw/main/assets/GE_logo.png "Gradient Energy logo")

## Yize NRG
**Founder & Data Scientist**, 2017-2019

Yize NRG ("wise energy") used AI to optimize the operations of HVAC (heating and cooling) systems for buildings for big savings and flexibility.

### Explained
Using AI to optimize the operating cost of large buildings is very promising, as shown by [Google DeepMind’s optimization of Google’s data centers](https://deepmind.google/discover/blog/deepmind-ai-reduces-google-data-centre-cooling-bill-by-40/). We initially targeted large office buildings (e.g. high rises in Manhattan). In target buildings, the HVAC system would consume 50-70% of all energy consumed in the building. We could save 15% all the way up to 50% on HVAC energy usage (there are many variables in this calculation, the high end is for environments with a high degree of flexibility).

### Impact
Optimizing HVAC systems seems pretty boring and esoteric. Are you wondering about the implications and impacts of it? [Contact me, they're more than you think](https://makedon.ski/contact).

### AI
At Yize NRG, for the optimization of HVAC systems, we used deep RL. I experimented with a wide variety of RL algorithms, configurations, and neural network architectures. Based on all published results, our AI system was state of the art, meaning it was the best in the world at its task when compared to other systems using standard benchmarks in 2019. Beyond these narrow benchmarks, we expanded the agent’s capabilities in our custom simulator. We forked the highest quality HVAC simulator available and improved on it to allow the agent to learn and handle more diverse situations and optimization objectives.

Here are some of the technical challenges I faced in deep RL at Yize NRG:
* Debugging RL agent training (it’s an eternal problem in the field)
* Stabilizing agent behavior with a time-dynamic reward function
* Enforcing two sets of constraints on agent behavior to ensure safety
* Ensuring high reliability and stability operating in critical systems
* Incorporating human action signals into agent behavior predictably and reliably
* Bridging the sim-to-real gap
* Monitoring agents in production
* [Ask me](https://makedon.ski/contact)

As you can see, there is much overlap with my current work at [Gradient Energy](#gradient-energy). Luckily for me, the field has progressed significantly since 2019 so a lot of these challenges have become much easier.

### Short Term Load Forecasting
Before working on the HVAC optimization product, we worked on a product for short term load forecasting (STLF) for electric utilities for more than a year. We partnered with several electric utilities to get their data to train our models on. Our performance exceeded the baselines set by other common STLF methods for the dataset for each utility. We did not find a standard benchmark to compare our methods against, so we cannot make specific claims, just that they surpassed common methods on our datasets. We paused work on this product for several business reasons and shifted focus to the HVAC product.

![Yize NRG logo ](https://github.com/wyatty/wyatty.github.io/raw/main/assets/YizeNRG_logo.png "Yize NRG logo")

## HiroFit
**Lead Data Scientist**, Early 2021-Late 2022

HiroFit turned your phone into your own personal fitness trainer using AI.

### Explained
Personal fitness trainers are very expensive and can cost more than $100 an hour. As much as 90% of the time of your time in session with a personal trainer is not spent on instruction, it is merely monitoring form and performing rote tasks like counting reps. Our product was a mobile app that utilized the user’s phone camera to watch the user while they work out. This computer vision system (ML) would count reps of the exercise, automatically create an exercise journal or log, and, most importantly, coach the user as they exercise, including correcting form and pacing. In its log, it would track exercises, sets, reps, weights, and would track and analyze the user’s exercise correctness over time.

### Impact
Our goal was to help the user with their fitness goals while saving them money on expensive personal fitness trainers. We knew that we would not completely replace a personal trainer or athletic coach, but make those sessions with trainers more effective and productive. On a broader note, modern AI (as of 2023), for most tasks, is not in a state to automate and replace humans, but it is better suited to augment humans and make them more productive. Like challenges in robotics, there is a “long tail” (referring to the tail end of a distribution) of tasks and corner cases that a system must be able to do before it can replace a human. Further, a phone is limited to its point of view whereas a personal trainer can freely roam and gain multiple points of view of the same user. There is the obvious physical aspect of touch and aid that personal trainers provide. We did not aim to replace a trainer, but to require less of their time. We could reduce much of the rote work the trainers did and have them focus on specific learning moments. For our users, this meant spending less time with personal trainers and athletic coaches and therefore less money. For users that elected to still see trainers and coaches, we provided those teachers summaries and statistics about the user’s workouts so that they could tailor their instruction to the user’s specific needs.

My opinion:
```
On a broader note, modern AI (as of 2024), for most tasks, is not in a state to automate and replace humans, but it is better suited to augment humans and make them more productive.
```

### AI
For more specific aspects of the AI work, here are some of the technical challenges I faced while working at HiroFit:
* Experimented with transferring pretrained vision models
* Experimented with different learning approaches: having one model learn everything vs a two-stage system
* Experimented with model explainability (we needed to tell users what they did wrong)
* Tuning the neural network size and architecture to enable high throughput (frames per second)
* Tuning neural network size to fit in the memory of a mobile GPU
* *NOTE*: No, we did not use a [ViT](https://arxiv.org/abs/2010.11929)-descended model, CNNs are still quite useful
* Curious about some of the details and how I got strong explainability? [Ask me](https://makedon.ski/contact)

![HiroFit Model Example](https://github.com/wyatty/wyatty.github.io/raw/main/assets/hirofit_model.jpg "HiroFit model example")

## IEEE GlobalSpec
**Software Engineer in Machine Learning**, Left 2020, Albany, New York

### Auto Parts Classification
I led a team that built a machine learning (AI) system to automate and accelerate the ingestion of content into the company’s catalog, a critical function for the company.

#### Explained
IEEE GlobalSpec’s main product can be thought of as a large parts database or catalog, with most of their products being electrical and mechanical parts. A large audience of GlobalSpec were electrical engineers and mechanical engineers around the world. They could come to the website, get parts information, order parts, and other related tasks. With this, adding parts to the catalog for the website directly led to more traffic and more revenue. The critical bottleneck of the process was classifying parts (with just attributes of the parts) to the proper section of the internal taxonomy. This classification was critical as it impacted indexing on the internal search engine, discoverability on the website, and discoverability on Google. Adding parts to the catalog, with this classification bottleneck, was a manual and error-prone process. It involved having trained engineers review spreadsheets of parts with dozens of columns of part attributes. As this is tedious, it had a high error rate. Further, since this process would involve a team of six different engineers, there would be inconsistency in classification across humans. Ingesting parts from a single vendor could take as long as two full business weeks and involve as many as six engineers reviewing them at once. Improving this process to accelerate it, increase accuracy, and increase consistency was a top priority for the company.

#### Impact
We exceeded all expectations that business leadership had for this internal product. We achieved superhuman results on both accuracy and consistency of the classifications of our AI model. We reduced processing time for the largest part updates from 300+ man hours to minutes. The speedup depended on how much we wanted to parallelize the process. We could reduce it from minutes to seconds, but spending engineering effort or on-premise compute was not a large business priority.

#### AI
We achieved superhuman results with an [F1 score](https://www.v7labs.com/blog/f1-score-guide) of 0.95, and an average accuracy of more than 96%. We used the F1 score internally as our primary metric, but largely communicated the average accuracy externally as that’s more intuitive. Qualitatively, the clients were very pleased with the performance and consistency. I led a team of software engineers; I contributed technically (including to the system architecture, ML model architecture, data pipelines, and model infrastructure), made product decisions, and represented the product to stakeholders and clients.

For more specific aspects of the AI work, here are some of the technical challenges I faced working on the APC system:
* Experimented with model architecture (including various experiments with embeddings)
* Modeled data that had an inherent hierarchical structure
* Managed imbalance classification (experimented with class weighting, oversampling, and data augmentation)
* Monitoring distribution drift in production (input data was inherently bursty with different distributions in each burst)
* Optimizing for inference on CPUs (internal cloud did not support GPUs)
* Experimented with model compression (for faster throughput and smaller footprints)
* Scaled up and optimized data pipelines to increase data throughput

### More
I also built, as part of a small team, a business intelligence system for the company built on the [Elastic stack](https://www.elastic.co/elastic-stack). It achieved very high user satisfaction metrics while providing high throughput and reliability. For it, I built data pipelines ingesting diverse logs, cleaning and extracting information, and then enriching the data from external sources that I built integrations for. I tuned and debugged Elastic’s out-of-the-box anomaly detection ML models. As usual, I did all the necessary software engineering support work with that product (that has been assumed with everything I have in Work Highlights).

Besides those two products, I contributed bug fixes, features, and A/B tests to various production systems using SQL, Java, and Kotlin. Interestingly, the company used the ancient framework ColdFusion.

![IEEE GlobalSpec Logo](https://github.com/wyatty/wyatty.github.io/raw/main/assets/ieee_globalspec_logo.jpg "IEEE GlobalSpec logo")

## Cisco Systems
**Software Engineer Intern**, 2015, San Jose, California

We created an internal financial management and tracking application managing over $160M and 1,300 people annually. It was a web app using the MEAN stack (MySQL, Express, Angular.js, Node.js).

## Johnson & Johnson
**Software Engineer Co-op (DevOps)**, 2015, New Jersey

Worked on AWS cloud management/policing software for internal clients; Wrote APIs for streamlined control.

## John Deere
**Software Engineer Intern**, Summer 2014 & Summer 2013, Iowa

I created a warranty data system that connected warranty claims with specific production segments, departments, and locations in their tractor factories. Within months of release, it was being used in multiple factories located around the world. The software used Excel as the primary UI, streamed analytics to SAS, and integrated with the enterprise SAP database.

![pretty picture 2](https://github.com/wyatty/wyatty.github.io/raw/main/assets/green_city_colorful_trains.png "Pretty Picture 2")

---

# Technical Skills
Machine Learning (AI)
* Deep learning (various architectures and purposes): 2017-Present
* Deep reinforcement learning (RL): 2019-Present
* Natural language processing (NLP): 2018-Present
* Computer vision (CV): 2021-2022
* Large language models (LLMs): 2023-Present

Machine Learning Technologies
* TensorFlow (and Keras): 2017-2022
* PyTorch: 2022-Present
* RLlib (Ray): 2022-Present
* Stable-baselines: 2019-Present
* scikit-learn
* numpy
* pandas

Programming languages
* Python (strong)
* Go (prior experience)
* Swift (prior experience)
* Java (prior experience)
* C++ (prior experience)

Software Technologies
* Linux (Ubuntu)
* Amazon Web Services (AWS)
* Google Cloud (GCP)
* Git
* MySQL
* Django
* Jupyter notebooks
* MongoDB
* Airflow