# Wyatt Makedonski

## Mission
I have committed my life to improving the world. This is not a light commitment or something I am saying to virtue signal. I mean it. I am doing this through my work in the energy field as that field is the single most important field in the battle against climate change (likely the biggest challenge facing humanity). I have founded multiple companies in energy (including my current company), have written multiple research papers to progress the field, and create educational content to attract more people to the field.

## Introduction
I have been working in energy since 2016. I have been working in AI (specifically machine learning) since 2017. Working in energy led me to my work in AI as the technology is capable of solving many problems and creating a lot of value in the world. I apply AI to the energy field.

### AI
I have built two state of the art machine learning systems (meaning that they are the single best performing system in the world at their task) at both Gradient Energy and Yize NRG (both using deep reinforcement learning). I have built another production machine learning system with superhuman performance on its task (natural language processing) while at IEEE GlobalSpec. I have built another high-performing production machine learning system (computer vision) at HiroFit; there were no published benchmarks for state of the art or human performance (the task was not suited to be compared one-to-one to human performance) so I cannot make a claim that it exceeded their performance, but it was a pioneering system in the field with subjectively higher performance and more features than other systems, and, most importantly, it made our users very happy.

### I’ll Be Honest
I am not known for my lack of weakness, I have many weaknesses. I have a narrow set of strengths and skills that I try to apply to create value. I try my best to be aware of my gaps and avoid commenting and acting on matters in those areas; I prefer to defer to someone better at those areas. Even in areas where I am relatively strong, I still have much to learn and improve.

![pretty picture 0](https://github.com/wyatty/wyatty.github.io/raw/main/assets/pretty_nn_controlling_grid_0.png "Pretty Picture 0")

## Work Highlights

### [Gradient Energy](https://www.gradient.energy/)
**Co-Founder**, Late 2022-Present

Gradient Energy optimizes electric vehicle charging using AI.

#### Explained
We use AI to control electric vehicle charging (EV) to optimize for maximum savings on electricity costs. We can save as much as $700 per year on charging for a single EV (there are many variables in this calculation, it depends on what baseline is used, and this number is focused on residential consumers and not commercial & industrial consumers). Further, we enable EV owners to earn as much as $1,000 per year in addition to the savings. EV owners are able to earn money by contributing to the stability of the grid when it is under stress. We aggregate many EVs together into a [Virtual Power Plant (VPP)](https://www.gradient.energy/virtual-power-plants) and participate in Demand Response programs. Demand response (DR) programs are built to alleviate stress on the grid; they are meant to reduce power consumption on the *demand* side of the grid in *response* to supply constraints. Demand Response programs pay owners to avoid consuming power during times when the grid is under stress and prices are at their peak. Demand Response programs pay a premium for avoided power consumption.

#### Impact
By saving owners a large portion on EV charging and allowing them to earn from VPP participation, we put more money in their pockets. This lowers the total cost of ownership of EVs. This makes EVs even more competitive with traditional gas and diesel consuming (ICE) vehicles. From the grid perspective, we provide a means for electric utilities and grid operators to manage EV power consumption at scale. This, along with other benefits, reduces the barriers from utilities and grid operators have from the significantly increased volatile load from EVs. All of this **accelerates the transition to electric vehicles**. What else can happen with this? What are other implications and opportunities? There’s a lot more, [ask me](#contact).

#### Market
The Edison Electric Institute estimates that there will be [26 million EVs on the road in the US by 2030](https://www.eei.org/-/media/Project/EEI/Documents/Issues-and-Policy/Electric-Transportation/EV-Forecast--Infrastructure-Report.pdf). Estimates for EVs in the entire world vary considerably. The economics of EVs are rapidly improving, including falling costs with batteries, engines, frames, and other components. In addition to this, EVs already have a lower cost of ownership for their lifetime than comparable ICE vehicles. There are heavy government incentives around the world, not just in the US, to electrify transportation. Further, we think that our services reducing the total cost of ownership of EVs can further accelerate the transition. With all of this, we are on a path to electrify most of the 200 million vehicles on the road in the US in the coming decades. Want more information? [Ask me](#contact).

#### AI
We use some of the same technology used in ChatGPT (explained below). According to all published benchmarks, our charging optimization AI system is state of the art and the best performing system in the world, meaning that it is the single best system in the world at its task. In addition to this, our system is capable of modeling and optimizing more diverse environments and charging situations than others. Our AI models consider several variables in its optimization process including a diverse array of distributed energy resources (DERs), including multiple EVs, stationary batteries, solar panels (PV), and EV charger constraints. Beyond this, we are able to model human behavior and adapt our models to learn it and optimize savings while incorporating human behavior, in addition to the various DERs. We usually optimize the cost according to some rate structure, including tiered, TOU (time-of-use), and C&I rate structures (demand charges, in KW, in addition to energy costs, in kWh). In certain circumstances for EV fleets, we can optimize for maximum availability of vehicles while trying to lower electricity costs as much as possible. Our AI systems are already the best in the world at their tasks, and we are continuing to improve them for increased savings, more diverse environments, more diverse scenarios, and more diverse human behavior.

When I say we use some of the same technology behind ChatGPT, I am obviously not referring to LLMs. I am referring to [deep reinforcement learning (RL)](https://rail.eecs.berkeley.edu/deeprlcourse/), specifically the use of proximal policy optimization (PPO). I try not to use buzzwords and marketing terms but I do have to sell the product, forgive me for I am aware of my sins. We have ran some experiments with the use of transformers (also like ChatGPT), but we do not use them ([LSTMs](https://dl.acm.org/doi/10.1162/neco.1997.9.8.1735) are not dead). When I say that we have surpassed the best published results in the field and have the state of the art system, we have searched for many benchmarks and have surpassed the most prominent one by [Cao et al.](https://arxiv.org/abs/2106.00854). We attempted to reproduce their work to get the best comparison, but we could not; we contacted them about this but they refused to cooperate. We have our own customized simulator to model environments (microgrids) and train RL agents in them. We are constantly improving this simulator to increase the capabilities of our agents.

Here are some of the technical challenges I have and am tackling in deep RL at Gradient (I may write about them in the future):
* Debugging RL agent training (if you know, you know)
* Stabilizing agent behavior with a time-dynamic reward function
* Enforcing safety constraints on agent behavior
* Helping the agent learn human behavior reliably and without overfitting
* Incorporating human preferences into the agent’s actions
* Training a multi task RL agent
* Training a generalist agent from offline RL
* Monitoring agents in production
* [Ask me](#contact)

#### Integrations Engine
X 

#### Virtual Power Plants
X 

#### V2G Virtual Power Plants
X

![GE logo ](https://github.com/wyatty/wyatty.github.io/raw/main/assets/GE_logo.png "Gradient Energy logo")

### Yize NRG
**Founder**, 2017-2019

Yize NRG ("wise energy") used AI to optimize the operations of HVAC (heating and cooling) systems for buildings for big savings and grid flexibility.

#### Explained
X

#### Impact
Optimizing HVAC systems seems pretty boring and esoteric. Are you wondering about the implications and impacts of it? [Contact me, they're more than you think](#contact).

#### AI
X

#### Short Term Load Forecasting
X

![Yize NRG logo ](https://github.com/wyatty/wyatty.github.io/raw/main/assets/YizeNRG_logo.png "Yize NRG logo")

### HiroFit
**Co-Founder**, Early 2022-Late 2022

#### Explained
X

#### Impact
X

#### AI
X

#### More
X

### IEEE GlobalSpec
**Software Engineer**, Left 2020, Albany, New York

#### Auto Parts Classification
I led a team that built a machine learning (AI) system to automate and accelerate the ingestion of content onto the company’s catalog.

#### Explained
X

#### Impact
X

#### AI
X

#### More
X

### Cisco Systems
**Software Engineer Intern**, 2015, San Jose, California

We created an internal financial management and tracking application managing over $160M, 1,300 people annually. It was a web app using the MEAN stack (MySQL, Express, Angular.js, Node.js).

### John Deere
**Software Engineer Intern**, Summer 2014 & Summer 2013, Iowa

I created a warranty data system that connected warranty claims with specific production segments, departments, and locations in their tractor factories. Within months of release, it was being used in multiple factories located around the world. The software used Excel as the primary UI, streamed analytics to SAS, and integrated with the enterprise SAP database.

## Research and Publications
I try to advance the world by releasing knowledge completely open source in addition to my work. I enjoy research, learning, and sharing knowledge, but I do appropriately budget my time. Two papers are already written and are under review, one is a draft that is mostly complete, and the last is an active draft. I contribute to this when I have free time as my work is my focus.

### Energy: Electricity Grid Architecture
X

### Energy: Virtual Power Plants
X

### Economics
X

### Educational Materials
I write and present, among other things, to teach people about the energy field to try and bring them into the field. I have contributed to publications on behalf of and presented to groups within the energy industry group [DER Task Force](https://www.dertaskforce.com/), and contribute to the educational group [inDERmediate](https://www.indermediate.com/).

Highlighted publications:
* For an introduction to energy and the grid, check out our [Grid Overview](https://www.indermediate.com/p/indermediate-the-grid-overview)

## Education
### Rensselaer Polytechnic Institute (RPI)
B.S. Computer Science 2013-2017

Troy, New York

### Cedar Falls High School
Cedar Falls, Iowa 2010–2013

## Technical Skills
Machine Learning (AI)
* Deep learning (various architectures and purposes): 2017-Present
* Deep reinforcement learning (RL): 2019-Present
* Natural language processing (NLP): 2018-2020
* Computer vision (CV): 2021-2022

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
* Swift (prior experience)
* Go (prior experience)
* Kotlin (prior experience)

Software Technologies
* Linux (Ubuntu)
* Amazon Web Services (AWS)
* Git
* MySQL
* Django
* Jupyter notebooks
* MongoDB
* Airflow

## Miscellaneous
### Theta Xi Fraternity (aka “Zoo”)
Brother, Alpha chapter. Initiated in 2014.

### Favorite Books
* “Meditations” by Marcus Aurelius
* “Zero to One” by Peter Thiel
* “Daily Stoic” by Ryan Holiday
* “Factfulness” by Hans Rosling
* “Extreme Ownership” by Jocko Willink and Leif Babin
* “Strong Towns” by Chuck Marohn
* “Grit” by Angela Duckworth
* “Peak” by Anders Ericsson

### Other
I’ve lived in over a dozen cities across several states. New York, New York has been my favorite.

## Contact
Email: wyatt at gradient dot energy

[Twitter](https://twitter.com/wyatt_yy)

[GitHub](https://github.com/wyatty)

[LinkedIn](http://www.linkedin.com/in/wyattmakedonski)
