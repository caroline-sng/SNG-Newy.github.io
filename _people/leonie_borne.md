---
title: Léonie Borne
auto-header: none
icon: fa-tree
order: 3
---

<head>
<style>
img.portrait {
  border-radius: 50%;
  width: 300px;
  border: 1px solid #ddd;
  padding: 5px;
}
.row {
  display: flex;
  justify-content: center;
}
</style>
</head>

<section>
  <div class="row">
  {% for person in site.team.people %}
	{% if person.initials == "LB" %}
	  <div class="col">
		<img class="portrait" src="{{ person.image }}" alt="">
	  </div> 
	  <div class="col">
	      <h2> {{person.name}} </h2>
              <h3> {{ person.role }} </h3>
		 {{ person.research_interest | markdownify }}
		 <ul class="icons">
		{% for network in person.social %}
		  <li><a href="{{- network.url -}}" class="{{ network.icon }} fa-2x"></a></li>
		{% endfor %}
		</ul>
	  </div> 
	{% endif %}
  {% endfor %}
  </div>
</section>

## Research Interests
I am passionate about the use of artificial intelligence in medical imaging. 
My work aims to develop intelligent algorithms to help the analysis of these images, notably using deep learning. 

## Deep learning for cortical fold study
After a master's degree in artificial intelligence, I did my PhD at Neurospin in France. 
My PhD work focused on the development of several **structural MRI analysis** pipelines using **machine learning** algorithms, including **deep learning**. 
The tools I developed are now available in the BrainVISA toolbox ([www.brainvisa.info](www.brainvisa.info)), to help researchers study the link between the fold shape and brain function. 

## Brain-behaviour association in dementia
Following my PhD, I started a postdoc in 2020 in the Systems Neuroscience Group where I applied my skills to address the challenges of dementia. 
Using **advanced statistical analysis**, I have notably identified a robust association between brain atrophy and cognitive decline during the **preclinical stage of Alzheimer's disease**. 
My work is based on the databases [ADNI](http://adni.loni.usc.edu/), [AIBL](https://aibl.csiro.au/) and [PISA](https://www.qimrberghofer.edu.au/pisa/).

