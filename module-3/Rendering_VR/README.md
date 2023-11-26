# Technical Components - I

### Index
  * [Rendering in Virtual World](#rendering-in-virtual-world)  
    * Haptic Representation
    * Aural Representation
  * [Rendering Systems](#rendering-systems)

---  

## Rendering in Virtual World

The representation of various content in the virtual world is possible due to different rendering techniques dedicated to specific types of renderers. The following figure gives an overview of the same with respect to an immersed participant:  

![Rendering Overview](./assets/Rendering-Overview.png)

There are two main types of representations in the virtual world:

> 1. Haptic Representation
> 2. Aural Representation 

### Haptic Rendering


**TL;DR**  
> * based on friction-induced vibrations
> * tactile rendering device - used to recreate the perception of textures from a distance
> * consists of electro-active polymer **actuator** as key components
> * **pre-recorded vibrational stimulus** (by actuators) are regenerated in VE for immersiveness


In virtual reality (VR), **haptic rendering** refers to the simulation of the sense of touch through the use of haptic feedback technologies. It involves generating tactile sensations, such as vibrations or forces, to replicate the feel of virtual objects or interactions within a virtual environment. Haptic rendering enhances the overall immersive experience in virtual reality by providing users with a sense of touch and interaction with the virtual world.  

In brief, the idea of haptic rendering is based on friction-induced vibrations, a tactile rendering device used to recreate the perception of textures from a distance, consisting of electro-active polymer actuators as key components, and pre-recorded vibrational stimuli (by actuators) are regenerated in VE for immersiveness.

The process largely depends on two factors:

> 1. Contact Information  
> 2. Force Estimation  

**Contact Information:**

* Collision Detection & Response
* Visuals - Force shading and polishing
* Contact Impedance - contact to the surface (pressure and direction of force)
* Friction parameters
* Texture of Surface

**Force Estimation:** 

The _lateral-force gradient algorithm_ can be a suitable algorithm. 

* Use texture (height field) to encode surface details
* Directional penetration depth

Let's discuss the complete process of Haptic Rendering in Detail. 

#### Haptics Rendering Algorithms

![Haptics Rendering Algorithms](./assets/haptics-info.jpg)  

We will focus on rendering algorithms here.

As introduced in the introduction to [Haptic Rendering](#haptic-rendering), there is a sequence of steps involved in it. We'll quickly explore them, one by one:  

![Haptic Rendering Flow](./assets/haptics-rendering-flow.png)

**Collision Detection:**  

Here are the key points to be considered:  

> - Pipeline (shown above)
> - **Methods:**
>   1. Haptic Colloid _(3 parts)_
>      - Surface Decomposition _(3D objects)_
>   2. Sensation Preserving Simplification
>      - Multiresolution Representation 
>   3. **Collision Handling Concepts**

**Collision Handling:**  

It provides feedback after collision. It can be typically of two types:  

> 1. Penalty Based
>    - Good for Simple (surface) Objects
> 2. Constraint Based
>    - Upgraded (minimum proxy)

#### Force Model Based Rendering

Something about Force Model Based Rendering is described. The force model based rendering system depends on the two main factors:

> 1. Surface Properties  
> 2. Force Shading

Here we elaborate on these in a few bullet points:  

1. **Surface Properties:**
    - _Normal_
      - Force normal to the surface

    - _Contact Impedance_
      - On user’s interaction
      - Resistive in nature
      - Perpendicular
      - Often represented with <u>Spring & Viscous Damping Force</u>

    - _Friction_
      - Inertial Friction
      - Resistive Friction
      - Role of Torque

    - _Texture_
      - 3 Ways of Representation
      - Virtual Surface Information
      - Stochastic Process
2. **Force Shading:**
    - For direction and other properties

#### Stochastic Surface Modeling

As it makes sense, haptic rendering highly depends on the type of surface as well. This is why surface modeling is equally important in this complete process.  

The _stochastic surface modeling_ is a process to achieve this that uses Stochastic Modeling to estimate the roughness. As the property of roughness:

* Waviness should be removed first
* Can use filter

Following approach is used to remove the waviness from the surface:  

![Stochastic Surface Modeling](./assets/remove-waviness.png)

Now based on the collision on the different surface (varying in terms of texture) and the force applied, the contact force can be modeled. Following the formulation of contact force, i.e., response, for haptic rendering:

![Contact Force Formulation](./assets/haptic-rendering-formula.png)



### Aural Rendering

We'll start with _aural rendering_ by looking onto the key takeayaws from two of the previously emerged research works.   

The article, titled [_"Audio in VR: Effects of a Soundscape and Movement-Triggered Step Sounds on Presence"_](#references), highlights:  

> * Ambient soundscapes and movement-triggered step sounds can improve presence in VR.
> * The soundscape has a larger effect on presence than step sounds.
> * Audio rendering is an important part of creating a VR experience.
> * **Positioning:**
>     * Non-localizable sounds, such as the **ambient nature soundscape**, might NOT be assigned to any particular location.
>     * **Footstep sounds** could be positioned in space by assigning them to the right and left **foot of the avatar**.
> * All sounds were provided in stereophonic WAVE format and compressed to the Vorbis format.
> * The sampling rate was preserved at **44.1 kHz**.  

Another recent work (published in 2022) titled [_"On the Relative Importance of Visual and Spatial Audio Rendering on VR Immersion"_](#references) suggests that:  

> * **Ambient soundscapes** and **movement-triggered step sounds** can improve presence in VR.
> * The **soundscape has a larger effect** on presence than step sounds.
> * Audio rendering is an important part of creating a VR experience.

Here is a sample code:  

<script src="https://gist.github.com/ravi-prakash1907/8228f0037387049c8c177b779ac4d6ed.js"></script>


---  

## Rendering Systems

Yet to be updated...


---  

#### References  

1. Steven M. LaValle, **"VIRTUAL REALITY,"** 2020 [[access online](http://lavalle.pl/vr/)]  
2. William R. Sherman et al., **"Understanding Virtual Reality,"** 2018 [[PDF](https://drive.google.com/file/d/1N4GNZFMVCjRYew58dXQjSBIKYhuUZXhu/view?usp=drive_link)]
3. Dangxiao Wang et al., **"Haptic display for virtual reality: progress and challenges,"** 2019 [[online](https://www.sciencedirect.com/science/article/pii/S2096579619300130)]  
4. Angelika C. Kern et al., **"Audio in VR: Effects of a Soundscape and Movement-Triggered Step Sounds on Presence,"** 2020 [[online](https://www.frontiersin.org/articles/10.3389/frobt.2020.00020/full)]  
5. Thomas P. et al., **"On the Relative Importance of Visual and Spatial Audio Rendering on VR Immersion,"** 2022 [[online](https://www.frontiersin.org/articles/10.3389/frobt.2020.00020/full)]  


---  

[🔙 Module-3 Home Page](../)