# Andy Wu's Portfolio

___

### Farming Robotics Challenge (_February 2023 – June 2023_)

**Overview:** I participated in this robotics challenge held by Farm_ng geared toward smart farms. The goal was to innovate upon and modify the Amiga farming robot given by Farm_ng to aid smaller farmers. My team decided to create a multipurpose data mule package that can travel to on-field sensors and both collect their data and charge each sensor.

In order to charge each sensor, we utilized Li-Fi laser charging technology which requires the robot to align an on-board charging laser with the receptors on the sensors. I designed and implemented a computer vision-based alignment system in Python for an on-board Raspberry Pi, allowing the Amiga to recognize predesignated AprilTags sensor and precisely position itself with the receptor. Next, we retrieved data from the sensors via Bluetooth connection between the on-board Raspberry Pi and on-field Raspberry Pi sensors, sending the data to the Amiga's central computer using Ethernet. On the central computer, I created a GUI using Python and Kivy to organize and graph the retrieved data as well as a separate application for displaying video and statistical information on the computer vision alignment system. Finally, we implemented a human and object detector using the frontal camera for safety purposes.

![Amiga Example](/assets/img/gort_movements.png)

**Improvements:** Although the alignment system works with good precision, I believe that implementing a mechanical linear motion system on the Amiga for the laser can greatly improve precision and energy efficiency.

**Technical Skills:** Building computer vision models, GUI development, data processing, robotics

**Tools:** Python, Kivy, Raspberry Pi, AprilTag, Li-Fi, Bluetooth, Ethernet

**Team:** Jesus Oviedo, Alejandro Rojas Rodriguez, Aashay Parab

[![View Demo Video](https://img.shields.io/badge/Google_Drive-View_Demo_Video-blue?logo=googledrive&logoColor=white)](https://drive.google.com/file/d/1W0euaoswMJ67xfmDPM8Pi-swa-j3bRrP/view?usp=sharing) [![View Report](https://img.shields.io/badge/PDF-View_Report-blue?logo=googledocs&logoColor=white)](/assets/files/robotics_final_report.pdf) 

___

### Capstone: Blockchain Rug-Pull Token Detector (_September 2022 – March 2023_)

**Overview:** As part of the UCSB Capstone program, my group and I partnered with Forta Network, a blockchain security company, to research and develop a comprehensive detector bot to uncover malicious, rug-pull smart contracts on the Ethereum network.

After researching hundreds of known malicious smart contracts, we identified several reoccurring rug-pull tactics including hidden mint functions, token burn functions, and self-destruct functions. To build the detector, we utilized the Etherscan API to obtain contract source code and broke down the code using Abstract Syntax Trees (AST) to analyze each individual function. The detector yielded a 91.8% recall rate on known rug-pull contracts during local testing. The detector bot was deployed on the Forta Network public page to allow users to check for potential common rug-pull functions in their contracts.

![Detector stats](/assets/img/detector_stats.png)

**Improvements:** This detector bot can only detect some rug-pull contracts with the heuristics we have covered. Therefore, future steps could be to add more detector functions to cover more malicious functions. Additionally, the use of machine learning with our detector results as inputs could improve the precision of our alerts.

**Technical Skills:** AST analysis, Solidity, Web3

**Tools:** Python, Etherscan API

**Team:** Nicholas Brown, John Lin, Khalid Mihlar, Alejandro Rojas Rodriguez

[![View Slides](https://img.shields.io/badge/PPT-Open_Slides-blue?logo=microsoftpowerpoint&logoColor=white)](assets/files/fortaknight_ppt.pptx)

___

### 2048 Game AI (_November 2021 – December 2021_)

**Overview:** As part of my Artificial Intelligence course, I was tasked to implement an AI using search algorithms to play the game 2048. The goal was to obtain the highest average tile reached over several runs.

I chose to implement the minimax search algorithm and ran node predictions based on the worst-case random tile placements. To achieve this, I employed a weighted tile matrix in order to evaluate the importance of each tile for the score function. To optimize runtime and allow deeper searches, I implemented alpha-beta pruning.

The resulting average highest tile reached was 2150.

![Detector Bot Stats](/assets/img/2048_stats.png)

**Improvements:** More research and testing to fine-tune the weighted tile matrix could help optimize the score function.

**Technical Skills:** Minimax search algorithm

**Tools:** Python

[![View Files](https://img.shields.io/badge/GitHub-View_File-blue?logo=github&logoColor=white)](https://github.com/anwu0203/CS165_MP2/tree/main) [![View Report](https://img.shields.io/badge/PDF-View_Report-blue?logo=googledocs&logoColor=white)](/assets/files/2048_report.pdf)

___

### Mastermind Web Game (_January 2021_)

**Overview:** For a hackathon hosted by SB Hacks, my team decided to create a Mastermind-type web game. The goal was to explore the process of web app development as well as learn new programming languages.

Over a 36-hour period, I learned how to program in Java, HTML, and CSS for webpage development. We designed the overall website layout and rigged the UI with back-end game logic to create a functioning Mastermind game. We presented the web game during the hackathon.

![Detector Bot Stats](/assets/img/mastermind.png)

**Improvements:** The webpage design could have been more complex given more experience in the languages. Furthermore, the website communicates through pop-up windows which could have been translated into an on-screen text box.

**Technical Skills:** Website development

**Tools:** Java, HTML, CSS

**Team:** Jesus Oviedo

[![View Files](https://img.shields.io/badge/GitHub-View_Files-blue?logo=github&logoColor=white)](https://github.com/jaoviedo/SBHacksProject2021) [![View Website](https://img.shields.io/badge/Link-View_Website-blue?logo=icloud&logoColor=white)](https://jaoviedo.github.io/SBHacksProject2021/)

___

### Early Research Scholarship Program (_September 2021 – December 2021_)

**Overview:** As part of the Early Research Scholarship Program, my team was assigned to work with Professor Eric Vigoda to research methods of utilizing Markov Chain Monte Carlo (MCMC) methods to uncover gerrymandering in the state voting system. 

My team researched and created a project plan to utilize recombination MCMC in combination with score functions. The model can then randomly generate non-partisan districting lines for electoral vote counting in order to accumulate large amounts of data on potential non-partisan districting plans. Next, we can compare the generated data with actual districting plans to determine the plan's partisanship, thus uncovering gerrymandering. We planned to utilize this model more generally to cover all states.

![Detector Bot Stats](/assets/img/gerrymandering.png)

**Technical Skills:** Computational theory

**Tools:** Markov Chain Monte Carlo

**Team:** Nicholas Johnson

[![View Slides](https://img.shields.io/badge/PPT-Open_Slides-blue?logo=microsoftpowerpoint&logoColor=white)](assets/files/ERSP_presentation.pptx) [![View Report](https://img.shields.io/badge/PDF-View_Proposal-blue?logo=googledocs&logoColor=white)](assets/files/ERSP_proposal.pdf)
