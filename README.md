<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<h1 align="center">GeoSketch: An Algorithm for Regularizing Shapes, Analyzing Symmetry, and Completing Complex Doodles</h1>
<div align="center">
  <a href="https://github.com/shashivardhan1/gensolve-adobe-">
  </a>
  <p>
    GeoSketch is your go-to tool for transforming distorted shapes into their closest geometric forms while ensuring symmetry in the refined shapes.
  <br />
    <br />
    <a href="https://youtu.be/TOwcUPju1h8">Watch the Demo</a>
    ·
    <a href="https://github.com/shashivardhan1/gensolve-adobe-/issues">Report a Bug</a>
    ·
    <a href="https://github.com/shashivardhan1/gensolve-adobe-/issues">Request a Feature</a>
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

GeoSketch leverages advanced deep learning and geometric algorithms to transform hand-drawn doodles into perfectly regularized shapes. By classifying shapes using a custom ResNet-based CNN, the system corrects irregularities, identifies symmetry, and even completes missing parts. The final output showcases a harmonious collection of flawless geometric figures, demonstrating the power of AI in creative and technical shape analysis. An impressive blend of art and technology!

Check out our demo [here](https://youtu.be/TOwcUPju1h8).

<h3 id="mission"> Our Mission </h3>

Our mission is to blend the power of AI with creative expression, transforming irregular doodles into perfect geometric forms. We aim to push the boundaries of shape recognition and correction, turning every sketch into a masterpiece of symmetry and precision.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
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

<h2 id="gettingstarted"> Getting Started </h2>

<h3 id="installation"> Installation Instructions </h3>

1. Clone the repository:

   ```sh
   git clone https://github.com/shashivardhan1/gensolve-adobe-.git
   ```

2. Install dependencies using Poetry:

   ```sh
   cd gensolve-adobe-
   poetry install
   ```

3. Activate the virtual environment:

   ```sh
   poetry shell
   ```

<h3 id="example"> Example Usage </h3>

- Run the following command to apply GeoSketch on an image:

  ```sh
  python gensolve-adobe-.py --input_path <path_to_input_image> --output_path <path_to_output_image>
  ```

- Example:

  ```sh
  python gensolve-adobe-.py --input_path ./samples/doodle1.png --output_path ./output/doodle1_fixed.png
  ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="clicommands"> CLI Commands </h2>

- **Run the model on an image:** Run `python gensolve-adobe-.py --input <image_path> --output <output_path>` to classify and regularize shapes in the input image, saving the results to the specified output path.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="license"> License </h2>

Distributed under the MIT License. See `LICENSE` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="contributing"> Contributing </h2>

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<h2 id="team"> Team Members </h2>

- **[dshashivardhj2c5_Team](https://github.com/shashivardhan1)**
  - **[Shashivardhan](https://github.com/shashivardhan1)**: Implemented the custom CNN model for shape classification.
  - **[Bala Barghav](https://github.com/balabhargav9)**: Developed the symmetry analysis algorithm and shape regularization.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
