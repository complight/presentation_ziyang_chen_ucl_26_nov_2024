---
favicon: /complight.png
titleTemplate: '%s - Computational Light Laboratory'
# You can also start simply with 'default'
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: black
# some information about your slides (markdown enabled)
title: Advanced Holographic Imaging Systems for 3D Vision and Immersive Display Applications
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center text-white
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# take snapshot for each slide in the overview
overviewSnapshots: true
# keywords field for exported PDF, comma-delimited
keywords: computational imaging, holography
css: ./style.css

---

# Advanced Holographic Imaging Systems for 3D Vision and Immersive Display Applications

Presenter: Ziyang Chen

Supervised by Dr. Kaan Akşit and Dr. He Wang

Nov 27th, 2024, London
<div style="position: absolute; bottom: 50px; right: 30px;">
  <img src="/lab_logo.png" alt="lab_logo" width="200" height="600">
</div>


<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

<style>
/* Custom CSS for header sizing */
h1 {
  font-size: 2em !important; /* Smaller size for main headers */
}

</style>



---
transition: fade-out
class: text-white
---

<!-- <div v-clicks class="mr-8">
  <h2 class="text-blue-400 mb-6 text-3xl font-semibold">Fourier Optics</h2>
  <div class="space-y-4 ml-4 text-xl">
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-blue-400"></div>
      <span>Fourier transform</span>
    </div>
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-blue-400"></div>
      <span>Linear system</span>
    </div>
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-blue-400"></div>
      <span>Light propagation</span>
    </div>
  </div>
</div>
<div v-after style="position: absolute; bottom: 50px; right: 660px;">
    <div class="w-64 h-64 overflow-hidden">
      <img src="/light_propagation.jpg" alt="sensor" class="w-full h-full object-cover">
    </div>
    <p style="position: absolute; bottom: -60px; right: 10px; font-size: 0.6em; color: #888;">
      "<a rel="noopener noreferrer" href="https://www.flickr.com/photos/14341815@N00/4174879359">Christmas Tree Lights Bokeh</a>" by 
      <a rel="noopener noreferrer" href="https://www.flickr.com/photos/14341815@N00">Sprogz</a> is licensed under 
      <a rel="noopener noreferrer" href="https://creativecommons.org/licenses/by/2.0/?ref=openverse">CC BY 2.0 
      <img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" />
      <img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" /></a>
    </p>
</div> -->

<div class="ml-8">
  <h2 class="text-purple-400 mb-6 text-3xl font-semibold">Lensless camera</h2>
  <div class="space-y-4 ml-4 text-xl">
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-purple-400"></div>
      <span>System Structure</span>
    </div>
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-purple-400"></div>
      <span>Applications</span>
    </div>
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-purple-400"></div>
      <span>Forward model</span>
    </div>
    <div class="flex items-center gap-3 text-gray-300 hover:text-white transition-colors">
      <div class="w-2 h-2 rounded-full bg-purple-400"></div>
      <span>Reconstruction Algorithms</span>
    </div>
  </div>
</div>



<div v-after style="position: absolute; bottom: 50px; right: 100px;">
  <div class="w-100 h-100 overflow-hidden">
    <img src="/image_sensor.jpg" alt="sensor" class="w-full h-full object-cover">
  </div>
  <p style="position: absolute; bottom: -60px; right: 10px; font-size: 0.6em; color: #888;">
  "<a rel="noopener noreferrer" href="https://www.flickr.com/photos/38365223@N03/8721197656">Reflection in image sensor</a>" by 
  <a rel="noopener noreferrer" href="https://www.flickr.com/photos/38365223@N03">Steys</a> is licensed under 
  <a rel="noopener noreferrer" href="https://creativecommons.org/licenses/by-sa/2.0/?ref=openverse">CC BY-SA 2.0 
  <img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" />
  <img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" />
  <img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" /></a>
</p>
</div>

<div v-click style="position: absolute; bottom: 50px; right: 100px;">
  <div class="w-100 h-100 overflow-hidden">
    <img src="/image_sensor_w_box.png" alt="sensor" class="w-full h-full object-cover">
  </div>
  <p style="position: absolute; bottom: -60px; right: 10px; font-size: 0.6em; color: #888;">
  "<a rel="noopener noreferrer" href="https://www.flickr.com/photos/38365223@N03/8721197656">Reflection in image sensor</a>" by 
  <a rel="noopener noreferrer" href="https://www.flickr.com/photos/38365223@N03">Steys</a> is licensed under 
  <a rel="noopener noreferrer" href="https://creativecommons.org/licenses/by-sa/2.0/?ref=openverse">CC BY-SA 2.0 
  <img src="https://mirrors.creativecommons.org/presskit/icons/cc.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" />
  <img src="https://mirrors.creativecommons.org/presskit/icons/by.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" />
  <img src="https://mirrors.creativecommons.org/presskit/icons/sa.svg" style="height: 0.8em; margin-right: 0.125em; display: inline;" /></a>
</p>
</div>

---
transition: fade
class: text-white
layout: default
---

# Imaging system Structure

<div class="text-center">
 Conventional imaging system
</div>
<div v-after style="position: absolute; left: 50%; bottom: 80px; transform: translateX(-50%);">
  <img src="/conventional.png" alt="sensor" class="w-130 h-auto object-cover">
  <br>
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
<a href="https://commons.wikimedia.org/wiki/File:Ccd-sensor.jpg">C-M</a>, <a href="http://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a>, via Wikimedia Commons

</p>



---
transition: fade
class: text-white
layout: default
---

# Imaging system Structure

<div v-after style="position: absolute; left: 50%; bottom: 80px; transform: translateX(-50%);">
  <img src="/no_lens.png" alt="sensor" class="w-130 h-auto object-cover">
  <br>
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
<a href="https://commons.wikimedia.org/wiki/File:Ccd-sensor.jpg">C-M</a>, <a href="http://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a>, via Wikimedia Commons

</p>

---
transition: fade
class: text-white
layout: default
---

# Imaging system Structure
<div class="text-center">
 Lensless imaging system
</div>
<div v-after style="position: absolute; left: 50%; bottom: 80px; transform: translateX(-50%);">
  <img src="/lensless_system.png" alt="sensor" class="w-130 h-auto object-cover">
  <br>
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
<a href="https://commons.wikimedia.org/wiki/File:Ccd-sensor.jpg">C-M</a>, <a href="http://creativecommons.org/licenses/by-sa/3.0/">CC BY-SA 3.0</a>, via Wikimedia Commons

</p>
---
transition: fade-out
class: text-white
layout: default
---

# Why?

<div class="text-2xl font-semibold" style="position: center;">
 <span class="text-red-500">Complex optics</span> & <span class="text-red-500">large form factor</span>
</div>
<br>
<div v-click="1" style="position: absolute; left: 50%; bottom: 50px; transform: translateX(-50%); background-color: white; padding: 1rem; border-radius: 8px;">
 <img src="/camera_slice.png" alt="sensor" class="w-130 h-auto object-cover">
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
 <a href="https://commons.wikimedia.org/wiki/File:Reflex_camera_simple_labels.svg">Astrocog</a>, <a href="https://creativecommons.org/licenses/by-sa/3.0">CC BY-SA 3.0</a>, via Wikimedia Commons
</p>


---
transition: fade-out
class: text-white
layout: default
---

# Why?

<div  class="text-2xl font-semibold" style="position: center;">
 <span class="text-red-500">Thick lens</span> 
</div>

<div style="position: absolute; left: 50%; bottom: 50px; transform: translateX(-50%); background-color: white; padding: 1rem; border-radius: 8px;">
  <img src="/iphone.jpg" alt="sensor" class="w-110 h-auto object-cover">
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
  <a href="https://commons.wikimedia.org/wiki/File:IPhone_13_Pro_camera_lens_group.jpg">人工知能</a>, <a href="https://creativecommons.org/licenses/by-sa/4.0">CC BY-SA 4.0</a>, via Wikimedia Commons
</p>


---
transition: fade-out
class: text-white
layout: default
---

# Why?

<div class="text-2xl font-semibold" style="position: center;">
 <span class="text-red-500">Single purpose</span> & <span class="text-red-500">Visual privacy</span>
</div>

<div style="position: absolute; left: 50%; bottom: 50px; transform: translateX(-50%); background-color: white; padding: 1rem; border-radius: 8px;">
  <img src="/quest.jpg" alt="sensor" class="w-110 h-auto object-cover">
</div>
<p style="position: absolute; bottom: 0px; right: 5%; font-size: 0.6em; color: #888;">
  <a href="https://commons.wikimedia.org/wiki/File:Meta_Quest_3_display_unit.jpg">IHazACatNamedMax</a>, <a href="https://creativecommons.org/licenses/by-sa/4.0">CC BY-SA 4.0</a>, via Wikimedia Commons
</p>

---
transition: fade-out
class: text-white
layout: default
---

# Lensless Camera Applications

<br>

## Microscopy

<div class="flex flex-col h-full ">
  <div class="flex items-center justify-center" style="background-color: white; padding: 0.2rem; border-radius: 8px;">
    <img src="/microscopy.png" class="w-150" alt="Lensless Camera">
  </div>

  <div class="text-sm text-gray-500 mb-6" style="font-size: 0.5em;">
    [G. Kuo, F. L. Liu, I. Grossrubatscher, R. Ng, and L. Waller, “On-chip
fluorescence microscopy with a random microlens diffuser,” Opt.
Express 28, 8384–8399 (2020).]
  </div>

  <div class="text-sm text-gray-500 mb-6" style="font-size: 0.5em;">
  [V. Boominathan, J. K. Adams, J. T. Robinson, and A. Veeraraghavan, “PhlatCam: designed phase-mask based thin lensless camera,” IEEE Trans. Pattern Anal. Mach. Intell. 42, 1618–1629 (2020).]
  </div>
</div>

---
transition: fade-out
class: text-white
layout: default
---

# Lensless Camera Applications

<br>

## Thermal imaging

<div class="flex flex-col h-full ">
  <div class="flex items-center justify-center" style="background-color: white; padding: 0.2rem; border-radius: 8px;">
    <img src="/thermal_imaging.png" class="w-180" alt="Lensless Camera">
  </div>

  <div class="text-sm text-gray-500 mb-6" style="font-size: 0.5em;">
    [. I. Reshetouski, H. Oyaizu, K. Nakamura, R. Satoh, S. Ushiki, R. Tadano, A. Ito, and J. Murayama, “Lensless imaging with focusing sparse URA masks in long-wave infrared and its application for human detection,” in Lecture Notes in Computer Science (including subseries Lecture Notes in Artificial Intelligence and Lecture Notes in Bioinformatics)(2020), Vol. 12364 LNCS, pp. 237–253.]
  </div>
</div>

---
transition: fade-out
class: text-white
layout: default
---

# Lensless Camera Applications

<br>

## 3D imaging

<div class="flex flex-col h-full ">
  <div class="flex items-center justify-center" style="background-color: white; padding: 0.2rem; border-radius: 8px;">
    <img src="/3d_imaging.png" class="w-100" alt="Lensless Camera">
  </div>

  <div class="text-sm text-gray-500 mb-6" style="font-size: 0.5em;">
    [N. Antipa, G. Kuo, R. Heckel, B. Mildenhall, E. Bostan, R. Ng, and L.Waller, “DiffuserCam: lensless single-exposure 3D imaging,” Optica 5, 1–9 (2018).]
  </div>
</div>

---
transition: fade-out
class: text-white
layout: default
---

# 3D vision - tracking
<br>

- Precision pose detection is demanded in personal fabrication, VR, and robotics.
- Conventional vision-based systems used in these systems often struggle with achieving high precision and accuracy
---
transition: fade-out
class: text-white
layout: default
---

# Speckle 

<br>
<br>

<div class="flex flex-col items-center justify-center">
  <img src="/speckle_0.png" class="w-180" alt="Lensless Camera">
  <p class="text-sm text-white-600 mt-2 italic">Holographic phenomenon where the phase and amplitude are random.</p>
</div>

---
transition: fade
class: text-white
layout: default
---

# Speckle 

<br>
<br>

<div class="flex flex-col items-center justify-center">
  <img src="/speckle_1.png" class="w-120" alt="Lensless Camera">
  <p class="text-sm text-white-600 mt-2 italic">Simplified forward propagation of the laser light.</p>
</div>

---
transition: fade
class: text-white
layout: default
---

# SpecTrack 

<br>
<br>

<div class="flex flex-col items-center justify-center">
  <img src="/speckle_2.png" class="w-120" alt="Lensless Camera">
  <p class="text-sm text-white-600 mt-2 italic">Information encoded in the speckle pattern.</p>
</div>

---
transition: fade-out
class: text-white
layout: center
---

<video width="800" controls autoplay>
  <source src="/demo.mp4" type="video/mp4">
</video>

---
transition: fade
class: text-white
layout: default
---

# Next

- Utilize this imaging system in immersive display systems
- Explore new 