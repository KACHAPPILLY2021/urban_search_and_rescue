<a name="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">


  <h1 align="center">Turtlebot3 Navigation using move_base and slam </h1>


</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary><h3>Table of Contents</h3></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#demo">Demo</a></li>
      </ul>
    </li>
    <li>
      <a href="#documentation">Documentation</a>
      <ul>
        <li><a href="#report">Report</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contributors">Contributors</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project



Implemented Depth First Search algorithm using Object Oriented Programming in C++ and visualized its output using Micromouse simulator.

Summary of tasks achieved:
* Implemented DFS using a representation of the maze(mouse has no prior knowledge of walls except the boundaries.)
* Generated path from current position to goal using the representation of the maze.
* Moved the mouse using API interface commands and updated the walls as detected.
* The robot halted when the mouse hit a wall, and DFS was employed to recalculate the path using prior wall data.
* The described steps were repeated until the goal position was achieved.


<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Demo

<div align="center">


  <h4 align="center"> Explorer and Follower working (X16 Speed)</h4>


</div>

https://user-images.githubusercontent.com/90359587/224387441-d45e0f85-1992-43dc-be13-360b4ef2d11c.mp4
<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- Document and Reports -->
## Documentation

The documentation for this project can be found [here](https://kachappilly2021.github.io/urban_search_and_rescue/).


### Report

* The detailed problem statement and additional background information can be found [here](https://github.com/KACHAPPILLY2021/urban_search_and_rescue/blob/main/primary/final_project_fall2021.pdf)
* The main report which dicusses our approach in great detail is [here](https://github.com/KACHAPPILLY2021/urban_search_and_rescue/blob/main/report/ENPM809Y_Final_Report__Group7.pdf)
<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- GETTING STARTED -->
## Getting Started

These are the instructions to get started on the project.
To get a local copy up and running follow these simple steps.

### Prerequisites
* ROS 1 with [Turtlebot3](https://emanual.robotis.com/docs/en/platform/turtlebot3/quick-start/) installed
* Catkin workspace ```catkin_ws```
* OS - Linux (tested)


### Installation

Installing the dependencies and running the code.

1. Clone the repo
   ```sh
   https://github.com/KACHAPPILLY2021/urban_search_and_rescue.git
   ```
2. To install navigation and slam dependencies
   ```sh
   cd ~/urban_search_and_rescue/script
   ```
   ```sh
   sudo chmod a+rwx install.bash
   ```
   ```sh
   ./install.bash
   ```
3. Copy the ROS package ```final_project``` and place it inside ```catkin_ws/src``` and build
   ```sh
   catkin build final_project
   ```
4. Save this command in ```bashrc``` file for loading ArUco markers in gazebo
   ```sh
   export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/home/<username>/catkin_ws/src/final_project/models
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

To run this project, only two commands are required.
1. Source the workspace
2. To start Gazebo and RViz, and for setting parameters on the Parameter Server and spawning robots:
   ```sh
   roslaunch final_project multiple_robots.launch
   ```
3. Open new terminal and run the node:
   ```sh
   rosrun final_project final_project_node
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTORS -->
## Contributors

- [Hemanth Joseph](https://github.com/HemanthJoseph)
- [Jeffin Johny](https://github.com/KACHAPPILLY2021)
- [Pradip Kathiriya](https://github.com/Pradip-Kathiriya)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Jeffin Johny K - [![MAIL](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:jeffinjk@umd.edu)
	
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/KACHAPPILLY2021)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](http://www.linkedin.com/in/jeffin-johny-kachappilly-0a8597136)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See [MIT](https://choosealicense.com/licenses/mit/) for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
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
