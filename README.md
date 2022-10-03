
<!-- Improved compatibility of back to top link: See: https://github.com/othneildrew/Best-README-Template/pull/73 -->
<a name="readme-top"></a>




<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/Arakim44/HAAR_DeepModel">
    <!--
    <img src="images/logo.png" alt="Logo" width="80" height="80">
    -->
  </a>
<h1 align="center"> HAAR_DeepModel (v.0.5) </h1>

<h3 align="center">Open Source Algorithm For Detecting Ship Passengers’ Abnormal Behaviors And Fall Accidents</h3>

  <p align="center">
    Preventing accident on ship and alert for help is the goal for the detection algorithm. Prevent more accidents, save more lives. 
    <br />
    <a href="https://github.com/Arakim44/HAAR_DeepModel"><strong>Explore the docs »</strong></a>
    <br />
    <br />
  <!--  <a href="https://github.com/Arakim44/HAAR_DeepModel">View Demo</a>
    ·-->
    <a href="https://github.com/Arakim44/HAAR_DeepModel/issues">Report Bug</a>
    ·
    <a href="https://github.com/Arakim44/HAAR_DeepModel/issues">Request Feature</a>
  </p>
</div>

<p align="center">
<img src="https://user-images.githubusercontent.com/20548632/193520288-a573b72a-bd71-4f44-bd7c-a083b6b4a0f1.gif" alt="Model Demo GIF"/>
</p>

<!-- ![modelDemoGif](https://user-images.githubusercontent.com/20548632/193520288-a573b72a-bd71-4f44-bd7c-a083b6b4a0f1.gif) -->



 
<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Requirenments</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <!-- <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul> -->
    </li>
    <!-- <li><a href="#usage">Usage</a></li> -->
    <!-- <li><a href="#roadmap">Roadmap</a></li> -->
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <!-- <li><a href="#contact">Contact</a></li> -->
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<!--
[![Product Name Screen Shot][product-screenshot]](https://example.com)
-->

Open Source CCTV based AI algorithm which detects the abnormal behaviors of passengers on the ship to predict the possible accidents and warn the on board sailors. When the CCTV catches the actual accidents, the algorithm will alert the incidents and the current accident location to nearby coast guards in real time in order to increase the rescue rate for the fallen passengers.

<!--Here's a blank template to get started: To avoid retyping too much info. Do a search and replace with your text editor for the following: `github_username`, `repo_name`, `twitter_handle`, `linkedin_username`, `email_client`, `email`, `project_title`, `project_description`-->

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Requirements

* Cuda, Cudnn : Cuda support GPU Device (We implemented RTX 3090)
* Detectron 2 
  * Linux or macOS with Python ≥ 3.7
  * PyTorch ≥ 1.8 and torchvision that matches the PyTorch installation. Install them together at pytorch.org to make sure of this
  * OpenCV is optional but needed by demo and visualization
  * See [Detectron Install.md](https://github.com/facebookresearch/detectron2/blob/main/INSTALL.md)
* AdelaiDet
  * Detectron2 base
  * See [AedlaiDet Install.md](https://github.com/aim-uofa/AdelaiDet)
  * FCPose

[Download pretrain Model](https://github.com/aim-uofa/AdelaiDet/blob/master/configs/FCPose/README.md)


<!--
* [![Next][Next.js]][Next-url]
* [![React][React.js]][React-url]
* [![Vue][Vue.js]][Vue-url]
* [![Angular][Angular.io]][Angular-url]
* [![Svelte][Svelte.dev]][Svelte-url]
* [![Laravel][Laravel.com]][Laravel-url]
* [![Bootstrap][Bootstrap.com]][Bootstrap-url]
* [![JQuery][JQuery.com]][JQuery-url]

-->


<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->

## Getting Started

The model can be started by executing haar_demo.py in /HAAR_Demo directory.


[Sample Run Script]
```
python HAAR_Demo/haar_demo.py \
--video-input ./HAAR_Demo/cctv_demo.mp4 \
--opts MODEL.WEIGHTS ./models/fcpose50.pth
```

<!--

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* Tensorflow
  ```sh
   install  -g
  ```
* PyTorch
  ```sh
  something
  ```
* Jupyter Lab
  ```sh
  something
  ```

  
### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/Arakim44/HAAR_DeepModel.git
   ```
3. Install packages
   ```sh
    install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- USAGE EXAMPLES -->


<!-- ## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->



<!-- ROADMAP -->

<!--
## Roadmap

- [ ] Feature 1
- [ ] Feature 2
- [ ] Feature 3
    - [ ] Nested Feature

See the [open issues](https://github.com/Arakim44/HAAR_DeepModel) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

-->

<!-- CONTRIBUTING -->
## Contributing

[Click Here To See How To Contribute](https://github.com/Smart-Safety-Ocean/HAAR_DeepModel/blob/main/Contributing.md)

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
<!-- ## Contact

Your Name - [@twitter_handle](https://twitter.com/twitter_handle) - email@email_client.com

Project Link: [https://github.com/Arakim44/HAAR_DeepModel](https://github.com/Arakim44/repo_name)

<p align="right">(<a href="#readme-top">back to top</a>)</p> -->



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [SSL](https://www.smartsafety.co.kr/)
* [Dr.Hong](https://github.com/HongDoubleS)
* ...[]()

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Arakim44/HAAR_DeepModel.svg?style=for-the-badge
[contributors-url]: https://github.com/Arakim44/HAAR_DeepModel/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Arakim44/HAAR_DeepModel.svg?style=for-the-badge
[forks-url]: https://github.com/Arakim44/HAAR_DeepModel/network/members
[stars-shield]: https://img.shields.io/github/stars/Arakim44/HAAR_DeepModel.svg?style=for-the-badge
[stars-url]: https://github.com/Arakim44/HAAR_DeepModel/stargazers
[issues-shield]: https://img.shields.io/github/issues/Arakim44/HAAR_DeepModel.svg?style=for-the-badge
[issues-url]: https://github.com/Arakim44/HAAR_DeepModel/issues
[license-shield]: https://img.shields.io/github/license/Arakim44/HAAR_DeepModel.svg?style=for-the-badge
[license-url]: https://github.com/Arakim44/HAAR_DeepModel/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[Vue-url]: https://vuejs.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com 

