# How to Break Things on Purpose:
Computer Vision Applied to Strategic Competition and Dynamic Graphs.
In an industry that relies on exacting logic, the term 'disruptor' has a singular seductive quality. Like many technological tools, 'computer vision' or CV, has the potential for disruption on a massive scale. Widely used for medical imaging and autonomous vehicles, its limits of versatility have yet to be reached; one recent proposal uses computer vision to protect beach-goers from riptides and sharks, and can recognize and alert safety personnel to unattended children and struggling swimmers.

![image](https://github.com/JessemanGray/BREAK/assets/123507565/00afe4d0-0efa-44a9-8a85-8146fa7b1018)


Bruce the Shark from 'Jaws'  (Photo : Academy of Motion Picture Arts and Sciences)In ourcase, CV is being used for a somewhat less altruistic cause. The original intent was to develop a better understanding of the benefits and limitations of different CV architectures while also gaining  insight into highly dynamic models that can be difficult to interpolate. Game theory and adversarial constructs have proved to be useful in solving challenges related to NLP-based LLMs, and these principles could translate to CV as well. 
The impetus for this research wasn't completely random. Late one evening moonlighting at a local dive bar watching the sharks circle the pool table, it occurred to me that a game like this, specifically the cue sport "eight-ball" could be an interesting way to document patterns of entropy devolving from organized systems, as well as chart probabilities of success for a given approach. Tracking each ball's progression and feeding those vectors into a predictive model could help narrow down the most reliable outcome for each setup. As a bonus, segmentation should also shed light on other trends and inferences that might not be as obvious without modeling, as well as reinforcing learned and intuited relationships. 

![Magic8ball](https://github.com/JessemanGray/BREAK/assets/123507565/f25ec42c-c253-42c5-88f8-2999387527b0)
✨Magic 8 Ball ✨

Not entirely sure that the concept had legs, I decided that training the CV on the initial contact or 'break', would give  the most immediate payback in tghe form of raw data. It also represents the most interactive moment in play, since all objects except for the cue ball begin isolated within an organized boundary. For the preliminary modeling I established an initial sample of ten breaks as a baseline and used OpenCV in a Google Colab notebook to process them into individual frames. 
Code cell randomly shuffles frames, saves them to 'content' file, and destroys all windowsOne plus about using pool balls' unique properties to illustrate vectors is the ease by which they can be identified: by color and number and as solid or stripe. The polarity of the cue ball and eight ball also creates an inherent tension and bias that activates and informs the shape of the results. However, the speed and velocity unleashed by kinetic force create sudden and unpredictable movements that can be difficult to track. This downside is one area where these models could have a positive impact on the bigger picture of CV performance. Improving models' reaction time and ability to decipher small movements could have beneficial implications upstream in product development where thresholds are measured in micrometers, as well as in VR and augmented reality applications.
After annotating the initial batch of 300 frames with bounding boxes in LabelImg they were ready to be loaded into a YOLO model. LabelImg saves the image information in an .xml file, which must be converted to .txt to use in the object detection model. The annotation proved to be the longest, and most arduous part of the process by far.

A common phrase offered by experienced pool enthusiasts when giving advice is "Pool is just math". There are some parallels you can draw between pool and computational thinking, and while not perfect, there are some similarities. One of the most obvious is the mandate to break down a bigger problem into smaller ones. Maybe you can't sink all the balls at once, but it's possible to manipulate them sequentially to that effect. Likewise, vectors, differentials, and tangential geometry are useful in successfully mapping out placements in a 3-dimensional field, even though most of the interactions can be envisioned as taking place on a 2D plane with x and y axes.
Dr. Martin Luther King Jr. shooting pool in 1966. Courtesy Bettman/Getty ImagesA less obvious way in which the dynamics of pool relate to math, specifically computer math, is that they are physical implementations of graph diagrams at work. Even though a ball may appear to collide with multiple others simultaneously,  there is an order not immediately discernible to the naked eye. Each instance of contact acts as a logic gate, defining the scope of the next iteration. Following the precise progression by which energy is absorbed and distributed is only possible with the aid of enhanced instruments. The arrow of time follows the same rule as graphs in computer science- the direction from one node to the next cannot be reversed. It's not unrealistic to think that by being able to model complex relationships between pool balls, we can also gain insight into dynamic graphing systems. What if we could reverse engineer the node code from the ball break?


