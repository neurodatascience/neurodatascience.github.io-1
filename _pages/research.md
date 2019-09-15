---
title: "NetNeuroLab - Research"
layout: textlay
excerpt: "NetNeuroLab - Research"
sitemap: false
permalink: /research/
---

# Research


{% assign number_printed = 0 %}
{% for proj in site.data.projlist %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if proj.highlight == 1 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
 <div class="well">
  <projtit>{{ proj.title }}</projtit>
  <img src="{{ site.url }}{{ site.baseurl }}/images/pubpic/{{ proj.image }}" class="img-responsive" width="33%" style="float: left" />
  <p>{{ proj.description }}</p>
  <p><em>{{ proj.authors }}</em></p>
  <p><strong><a href="{{ proj.link.url }}">{{ proj.link.display }}</a></strong></p>
  <p class="text-danger"><strong> {{ proj.news1 }}</strong></p>
  <p> {{ proj.news2 }}</p>
 </div>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endif %}
{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<p> &nbsp; </p>






![]({{ site.url }}{{ site.baseurl }}/images/respic/layers_real.jpg){: style="width: 300px; border: 10px"}

**NETWORK COMMUNICATION**

A fundamental question in connectomics is how the organization of brain networks supports neural signalling. Using anatomically realistic networks derived from diffusion weighted imaging (DWI), we develop analytic and computational models of communication, diffusion and spreading. We use these models to characterize how communication processes unfold on structural brain networks and to individual differences in cognitive performance.

**NETWORK TRANSPORT**

Axonal fibers provide a scaffold through which misfolded pathogenic proteins spread, shaping the course and expression of neurodegenerative diseases such as Parkinson’s (PD) and Alzheimer’s (AD) disease.  We are developing generative models that integrate connectivity (diffusion MRI), co-activation (functional MRI) and genetics (mRNA transcription patterns) to predict neurodegenerative spread in PD and AD. These dynamic agent-based models simulate the propagation of pathogenic protein molecules (agents) along white matter fibers.

![]({{ site.url }}{{ site.baseurl }}/images/respic/layers_real.jpg){: style="width: 300px; align-left; border: 10px"}

**ANNOTATED NETWORKS**

Brain regions differ markedly in terms of their cytoarchitecture, receptor distributions, gene expression, temporal dynamics, etc. We are therefore constructing “annotated” connectomes, enriched with local node information. The goal of this work is to understand how microscopic properties and macroscale network embedding interact to support the emergence of global dynamics and patterned neural activity.

**STATISTICAL CONNECTOMICS**

An emerging theme in network neuroscience emphasizes representations and models that not only embody the topological organization of the brain, but also capture the complex multi-scale relationships that link brain topology to its origins in genetics and development, and to the rich cognitive-behavioural repertoire it supports. We develop high-dimensional statistical models that map brain network organization to  phenotypic variation in healthy and clinical populations.
