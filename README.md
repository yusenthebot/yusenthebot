<!-- ASCII name banner: all lines padded to exactly 67 chars (incl. trailing -->
<!-- spaces) so per-line centering inside <pre> can never misalign the box art. -->
<div align="center">

<pre>
██╗   ██╗██╗   ██╗███████╗███████╗███╗   ██╗    ██╗  ██╗██╗███████╗
╚██╗ ██╔╝██║   ██║██╔════╝██╔════╝████╗  ██║    ╚██╗██╔╝██║██╔════╝
 ╚████╔╝ ██║   ██║███████╗█████╗  ██╔██╗ ██║     ╚███╔╝ ██║█████╗  
  ╚██╔╝  ██║   ██║╚════██║██╔══╝  ██║╚██╗██║     ██╔██╗ ██║██╔══╝  
   ██║   ╚██████╔╝███████║███████╗██║ ╚████║    ██╔╝ ██╗██║███████╗
   ╚═╝    ╚═════╝ ╚══════╝╚══════╝╚═╝  ╚═══╝    ╚═╝  ╚═╝╚═╝╚══════╝
                                                                   
        WHOLE-BODY RL + LLM AGENT KERNELS FOR LEGGED ROBOTS        
        AI ENGINEERING @ CMU // CO-FOUNDER @ VECTOR ROBOTICS       
</pre>

</div>

<!-- Animated tagline: readme-typing-svg (demolab instance, verified live). -->
<!-- <picture> serves a darker green on light theme so it stays readable. -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&pause=1200&duration=2600&color=00FF9C&center=true&vCenter=true&width=620&height=40&lines=%24+vector+%22fetch+the+bottle%22;decompose+-%3E+plan+-%3E+verify+-%3E+act;whole-body+RL+for+legged+robots;LLM+agent+kernel+--+no+fine-tuning;Unitree+Go2+%2B+SO-ARM101+--+sim2real" />
    <source media="(prefers-color-scheme: light)" srcset="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&pause=1200&duration=2600&color=00935A&center=true&vCenter=true&width=620&height=40&lines=%24+vector+%22fetch+the+bottle%22;decompose+-%3E+plan+-%3E+verify+-%3E+act;whole-body+RL+for+legged+robots;LLM+agent+kernel+--+no+fine-tuning;Unitree+Go2+%2B+SO-ARM101+--+sim2real" />
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=16&pause=1200&duration=2600&color=00FF9C&center=true&vCenter=true&width=620&height=40&lines=%24+vector+%22fetch+the+bottle%22;decompose+-%3E+plan+-%3E+verify+-%3E+act;whole-body+RL+for+legged+robots;LLM+agent+kernel+--+no+fine-tuning;Unitree+Go2+%2B+SO-ARM101+--+sim2real" alt="Rotating terminal lines: vector fetch command, decompose to act pipeline, whole-body RL, LLM agent kernel, Go2 plus SO-ARM101 sim2real" />
  </picture>
</p>

<p align="center">
  <a href="https://yusenthebot.github.io"><img src="https://img.shields.io/badge/portfolio-enter_terminal-00FF9C?style=flat-square&logo=gnometerminal&logoColor=black&labelColor=0a0e14" alt="Terminal portfolio" /></a>
  <a href="https://github.com/VectorRobotics"><img src="https://img.shields.io/badge/Vector_Robotics-co--founder-00FF9C?style=flat-square&logo=github&logoColor=white&labelColor=0a0e14" alt="Vector Robotics" /></a>
  <a href="https://www.linkedin.com/in/yusen-xie-5327b8382/"><img src="https://img.shields.io/badge/LinkedIn-connect-00FF9C?style=flat-square&logo=linkedin&logoColor=white&labelColor=0a0e14" alt="LinkedIn" /></a>
</p>

<p align="center">
  <a href="https://yusenthebot.github.io"><img src="./assets/robot.gif" width="200" alt="Pixel robot V — click to enter the terminal portfolio" /></a>
  <br/>
  <sub><code>now building -> vector-os-nano: one natural-language command in, whole-body motion out</code></sub>
</p>

### `[ flagship ]`

<!-- Repo pin card: github-readme-stats (verified 200), self-contained dark -->
<!-- panel so it reads on both GitHub themes. -->
<p align="center">
  <a href="https://github.com/VectorRobotics/vector-os-nano"><img src="https://github-readme-stats.vercel.app/api/pin/?username=VectorRobotics&repo=vector-os-nano&show_owner=true&bg_color=0a0e14&title_color=00FF9C&text_color=9fb1c1&icon_color=00FF9C&hide_border=true" alt="vector-os-nano repository card" /></a>
  <br/>
  <sub>Cross-embodiment robot OS — natural-language control with no fine-tuning, ROS2 Nav2 autonomy,<br/>and an MCP server exposing every robot skill plus live world state. Runs on Unitree Go2 and SO-ARM101.</sub>
</p>

<!-- The kernel loop. Mermaid renders natively on GitHub; theme:base with -->
<!-- self-contained dark node fills stays legible on light and dark pages. -->
```mermaid
%%{init: {"theme": "base", "themeVariables": {"primaryColor": "#0d1117", "primaryTextColor": "#00ff9c", "primaryBorderColor": "#00c277", "lineColor": "#00a86b", "fontFamily": "monospace", "fontSize": "13px"}}}%%
flowchart LR
    NL["natural language"] --> DEC["decompose"]
    DEC --> PLAN["plan"]
    PLAN --> VER["verify"]
    VER --> ACT["act"]
    ACT --> WBC["whole-body control"]
    WBC --> HW["Go2 + SO-ARM101"]
    VER -.-> PLAN
```

<p align="center">
  <sub><code>[ the agent kernel loop — every command runs through it ]</code></sub>
</p>

### `[ selected_work ]`

> Physical-robot RL and control first; the tooling that makes it shippable second.

| repo | signal |
|------|--------|
| [`G1Pilot`](https://github.com/VectorRobotics/G1Pilot) | C++ inverse kinematics for the Unitree G1 humanoid — Pinocchio + CasADi |
| [`vector_perception`](https://github.com/VectorRobotics/vector_perception) | full perception pipeline for general robotics |
| [`Hop-Dynamics`](https://github.com/yusenthebot/Hop-Dynamics) | wheeled bipedal robot with an active tail |
| [`openclaw-dashboard`](https://github.com/yusenthebot/openclaw-dashboard) | terminal-aesthetic agent control panel |

### `[ stack ]`

<pre>
$ vector skills --tree
.
├── learning/     RL (PPO) · imitation · diffusion policy · VLA/VLN · sim2real
├── control/      whole-body control · legged locomotion · IK · behavior trees · Nav2
├── perception/   SLAM · LiDAR-IMU odometry · sensor fusion · YOLO
├── simulation/   MuJoCo · Isaac Lab/Sim · Genesis · Gazebo
└── agents/       LLM agent kernels · MCP servers · tool calling · Claude Code
</pre>

<p align="center">
  <img src="https://skillicons.dev/icons?i=python,cpp,pytorch,ros,opencv,linux,bash,docker,git,githubactions,cmake,raspberrypi,ts,react,nextjs,fastapi&perline=8" alt="Tooling: Python, C++, PyTorch, ROS, OpenCV, Linux, Bash, Docker, Git, GitHub Actions, CMake, Raspberry Pi, TypeScript, React, Next.js, FastAPI" />
</p>

---

<!-- 3D contribution graph - generated daily by .github/workflows/profile-3d.yml, -->
<!-- committed under profile-3d-contrib/ by the Action. Themed placeholder SVGs -->
<!-- are committed at the same paths so this section never renders a broken image -->
<!-- before the first run; the Action overwrites them with the real graphs. -->
<!-- Fallback <img> uses the night variant deliberately: its dark panel is -->
<!-- self-contained and legible on both GitHub themes. -->
<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./profile-3d-contrib/profile-night-rainbow.svg" />
    <source media="(prefers-color-scheme: light)" srcset="./profile-3d-contrib/profile-green.svg" />
    <img src="./profile-3d-contrib/profile-night-rainbow.svg" width="100%" alt="3D isometric contribution graph, regenerated daily by a GitHub Action (placeholder shown until the first run)" />
  </picture>
  <br/>
  <sub><code>[ contribution telemetry - regenerated daily by a GitHub Action ]</code></sub>
</p>

<p align="center">
  <sub><code>[ contact ]</code> &nbsp;<a href="mailto:yusenthebot@outlook.com">yusenthebot@outlook.com</a></sub>
</p>
