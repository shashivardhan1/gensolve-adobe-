<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<h1 align="center">DoodleFix: An Algorithm for Regularizing Shapes, Analyzing Symmetry, and Completing Complex Doodles</h1>
<div align="center">
  <a href="https://github.com/dshashivardhj2c5_team/doodlefix">
    <img src="assets/doodlefix-high-resolution-logo.png" alt="DoodleFix Logo">
  </a>
  <p>
    DoodleFix is your go-to tool for transforming distorted shapes into their closest geometric forms while ensuring symmetry in the refined shapes.
  <br />
    <br />
    <a href="https://youtu.be/TOwcUPju1h8">Watch the Demo</a>
    ·
    <a href="https://github.com/dshashivardhj2c5_team/doodlefix/issues">Report a Bug</a>
    ·
    <a href="https://github.com/dshashivardhj2c5_team/doodlefix/issues">Request a Feature</a>
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary><h2> Table of Contents </h2></summary>
  <ol>
    <li>
      <a href="#abouttheproject"> About The Project </a>
      <ul>
        <li><a href="#mission"> Mission </a></li>
        <li><a href="#valueproposition"> Value Proposition </a></li>
      </ul>
    </li>
    <li><a href="#keyfeatures">Key Features</a></li>
    <li><a href="#builtwith">Built With</a></li>
    <li><a href="#detection">Shape Classification and Transformation</a></li>
    <li>
      <a href="#gettingstarted">Getting Started</a>
      <ul>
        <li><a href="#installation">Installation Instructions</a></li>
        <li><a href="#example">Example Usage</a></li>
      </ul>
    </li>
    <li><a href="#clicommands">CLI Commands</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#team">Team Members</a></li>
  </ol>
</details>

<h2 id="abouttheproject"> About the Project </h2>

DoodleFix leverages advanced deep learning and geometric algorithms to transform hand-drawn doodles into perfectly regularized shapes. By classifying shapes using a custom ResNet-based CNN, the system corrects irregularities, identifies symmetry, and even completes missing parts. The final output showcases a harmonious collection of flawless geometric figures, demonstrating the power of AI in creative and technical shape analysis. An impressive blend of art and technology!

Check out our demo [here](https://youtu.be/TOwcUPju1h8).

<h3 id="mission"> Our Mission </h3>

Our mission is to blend the power of AI with creative expression, transforming irregular doodles into perfect geometric forms. We aim to push the boundaries of shape recognition and correction, turning every sketch into a masterpiece of symmetry and precision.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h3 id="flowchart"> WorkFlow </h3>

![flowchart](https://github.com/user-attachments/assets/e6acb522-a469-42c3-b3a9-ccb27af42e85)
![flowchart2](https://github.com/user-attachments/assets/c0de5de4-147b-4660-9031-83e6ae3dd8c9)

<h2 id="keyfeatures"> Key Features </h2>

- 🔧 **Irregular Shape Identification:** Detect and classify various irregular doodle shapes, including polygons, stars, and more. Utilize advanced image processing to handle diverse and complex forms.

- 🔧 **Shape Regularization:** Transform identified shapes into regular geometric forms. Ensure shapes are correctly represented by applying algorithms to correct distortions and irregularities.

- 🔧 **Symmetry Analysis:** Evaluate shapes for symmetry along multiple axes. Display symmetry results visually and use these insights to complete and enhance the shapes.

- 🔧 **Shape Completion and Occlusion Handling:** Fill in incomplete shapes and reveal any occluded parts based on detected symmetry. Ensure that all visible and hidden portions are accurately represented.

- 🔧 **Multi-Class Classification:** Use a custom CNN model to classify shapes into predefined categories such as Square, Circle, Star, Rectangle, and polygons. Handle edge cases with high accuracy.

- 🔧 **Visual Representation and Correction:** Provide visual feedback by displaying regularized shapes and their symmetry on a unified image. Correct shapes to ensure they meet predefined geometric criteria.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="builtwith"> Built With </h2>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)  ![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white) ![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white) ![Poetry](https://img.shields.io/badge/Poetry-%233B82F6.svg?style=for-the-badge&logo=poetry&logoColor=0B3D8D) 
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)

<h3> Open Source Pre-trained Models: </h3>

- [ResNet18](https://pytorch.org/vision/main/models/generated/torchvision.models.resnet18.html)
  
<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h1 id="detection"> How DoodleFix Works 🤔 </h1>

**Step 1: Finding Connected Components**
- Detect and extract distinct shapes from the doodle using connected component analysis. This process involves identifying and labeling clusters of black pixels to determine individual shapes.

<p align="center">
  <img src="https://github.com/user-attachments/assets/60d9a886-0f31-42eb-999d-64b798c3e430" alt="DoodleFix making sad circle into happy one" style="width: 50%; height: auto;">
</p>

**Step 2: Classifying Shapes with CNN**
- Apply a custom CNN model to classify each identified shape into predefined categories such as Square, Circle, Star, Rectangle, or Polygon. The model processes black-and-white images of each shape to determine its class.

 <p align="center">
  <img src="https://github.com/user-attachments/assets/1254558c-eac2-4e06-8c1b-6122c17df7d4" alt="DoodleFix making sad circle into happy one" style="width: 50%; height: auto;">
</p>


**Step 3: Applying Shape Regularization**
- Use algorithms to transform classified shapes into their correct geometric representations. Regularize the shapes by correcting distortions and aligning them to standard geometric forms.

<p align="center">
  <img src="https://github.com/user-attachments/assets/d5b897a0-19ae-483b-9327-ae3bc270d224" alt="DoodleFix making sad circle into happy one" style="width: 30%; height: auto; margin: 0 10px;">
  <img src="https://github.com/user-attachments/assets/f3cc6f15-35df-4a9b-aee4-f714e8a2aea6" alt="Description of the second image" style="width: 30%; height: auto; margin: 0 10px;">
  <img src="https://github.com/user-attachments/assets/18982be1-df46-4dc4-8543-51fb98aecaf9" alt="Description

 of the second image" style="width: 30%; height: auto; margin: 0 10px;">
</p>

**Step 4: Symmetry Analysis and Shape Completion**
- Evaluate the regularized shapes for symmetry along multiple axes. Use the detected symmetry to complete missing parts of the shape, ensuring a harmonious and accurate representation.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="gettingstarted"> Getting Started </h2>

<h3 id="installation"> Installation Instructions </h3>

1. Clone the repository:

   ```sh
   git clone https://github.com/dshashivardhj2c5_team/doodlefix.git
   ```

2. Install dependencies using Poetry:

   ```sh
   cd doodlefix
   poetry install
   ```

3. Activate the virtual environment:

   ```sh
   poetry shell
   ```

<h3 id="example"> Example Usage </h3>

- Run the following command to apply DoodleFix on an image:

  ```sh
  python doodlefix.py --input_path <path_to_input_image> --output_path <path_to_output_image>
  ```

- Example:

  ```sh
  python doodlefix.py --input_path ./samples/doodle1.png --output_path ./output/doodle1_fixed.png
  ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="clicommands"> CLI Commands </h2>

- **Run the model on an image:** Run `python doodlefix.py --input <image_path> --output <output_path>` to classify and regularize shapes in the input image, saving the results to the specified output path.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="license"> License </h2>

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="contributing"> Contributing </h2>

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="team"> Team Members </h2>

- **[dshashivardhj2c5_Team](https://github.com/dshashivardhj2c5_team)**
  - **[Ashutosh Singh](https://github.com/username)**: Implemented the custom CNN model for shape classification.
  - **[Jane Doe](https://github.com/janedoe)**: Developed the symmetry analysis algorithm and shape regularization.
  - **[John Smith](https://github.com/johnsmith)**: Handled the data collection and preprocessing pipeline.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
