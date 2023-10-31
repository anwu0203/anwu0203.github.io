# Andy Wu's Portfolio

___

### Farming Robotics Challenge (_February 2023 – June 2023_)

**Overview:** I participated in this robotics challenge hosted by Farm_ng geared toward smart farms. The goal was to innovate and enhance the Amiga farming robot given by Farm_ng to aid smaller farmers. My team decided to create a multipurpose data mule package capable of traveling to on-field sensors, collecting data, and charging each sensor.

To charge each sensor, we utilized Li-Fi laser charging technology which required the robot to align an onboard charging laser with the receptors on the sensors. I designed and implemented a computer vision-based alignment system in Python for an onboard Raspberry Pi, enabling the Amiga to recognize predesignated AprilTags on sensors and precisely position itself with the receptors. Next, we retrieved data from the sensors via Bluetooth connections between the on-board Raspberry Pi and on-field Raspberry Pi sensors, sending the data to the central computer of the Amiga using Ethernet. On the central computer, I created a GUI using Python and Kivy to organize and visualize the retrieved data. Additionally, I developed a separate application for displaying video and providing statistical information on the computer vision alignment system. Finally, we implemented a human and object detector using the frontal camera for safety purposes.

![Amiga Example](/assets/img/gort_movements.png)

**Improvements:** Although the alignment system works with good precision, I believe that implementing a mechanical linear motion system on the Amiga for the laser can greatly improve precision and energy efficiency.

**Technical Skills:** Building computer vision models, GUI development, data processing, robotics

**Tools:** Python, Kivy, Raspberry Pi, AprilTag, Li-Fi, Bluetooth, Ethernet

**Team:** Jesus Oviedo, Alejandro Rojas Rodriguez, Aashay Parab

[![View Demo Video](https://img.shields.io/badge/Google_Drive-View_Demo_Video-blue?logo=googledrive&logoColor=white)](https://drive.google.com/file/d/1W0euaoswMJ67xfmDPM8Pi-swa-j3bRrP/view?usp=sharing) [![View Report](https://img.shields.io/badge/PDF-View_Report-blue?logo=googledocs&logoColor=white)](/assets/files/robotics_final_report.pdf) 

___

### Capstone: Blockchain Rug-Pull Token Detector (_September 2022 – March 2023_)

**Overview:** As part of the UCSB Capstone program, my group and I partnered with Forta Network, a blockchain security company, to research and develop a comprehensive detector bot designed to uncover malicious rug-pull smart contracts on the Ethereum network.

After researching hundreds of known malicious smart contracts, we identified several recurring rug-pull tactics, including hidden mint functions, token burn functions, and self-destruct functions. To build the detector, we utilized the Etherscan API to obtain contract source code and broke down the code using Abstract Syntax Trees (AST) to analyze each individual function. The detector achieved a 91.8% recall rate on known rug-pull contracts during local testing. The detector bot was deployed on the Forta Network public page to allow users to check for potential common rug-pull functions in their contracts.

![Detector stats](/assets/img/detector_stats.png)

**Improvements:** This detector bot can only detect some rug-pull contracts with the heuristics we have covered. Therefore, future steps could be to add more detector functions to cover more malicious functions. Additionally, the use of machine learning with our detector results as inputs could improve the precision of our alerts.

**Technical Skills:** AST analysis, Solidity, Web3

**Tools:** Python, Etherscan API

**Team:** Nicholas Brown, John Lin, Khalid Mihlar, Alejandro Rojas Rodriguez

[![View Slides](https://img.shields.io/badge/PPT-Open_Slides-blue?logo=microsoftpowerpoint&logoColor=white)](assets/files/fortaknight_ppt.pptx)

___

### Early Research Scholarship Program (_September 2021 – December 2021_)

**Overview:** As part of the Early Research Scholarship Program, my team was assigned to collaborate with Professor Eric Vigoda on researching the application of Markov Chain Monte Carlo (MCMC) methods to uncover gerrymandering within the state voting system. 

We researched and devised a project plan to utilize recombination MCMC in conjunction with score functions. The model can randomly generate non-partisan districting lines for electoral vote counting, allowing us to accumulate large amounts of data on potential non-partisan districting plans. Next, we can compare this generated data with actual districting plans to determine their partisanship, thus uncovering instances of gerrymandering. We planned to apply this model more generally to other U.S. states.

![MCMC](/assets/img/MCMC.png)

**Technical Skills:** Computational theory

**Tools:** Markov Chain Monte Carlo

**Team:** Nicholas Johnson

[![View Slides](https://img.shields.io/badge/PPT-Open_Slides-blue?logo=microsoftpowerpoint&logoColor=white)](assets/files/ERSP_presentation.pptx) [![View Report](https://img.shields.io/badge/PDF-View_Proposal-blue?logo=googledocs&logoColor=white)](assets/files/ERSP_proposal.pdf)

___

### 2048 Game AI (_November 2021 – December 2021_)

**Overview:** As part of my Artificial Intelligence course, I was tasked to implement an AI using search algorithms to play the game 2048. The goal was to obtain the highest average tile reached over multiple runs.

I chose to implement the minimax search algorithm and conducted node predictions based on worst-case random tile placements. To accomplish this, I utilized a weighted tile matrix to evaluate the significance of each tile for the score function. To optimize runtime and allow deeper searches, I also integrated alpha-beta pruning.

The resulting average highest tile reached was 2150.

![2048 stats](/assets/img/2048_stats.png)

**Improvements:** More research and testing to fine-tune the weighted tile matrix could help optimize the score function.

**Technical Skills:** Minimax search algorithm

**Tools:** Python

[![View Files](https://img.shields.io/badge/GitHub-View_File-blue?logo=github&logoColor=white)](https://github.com/anwu0203/CS165_MP2/tree/main) [![View Report](https://img.shields.io/badge/PDF-View_Report-blue?logo=googledocs&logoColor=white)](/assets/files/2048_report.pdf)

___

### Mastermind Web Game (_January 2021_)

**Overview:** For a hackathon hosted by SB Hacks, my team decided to create a web-based game inspired by Mastermind. Our goals were to explore the process of web app development and gain proficiency in new programming languages.

Over a 36-hour period, I learned how to program in Java, HTML, and CSS for webpage development. We designed the overall website layout and connected the user interface with back-end game logic, resulting in a fully functional Mastermind game. We presented our web game during the hackathon.

![Website](/assets/img/mastermind.png)

**Improvements:** The webpage design could have been more complex given more experience in the languages. Furthermore, the website communicates through pop-up windows which could have been translated into an on-screen text box.

**Technical Skills:** Website development

**Tools:** Java, HTML, CSS

**Team:** Jesus Oviedo

[![View Files](https://img.shields.io/badge/GitHub-View_Files-blue?logo=github&logoColor=white)](https://github.com/jaoviedo/SBHacksProject2021) [![View Website](https://img.shields.io/badge/Link-View_Website-blue?logo=icloud&logoColor=white)](https://jaoviedo.github.io/SBHacksProject2021/)

