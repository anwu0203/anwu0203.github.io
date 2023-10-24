# Andy Wu's Portfolio

### Education
B.S. - Computer Science University of California, Santa Barbara (_June 2023_)

___

### Capstone: Blockchain Rug-Pull Token Detector (_September 2022 – March 2023_)

**Overview:** As part of the UCSB Capstone program, my group and I partnered with Forta Network, a blockchain security company, to research and develop a comprehensive detector bot to uncover malicious, rug-pull smart contracts on the Ethereum network.

After researching hundreds of known malicious smart contracts, we identified several reoccurring rug-pull tactics including hidden mint functions, token burn functions, and self-destruct functions. To build the detector, we utilized the Etherscan API to obtain contract source code and broke down the code using Abstract Syntax Trees (AST) to analyze each individual function. The detector yielded a 91.8% recall rate on known rug-pull contracts during local testing. The detector bot was deployed on the Forta Network public page to allow users to check for potential common rug-pull functions in their contracts.

![Detector stats](/assets/img/detector_stats.png)

**Improvements:** This detector bot can only detect some rug-pull contracts with the heuristics we have covered. Therefore, future steps could be to add more detector functions to cover more malicious functions. Additionally, the use of machine learning with our detector results as inputs could improve the precision of our alerts.

**Technical Skills:** AST analysis, Solidity, Web3

**Tools:** Python, Etherscan API

**Team:** Nicholas Brown, John Lin, Khalid Mihlar, Alejandro Rojas Rodriguez, Aashay Parab

___

### Farming Robotics Challenge (_February 2023 – June 2023_)

**Overview:** I participated in this robotics challenge held by Farm_ng geared toward smart farms. The goal was to innovate upon and modify the Amiga farming robot given by Farm_ng to aid smaller farmers. My team decided to create a multipurpose data mule package that can travel to on-field sensors and both collect their data and charge each sensor.

In order to charge each sensor, we utilized Li-Fi laser charging technology which requires the robot to align an on-board charging laser with the receptors on the sensors. I designed and implemented a computer vision-based alignment system in Python for an on-board Raspberry Pi, allowing the Amiga to recognize predesignated AprilTags sensor and precisely position itself with the receptor. Next, we retrieved data from the sensors via Bluetooth connection between the on-board Raspberry Pi and on-field Raspberry Pi sensors, sending the data to the Amiga's central computer using Ethernet. On the central computer, I created a GUI using Python and Kivy to organize and graph the retrieved data as well as a separate application for displaying video and statistical information on the computer vision alignment system. Finally, we implemented a human and object detector using the frontal camera for safety purposes.

![Amiga Example](/assets/img/gort_movements.png)

**Improvements:** Although the alignment system works with good precision, I believe that implementing a mechanical linear motion system on the Amiga for the laser can greatly improve precision and energy efficiency.

**Technical Skills:** Building computer vision models, GUI development, data processing, robotics

**Tools:** Python, Kivy, Raspberry Pi, AprilTag, Li-Fi, Bluetooth, Ethernet

**Team:** Jesus Oviedo, Alejandro Rojas Rodriguez

**Resources:** [Demo Video](https://drive.google.com/file/d/1W0euaoswMJ67xfmDPM8Pi-swa-j3bRrP/view?usp=sharing), [Final Report](/assets/files/robotics_final_report.pdf) 

___

### 2048 Game AI (_November 2021 – December 2021_)

**Overview:** As part of my Artificial Intelligence course, I was tasked to implement an AI using search algorithms to play the game 2048. The goal was to obtain the highest average tile reached over several runs.

I chose to implement the minimax search algorithm and ran node predictions based on the worst-case random tile placements. To achieve this, I employed a weighted tile matrix in order to evaluate the importance of each tile for the score function. To optimize runtime and allow deeper searches, I implemented alpha-beta pruning.

The resulting average highest tile reached was 2150.

![Detector Bot Stats](/assets/img/2048_stats.png)

**Improvements:** More research and testing to fine-tune the weighted tile matrix could help optimize the score function.

**Technical Skills:** Minimax search algorithm

**Tools:** Python

___

### Mastermind Web Game (_January 2021_)

**Overview:** 

![Detector Bot Stats](/assets/img/detector_stats.png)

**Improvements:** 

**Technical Skills:**

**Tools:** 

**Team:** 
- Led a team during a 36-hour hackathon to create a web game
- Developed a Mastermind-type game where the player has several attempts to guess a specific order of colors. Each guess will provide the accuracy of the guess, leading to more educated guesses
- Utilized HTML and CSS for front-end visuals and Java for back-end game logic

___

### Early Research Scholarship Program (_September 2021 – December 2021_)

**Overview:** 

![Detector Bot Stats](/assets/img/detector_stats.png)

**Improvements:** 

**Technical Skills:**

**Tools:** 

**Team:** 
- Focus: applying and implementing a Markov Chain Monte Carlo (MCMC) algorithm on electoral districting lines to uncover gerrymandering in U.S. state voting
- Generated non-partisan data utilizing the MCMC algorithm and compared the collected data with state voting results in order to determine the partisanship of state districting lines
