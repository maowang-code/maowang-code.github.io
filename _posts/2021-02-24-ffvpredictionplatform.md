---
layout: post
title: Polymer Fractional Free Volume (FFV) prediction platform is online ! 
date: 2022-02-24
comments: true
description: predict the fractional free volume of polymer based on its structure
---

## A brief introduction of FFV of polymers
In polymeric materials, free volume refers to the empty space existing among polymer chains (Figure below).   

<center>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/blog_img/ffv_prediction/fv.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</center>

<center>Graphical representation of free volume in polymers. Holes are evidenced by the red dash. [Source:http://eprints-phd.biblio.unitn.it/2733/1/David_Roilo_Thesis.pdf]
</center>

<br>

To quantitatively measure the free volume, fractional free volume (FFV) (*i.e.*, the percentage of free volume to the whole polymer) is widely used. FFV is regarded as an intrinsic property of polymer materials.   

polymers with high FFV are desired for separation applications. The PIM (polymers of intrinsic microporosity) polymers are one of the most popular high-FFV polymers. The interconnect pores inside PIMs enable PIMs to have extremely high gas permeability which is several orders higher than the traditional gas separation polymers.   

Fast prediction of FFV of polymers on its structure will greatly accelerate the discovery of high FFV polymers. This is what our FFV prediction platform is made for.  

Below, I will introduce the interface of the platform.  
<br>

## Interface

**To use the platform, first, visit the website** [https://ffv-prediction.herokuapp.com](https://ffv-prediction.herokuapp.com)

<center>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/blog_img/ffv_prediction/ffv1.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</center>


<center>Platform interface</center>

### 1. visualization
There are 4 columns on the page and the left 3 columns are used for visualization of the 29,482 screened polymers with predicted FFV > 0.2 in our recent work.   
- You can use the dropdown bar to select the density, van der Waals volume, FFV, SCScore of the polymers. The relationship between those parameters are:  
FFV = 1 - 1.3 density * Vvdw 
- As for SCScore, it is used to evaluate the synthesizability of a molecule (the lower, the easier to synthesize).  
- By clicking a data point in the plot (2nd column), its corresponding polymer structure and selected values will appear in the 3rd column.  
- You can also download the whole Excel files of the 29,482 screened polymers by clicking the Download bottom.

### 2. FFV prediction
One main purpose of the platform is to enable everyone to perform fast FFV prediction on polymer structures.  
in the 4th column, after inputting the SMILES strings of the polymer, its prediction will show up below.  
There are some requirements for the input polymer SMILES strings.  
- It should have two connecting points
- The connecting points are represented by *  

If you are not familiar with the SMILES representation of polymers, you can use the link provided to draw your polymer structures online to generate the SMILES strings.  

<center>
<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/blog_img/ffv_prediction/draw4.png" class="img-fluid rounded z-depth-1" zoomable=true %}
    </div>
</div>
</center>

<center>A Method to generate polymer SMILES </center>  
(In step 4, you should replace [K] with [*])

Now, you can predict the density, van der Waals volume, FFV of polymer of your interests.
**Please enjoy!** :fire:










