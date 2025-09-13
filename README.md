<a id="top"></a>

# Multi-segment Soft Robot Control via  
**Deep Koopman-based Model Predictive Control (DK-MPC)**

**Authors:**  
Lei Lv<sup>1,2</sup>, Lei Liu<sup>2,3</sup>, Lei Bao<sup>3,4</sup>, Fuchun Sun<sup>2</sup>, Jiahong Dong<sup>5</sup>, Jianwei Zhang<sup>6</sup>, Xuemei Shan<sup>4</sup>, Kai Sun<sup>2,3</sup>, Hao Huang<sup>7</sup>, Yu Luo<sup>2</sup>

**Affiliations:**  
<sup>1</sup> Shanghai Research Institute for Intelligent Autonomous Systems, Tongji University  
<sup>2</sup> Department of Computer Science and Technology, Tsinghua University  
<sup>3</sup> School of Biomedical Engineering, Tsinghua University  
<sup>4</sup> Beijing Soft Robot Tech Co., Ltd  
<sup>5</sup> School of Clinical Medicine, Tsinghua University  
<sup>6</sup> Department of Informatics, University of Hamburg  
<sup>7</sup> School of Mechanical Engineering and Automation, Beihang University

---

## Abstract

Soft robots, compared to regular rigid robots, as their multiple segments with soft materials bring flexibility and compliance, have the advantages of safe interaction and dexterous operation in the environment. However, due to its characteristics of high dimensional, nonlinearity, time-varying nature, and infinite degree of freedom, it has been challenges in achieving precise and dynamic control such as trajectory tracking and position reaching. To address these challenges, we propose a framework of Deep Koopman-based Model Predictive Control (DK-MPC) for handling multi-segment soft robots. We first employ a deep learning approach with sampling data to approximate the Koopman operator, which therefore linearizes the high-dimensional nonlinear dynamics of the soft robots into a finite-dimensional linear representation. Secondly, this linearized model is utilized within a model predictive control framework to compute optimal control inputs that minimize the tracking error between the desired and actual state trajectories. The real-world experiments on the soft robot “Chordata” demonstrate that DK-MPC could achieve high-precision control, showing the potential of DK-MPC for future applications to soft robots.

---

## The proposed DK-MPC architecture

![DK-MPC architecture](Figures/dkmpc2.png)  
*DK-MPC architecture.*

---

## Framework for Learning Koopman Operators

![Framework for learning Koopman operators](Figures/framework.png)

---

## Design of soft robot “Chordata”

![Design of soft robot "Chordata"](Figures/design.png)

---

## Experiments on soft robot “Chordata”

### Moving target tracking (1×)

<video src="Videos/trackingfront.mp4" controls loop muted width="720">
  Your browser does not support the video tag.
</video>  
[Download video](Videos/trackingfront.mp4)

---

### Path tracking (10×)

> For accurate video alignment, please refresh the page prior to playback.

<table>
  <tr>
    <td align="center">
      <video src="Videos/t2.mp4" controls loop muted width="320"></video><br/>
      <sub>t2</sub><br/>
      <a href="Videos/t2.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/h2.mp4" controls loop muted width="320"></video><br/>
      <sub>h2</sub><br/>
      <a href="Videos/h2.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/u2.mp4" controls loop muted width="320"></video><br/>
      <sub>u2</sub><br/>
      <a href="Videos/u2.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/o2.mp4" controls loop muted width="320"></video><br/>
      <sub>o2</sub><br/>
      <a href="Videos/o2.mp4">Download</a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center">
      <video src="Videos/t2fig.mp4" controls loop muted width="320"></video><br/>
      <sub>t2 (fig)</sub><br/>
      <a href="Videos/t2fig.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/h2fig.mp4" controls loop muted width="320"></video><br/>
      <sub>h2 (fig)</sub><br/>
      <a href="Videos/h2fig.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/u2fig.mp4" controls loop muted width="320"></video><br/>
      <sub>u2 (fig)</sub><br/>
      <a href="Videos/u2fig.mp4">Download</a>
    </td>
    <td align="center">
      <video src="Videos/o2fig.mp4" controls loop muted width="320"></video><br/>
      <sub>o2 (fig)</sub><br/>
      <a href="Videos/o2fig.mp4">Download</a>
    </td>
  </tr>
</table>

---

### Path tracking (figure)

![Path tracking](Figures/THU3.png)

---

### Moving target tracking (figure)

![Moving target tracking](Figures/fig9.png)

---

## Video (full)

<video src="Videos/video.mp4" controls loop muted width="1000">
  Your browser does not support the video tag.
</video>  
[Download video](Videos/video.mp4)

---

<p align="right"><a href="#top">Back to top ↑</a></p>
