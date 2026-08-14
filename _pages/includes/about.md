I am a Postdoctoral Associate at Cornell University, working with [Prof. Jian-Xun Wang](https://www.duffield.cornell.edu/people/jian-xun-wang/). Previously, I was a Postdoctoral Fellow at the University of Notre Dame. I received both my Ph.D. and B.S. degrees from Tianjin University.

My research is **differentiable computation and embedded learning for nonlinear, coupled dynamical systems in mechanics**—fluid, structural, and their interaction (FSI)—grounded in physical understanding and proven on real engineering systems, toward intelligent computation that serves understanding, prediction, and inverse design. This spans three connected thrusts:

- **Differentiable computation** for multiphysics simulation — GPU-native solvers that make gradient-based inverse design tractable on high-dimensional, coupled systems.
- **Learning within physics-based solvers** — neural components trained end-to-end through the solver dynamics, so models stay stable and generalizable over long rollouts.
- **Fluid–structure interaction**, from mechanism to deployment — explaining, predicting, and controlling flow-induced vibration in real multi-body engineering systems.

<mark>I'm actively searching for a tenure-track faculty position in mechanical, aerospace, civil, or computing-related departments. Please reach out to me if you think my background fits the position.</mark>

<!-- I am a Ph.D. candidate in [Elmore Family School of Electrical and Computer Engineering](https://engineering.purdue.edu/ECE) at [Purdue University](https://www.purdue.edu) and working with [Prof. Qi Guo](https://www.qiguo.org/pi). My current research focuses on computer vision and deep learning, with a particular emphasis on the joint development of novel deep learning algorithms and camera setups to optimize overall system performance across multiple tasks, such as boundary detection and depth estimation, in photon-limited environments.

Prior to Purdue, I completed my M.S. in [Khoury College of Computer Sciences](https://www.khoury.northeastern.edu/) at [Northeastern University](https://www.northeastern.edu) under the supervision of [Prof. Lawson L.S. Wong](http://www.ccs.neu.edu/home/lsw/). Previously, I received my B.Eng. and M.S. in Department of Process Equipment and Control Engineering at [Tianjin University](http://www.tju.edu.cn), advised by [Prof. Liyan Liu](http://chemeng.tju.edu.cn/cn/szdw?type=detail&id=52). -->

<i class="fa-solid fa-fw fa-file"></i> Download my <a href="/images/Xiantao_CV.pdf">curriculum vitae</a>.

# <i class="fa-solid fa-fw fa-diagram-project" style="color: #6a4fbf"></i> Research Focus {#research-focus}

### Thrust I: Differentiable Computation for Dynamical Systems

<a href="#" class="show-notice-link" data-target="thrust1-desc" data-display-style="block" data-duration="15000" style="text-decoration:none;">
<figure style="max-width:650px; margin: 1em auto; text-align: center; cursor: pointer;">
  <img src="{{ '/images/research_agenda/thrust1.png' | relative_url }}" style="width:100%; height:auto;">
  <figcaption style="font-size:0.85em; color: var(--text-color-light, #888); margin-top:0.3em;">Click for a short description</figcaption>
</figure>
</a>
<div id="thrust1-desc" class="notice--info" markdown="1" style="display: none; max-width:650px; margin: 0 auto 1em auto;">

A GPU-native differentiable platform for turbulence and FSI. **Diff-FlowFSI** is end-to-end differentiable and roughly 60× faster than conventional CPU-based solvers, extended with differentiable geometry (**Warp-Geo**) for shape and topology optimization, a multigrid-based differentiable sparse linear solver (**JAX-AMG**), and, in a manufacturing setting, coupled electrochemical machining (**JAX-ECM**).

</div>

### Thrust II: Learning Within Physics-Based Solvers

<a href="#" class="show-notice-link" data-target="thrust2-desc" data-display-style="block" data-duration="15000" style="text-decoration:none;">
<figure style="max-width:650px; margin: 1em auto; text-align: center; cursor: pointer;">
  <img src="{{ '/images/research_agenda/thrust2.png' | relative_url }}" style="width:100%; height:auto;">
  <figcaption style="font-size:0.85em; color: var(--text-color-light, #888); margin-top:0.3em;">Click for a short description</figcaption>
</figure>
</a>
<div id="thrust2-desc" class="notice--info" markdown="1" style="display: none; max-width:650px; margin: 0 auto 1em auto;">

Neural networks embedded inside differentiable solvers and trained end-to-end, *a posteriori*, through the dynamics they serve rather than against static labels. This yields hybrid numerical schemes, jointly learned turbulence closures, and generative models of spatiotemporal flow fields that stay stable and generalizable outside their training range.

</div>

### Thrust III: Fluid–Structure Interaction, from Mechanism to Deployment

<a href="#" class="show-notice-link" data-target="thrust3-desc" data-display-style="block" data-duration="15000" style="text-decoration:none;">
<figure style="max-width:650px; margin: 1em auto; text-align: center; cursor: pointer;">
  <img src="{{ '/images/research_agenda/thrust3.png' | relative_url }}" style="width:100%; height:auto;">
  <figcaption style="font-size:0.85em; color: var(--text-color-light, #888); margin-top:0.3em;">Click for a short description</figcaption>
</figure>
</a>
<div id="thrust3-desc" class="notice--info" markdown="1" style="display: none; max-width:650px; margin: 0 auto 1em auto;">

Wind-tunnel experiments, reduced-order models, and differentiable simulation reveal the mechanisms of flow-induced vibration in multi-body systems, translated into control strategies—meta-surfaces, helical strakes—deployed on real systems: marine risers, towers, heat exchangers, pressure vessels, and flow-energy harvesters.

</div>

### Future Directions

<figure style="max-width:650px; margin: 1em auto; text-align: center;">
  <img src="{{ '/images/research_agenda/future.png' | relative_url }}" style="width:100%; height:auto;">
</figure>

Looking ahead, I aim to grow this into a fully differentiable multiphysics pipeline—coupling structural, thermal, and other fields with the flow—and embed learned coarse-graining that stays stable outside its training regime, enabling fast, physically faithful prediction and design at scales beyond conventional high-fidelity solvers. I will extend these tools from analyzing FSI to designing autonomous systems whose behavior is inseparable from the flow around them (bio-inspired robots, autonomous vehicles), and build an agentic AI layer that reasons over the solver's gradients to steer design, calibration, and control—making simulation, learning, and design one differentiable whole.
