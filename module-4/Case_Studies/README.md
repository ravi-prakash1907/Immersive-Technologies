# Case Studies  

## Index
* [Design and Evaluation](#design-and-evaluation)  
* [Production Pipeline](#production-pipeline)  
  * Sensing  
  * Rendering  
  * Mobile, Stand-alone, and High-end Computing Platforms 

---  

## Design and Evaluation

### Design 

- AR/VR
- Flow
- UI
- Backend and integration technologies

### Evaluation

- Ease of access
- Dependencies 
- Security
- Scope and Usability

---  

## Production Pipeline

### General Pipeline

1. Selection of problem
2. Based on the R-V Continuum, finalize the suitable solution
3. Sorting dependencies
4. Production
  - Sensing
  - Rendering
5. Adaptability _etc..._

The production of Immersive Reality typically consists of several steps and processes. Three of such most essential processes include:  

1. Sensing
2. Rendering
3. High-end computing platforms


#### Sensing

During the sensing process, the devices are set up and calibrated to synthesize the information the most efficiently. This information can be:  

- Audio
- Image/Video
- Haptic Sensations _etc.._

The sensed information is then ready for processing and further operations.  

#### Rendering

It involves the presentation of different information to the end user. Depending upon the type of information, the rendering can be done in many ways. It can be:  

- Aural rendering
- Visual rendering
- Haptic rendering _etc..._

As discussed, the cruciality, volume, and dependency of and over the information may vary as per the use cases; it’s important to note the requirement to make the rendering compatible for various devices ranging from mobile phones to smart HMDs.  


### XR Video Production 

The 360 VR production requires sequential steps to write, plan, staff, and cast the VR solution.

#### Writing & Planning

- Native thinking is the art of composing content with the unique capabilities of XR in writing.  
- Consider/use space as a scope of understanding the user's behavior.  
- Location scouting is a crucial consideration. Before getting into production, practice 360 shots should be taken.  
- Due to distant background objects, it’s very important to consider the placement of objects, characters, and plot details while writing and planning.  
- Production Tools (for 360):  
  - Guiding cues: No cuts, zooms, and camera movements.  
  - Audio cues are sound elements designed to draw the audience's attention.  
  - Visual cues  
  - Point of Interest, or POI is the viewer’s area of attention.  
  - Camera movements, lightening, and colors.  
  - Text and graphic overlays  
  - The Authoring tools are also categorized into 5 classes based on the complexity and compatibility of ideas and devices, respectively. [paper](http://michael-nebeling.de/publications/ismar18adj.pdf)  

#### Production Preparation

**Storyboarding and Prototyping**  

* The storyboard should be a **representation of how the video will unfold,** it’s typically a series of thumbnails that illustrate key scenes, environments, and production elements with notes. 

**Overhead Diagrams & Blocking Shots**  

![Overhead Diagrams & Blocking Shots](./assets/1-Overhead-Diagrams-Blocking-Shots.png)  

- Strategic Scene Mapping  
- Stitching Awareness  
- Quality Boost with Overheads  
- Prototyping can also be split among many levels. Broadly we can categorize it into 2 parts [paper](http://michael-nebeling.de/publications/chi18a.pdf):  
  - Physical Prototyping
  - Digital Prototyping 

![Prototyping](./assets/2-Prototyping.png)  


**Shot Lists**  

![Shot Lists](./assets/3-Shot-List.png)  

* Create a shot list and prepare a schedule  

#### Crewing-up

There can be different crews depending on the **scenarios** and the **type of project,** i.e., _experiment, short-term project, and big/long-term project._ Following table discusses this better:  

| Crew Size | Roles Covered | Benefits | Drawbacks |
|-----------|---------------|----------|-----------|
| **1**         | Director, Director of Photography (DP), Sound Engineer _(all combined)_       | Learn quickly, **cost-effective,** gain experience across all aspects | Time-consuming, potentially overwhelming |
| **2-3**       | Director, DP, Sound Engineer _**(split responsibilities)**_        | Specialization based on strengths, **efficient workflow** | Requires **strong communication** and **collaboration** |
| **3+**        | Director, DP, Sound Engineer, Producer/Coordinator, Grip & Electric, Script Supervisor, Production Assistant _(dedicated roles)_ | Ideal for **complex** shoots, high-quality production | Increased cost and complexity |


### Reviewed Projects

1. [Field Engineer **Assistance via Augmented Reality**](https://www.infosys.com/services/incubating-emerging-technologies/success-stories/augmented-reality-app.html)
    1. Visualize relevant data via Infosys AR-VR
        - visualize & manipulate large amounts of data
        - identify business anomalies
        - remote maintenance, _etc.._
    2. Real-time augmentation of sensor information
    3. Capable of predictive maintenance
    4. Multiple synchronized processes

2. [A global EPC company undertakes **immersive design reviews with 3D models and VR**](https://www.infosys.com/services/incubating-emerging-technologies/success-stories/augmented-reality-app.html)
   1. Solution for viewing the BIM data onto a virtual reality (VR) device
   2. Immersive viewing on a 1:1 scale
      - Facilitated collaboration in VR
   3. Architecture:
      - Built on the iModel.js framework of JavaScript
      - Frontend using Unity 3D (game engine)
      - Server through a Google Protocol Buffer over a WebSocket
   4. Streaming Building information modeling (BIM) data to the HTC VIVE VR device
   5. Enables walk-through and self-teleporting at different locations on the 3D model
   6. Challenges:
      - Varying data sizes _(70MB to 5.8GB triangles)_
      - Iterative design

3. Role-based **Collaborative Immersive Authoring** [[online]](https://dl.acm.org/doi/abs/10.1145/3313831.3376637) [[pdf]](https://dl.acm.org/doi/pdf/10.1145/3313831.3376637)

- _Here the authors study how novice AR/VR creators can take advantage of the roles and modes in **“XRDirector” to prototype complex scenes** with animated 3D characters, light effects, and camera movements._  

    1. XRDirector is a role-based collaborative immersive authoring system.  
    2. It addresses the challenges of existing immersive authoring tools by using roles inspired by filmmaking to structure the authoring process and enable multiple designers to work together.  
    3. The system was informed by case studies and workshops with novice AR/VR creators.  
    4. It was found to make AR/VR scene creation faster and easier, and to help identify strengths and weaknesses of different roles and modes.  
 

### Considerations & Mistakes in Production  

#### Synchronization:
- Crucial for smooth editing, especially when using separate audio or multi-camera rigs.
- Techniques: _Clap, light flash, dog clicker, motion twist._
- Resources: GoPro 360 Beginners Guide, Syncing in Premiere for Autopano Video Pro.

#### Stabilization & Movement:
- Avoid _yaw movement_ (twisting the entire world) - _VR sickness._
- Move steadily and linearly, and avoid shaky accelerations.
- Consider stabilizers like gimbals and _anti-vibration equipment._
- Balance weight on monopods/tripods to avoid falls and damage.

#### Settings:
- Check before each shot (exposure, etc.)
- Use _live-preview options_ when possible.

#### Object Proximity:
- Keep objects at a comfortable distance to _avoid immersion breaks._
- Careful with optical-flow stitching (Google Jump).

#### Avoiding Stitch Issues:
- Keep action in front of camera lenses, not between.
- Shoot test shots to identify potential stitch line problems.

#### Hiding Equipment & Crew:
- Takes away from immersion - finds _hiding spots_ or uses crew as extras.
- _Live preview_ helps spot details.

#### Plate Shots & Post-Production Masking:
- Secondary shots of empty _environments for covering mistakes._
- Ensures a clean baseline for editing and masking.



---  

#### References  

<!-- 1. Frank Dellaert, **"Square root SAM,"** 2005 [[online](https://www.researchgate.net/publication/221344652_Square_root_SAM)]    
2. **Digital Guide - IONOS,** last accessed December 2023 [[website](https://www.ionos.co.uk/digitalguide/)]
3. **Paninian,** (online), last accessed December 2023 [[website](https://www.paninian.com/airvoxels-digitaltwin)] -->

---  

[🔙 Module-3 Home Page](../)