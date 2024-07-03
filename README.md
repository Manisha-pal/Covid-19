**Overview:**

1. Given the limited availability of COVID-19 test kits in medical facilities, it is crucial to develop and implement an automated detection system as an alternative diagnostic tool for commercial use. Chest X-ray imaging plays a pivotal role in diagnosing COVID-19, and computer vision combined with deep learning techniques can effectively detect the virus from these images.

2. Leveraging the extensive availability of large-scale annotated image datasets, convolutional neural networks (CNNs) have achieved significant success in image analysis and classification. In this research, we propose a deep convolutional neural network trained on five open-access datasets, providing binary output (Normal and COVID).

**Motivation:**

1. Objective: Identify the most efficient and cost-effective methods for diagnosing COVID-19 and other viral and bacterial pneumonias (such as MERS, SARS, and ARDS).
2. Challenges: PCR tests often take around 48 hours to deliver results, which can be inaccurate and expensive, making them inaccessible to many people. Limited availability of tests in some regions leads to untreated cases and potential fatalities.
3. Resource Shortage: The overwhelming number of infected individuals has resulted in medicine shortages in local pharmacies.

**Dataset:**

1. The proposed model is trained on a combination of two open-source datasets: the COVID-19 Image Data Collection and Covid-Net. The former includes high-quality chest X-ray images from various medical sources, while the latter has images from infected patients, making it the largest benchmark dataset for COVID-19.

2. The combined dataset, after filtering, contains chest X-ray images categorized into two labels: Covid (Pneumonia)(Positive) and normal (Negative) . It includes images from notable medical databases such as the COVID-19 Chest X-ray Dataset Initiative.

**Techniques and Methodology:**

Proposed Model/Algorithm:
For the purpose of this project, I propose to implement a model based on Convolutional Neural Network (CNN). A Convolutional Neural Network (ConvNet/CNN) is a Deep Learning algorithm which can take in an input image, assign importance (learnable weights and biases) to various aspects/objects in the image and be able to differentiate one from the other. The pre-processing required in a ConvNet is much lower as compared to other classification algorithms. While in primitive methods filters are hand-engineered, with enough training, ConvNets have the ability to learn these filters/characteristics.

The architecture of a ConvNet is analogous to that of the connectivity pattern of Neurons in the Human Brain and was inspired by the organization of the Visual Cortex. Individual neurons respond to stimuli only in a restricted region of the visual field known as the Receptive Field. A collection of such fields overlaps to cover the entire visual area.

**Working of Model:**

Step 1: Initialising the CNN model.

Step 2: Add Convolutional layer. The objective of the Convolution Operation is to extract the high-level features such as edges, from the input image. ConvNets need not be limited to only one Convolutional Layer. Conventionally, the first ConvLayer is responsible for capturing the Low-Level features such as edges, colour, gradient orientation, etc. With added layers, the architecture adapts to the High-Level features as well, giving us a network, which has the wholesome understanding of images in the dataset, similar to how we would.

Step 3: Add Pooling Layer. The Pooling layer is responsible for reducing the spatial size of the Convolved Feature. This is to decrease the computational power required to process the data through dimensionality reduction. Furthermore, it is useful for extracting dominant features which are rotational and positional invariant, thus maintaining the process of effectively training the model. There are two types of Pooling: Max Pooling and Average Pooling.

Step 4: Add Convolutional layer and Pooling layer again to increase the accuracy.

Step 5: Flatten. Flatten layer is used to flatten images in to column vector. The flattened output is fed to a feed-forward neural network and backpropagation applied to every iteration of training

Step 6: Fully Connected Layer (Adding ANN layer into this model).

Step 7: Compile the model.

Step 8: Train the Model.

Step 9: Save the Model.

**Goals:**

1. Diagnosis Improvement: Address the issues of medication scarcity and inaccurate diagnoses by some healthcare providers.
2. Cost Reduction: Reduce the substantial national expenditure on diagnostic tests and treatments.
3. Technological Solution: Develop a web application utilizing Deep Learning and Artificial Intelligence algorithms to analyze CT chest scans and chest X-rays, providing immediate and accurate results for suspected cases.
