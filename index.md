# <center> Video-to-Audio Generation with Fine-grained Temporal Semantics</center>
<br>
## Abstract
<div style="text-align: justify"> With recent advances of AIGC, video generation have gained a surge of research interest in both academia and industry (e.g., Sora). However, it remains a challenge to produce temporally aligned audio to synchronize the generated video, considering the complicated semantic information included in the latter. In this work, inspired by the recent success of text-to-audio (TTA) generation, we first investigate the video-to-audio (VTA) generation framework based on latent diffusion model (LDM). Similar to latest pioneering exploration in VTA, our preliminary results also show great potentials of LDM in VTA task, but it still suffers from sub-optimal temporal alignment. To this end, we propose to enhance the temporal alignment of VTA with frame-level semantic information. With the recently popular grounding segment anything model (Grounding SAM), we can extract the fine-grained semantics in video frames to enable VTA to produce better-aligned audio signal. Extensive experiments demonstrate the effectiveness of our system on both objective and subjective evaluation metrics, which shows both better audio quality and fine-grained temporal alignment.</div> 

<br>

![arch](images/vta-sam.png)

<br>

## Video-to-Audio Generation Results

<br>
<table align="center">
  <thead>
    <tr>
      <th>System</th>
      <th>Racing Car</th>
      <th>Popping Popcorn</th>
    </tr>
  </thead>
  <tbody>
    
   <tr>
    <td>GT </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/1-gt.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/2-gt.mp4"></video></td>
   </tr>
   <tr>
      <td>Tango </td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/1-1.mp4"></video></td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/2-1.mp4"></video></td>
   </tr>
   <tr>
   <td>Diff-Foley </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/1-2.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/2-2.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-LDM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/1-3.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/2-3.mp4"></video></td>
   </tr>
   <tr>
    <td>FoleyCrafter </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/1-4.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/2-4.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-SAM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/1-5.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/2-5.mp4"></video></td>
   </tr>
  </tbody>
</table>

<br>
<table align="center">
  <thead>
    <tr>
      <th>System</th>
      <th>Pigeon Dove Cooing</th>
      <th>Dog Bow-wow</th>
    </tr>
  </thead>
  <tbody>
    
   <tr>
    <td>GT </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/10-gt.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/11-gt.mp4"></video></td>
   </tr>
   <tr>
      <td>Tango </td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/10-1.mp4"></video></td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/11-1.mp4"></video></td>
   </tr>
   <tr>
   <td>Diff-Foley </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/10-2.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/11-2.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-LDM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/10-3.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/11-3.mp4"></video></td>
   </tr>
   <tr>
    <td>FoleyCrafter </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/10-4.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/11-4.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-SAM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/10-5.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/11-5.mp4"></video></td>
   </tr>
  </tbody>
</table>

<br>
<table align="center">
  <thead>
    <tr>
      <th>System</th>
      <th>Canary Calling</th>
      <th>Playing Badmintonn</th>
    </tr>
  </thead>
  <tbody>
    
   <tr>
    <td>GT </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/3-gt.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/5-gt.mp4"></video></td>
   </tr>
   <tr>
      <td>Tango </td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/3-1.mp4"></video></td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/5-1.mp4"></video></td>
   </tr>
   <tr>
   <td>Diff-Foley </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/3-2.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/5-2.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-LDM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/3-3.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/5-3.mp4"></video></td>
   </tr>
   <tr>
    <td>FoleyCrafter </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/3-4.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/5-4.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-SAM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/3-5.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/5-5.mp4"></video></td>
   </tr>
  </tbody>
</table>

<br>
<table align="center">
  <thead>
    <tr>
      <th>System</th>
      <th>Chicken Crowing</th>
      <th>Playing Harpsichord</th>
    </tr>
  </thead>
  <tbody>
    
   <tr>
    <td>GT </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/6-gt.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/7-gt.mp4"></video></td>
   </tr>
   <tr>
      <td>Tango </td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/6-1.mp4"></video></td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/7-1.mp4"></video></td>
   </tr>
   <tr>
   <td>Diff-Foley </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/6-2.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/7-2.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-LDM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/6-3.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/7-3.mp4"></video></td>
   </tr>
   <tr>
    <td>FoleyCrafter </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/6-4.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/7-4.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-SAM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/6-5.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/7-5.mp4"></video></td>
   </tr>
  </tbody>
</table>

<br>
<table align="center">
  <thead>
    <tr>
      <th>System</th>
      <th>Playing Clarinet</th>
      <th>Ferret Dooking</th>
    </tr>
  </thead>
  <tbody>
    
   <tr>
    <td>GT </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/8-gt.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/gt/9-gt.mp4"></video></td>
   </tr>
   <tr>
      <td>Tango </td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/8-1.mp4"></video></td>
      <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/tango/9-1.mp4"></video></td>
   </tr>
   <tr>
   <td>Diff-Foley </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/8-2.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/diff-foley/9-2.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-LDM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/8-3.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-ldm/9-3.mp4"></video></td>
   </tr>
   <tr>
    <td>FoleyCrafter </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/8-4.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/foleycrafter/9-4.mp4"></video></td>
   </tr>
   <tr>
    <td>VTA-SAM </td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/8-5.mp4"></video></td>
     <td><video style="height: 200px; width: auto;" controls="" preload="auto">
            <source src="videos/vta-sam/9-5.mp4"></video></td>
   </tr>
  </tbody>
</table>

