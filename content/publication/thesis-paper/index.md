---
title: 'Modeling and Simulation of a Spacecraft Payload Hardware Using Machine Learning Techniques'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Arnau Prat
  - Kilian Johann Hoeflinger
  - Andreas Gerndt
  - Daniel Luedtke

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

date: '2020-11-16T00:00:00Z'
doi: '10.2514/6.2020-4219'

# Schedule page publish date (NOT publication's date).
publishDate: '2020-11-02T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *Accelerating Space Commerce, Exploration, and New Discovery Conference, ASCEND 2020*
publication_short: In *ASCEND 2020*

abstract: Space systems are complex and consist of multiple subsystems. Research and development teams of such complex systems are usually distributed among various institutions and space agencies. This affects the quality of the On-board Software (OBSW) since testing it without having all required subsystems at the software development site can be troublesome. In this paper, we present a data-driven method which can be used to synthesize parts of a system or even an entire system as a black-box model. We exploit the data collected from the real hardware to derive a model using a Machine Learning (ML) algorithm. The proposed model can easily be distributed among development teams and is dedicated to emulate the system for testing the OBSW.

# Summary. An optional shortened abstract.
summary: Modeling and simulating hardware facilitates seamless integration of the model into CI pipelines, enabling rigorous testing of onboard software without expensive physical hardware in the loop, thereby enhancing efficiency and reducing development time. 

tags:
  - Modeling and Simulation
  - Neural Networks
  - Artificial Intelligence

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://elib.dlr.de/137571/1/ASCEND_full_paper_published.pdf'
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

<!--
{{% callout note %}}
Click the _Cite_ button to download citation.
{{% /callout %}}

{{% callout note %}}
Click the _Slides_ button to download the paper.
{{% /callout %}}
-->

Quality assurance is an integral part of the product life-cycle of any safety critical software, such as On-board Software (OBSW) for aviation and space systems. Modern aerospace systems have a modular structure consisting of several subsystems and components [1]. These components interact with each other to fulfill a common task and ultimately achieve the mission goal. With an increasing number of components and their interactions, the complexity of the system rises [1]. Software that drives such a complex system must be robust and resilient to a wide variety of failures. In order to ensure that all features of the OBSW work as expected, they must be thoroughly tested on the component, the subsystem, and the system level. 

Aerospace projects are often carried out in collaborations between agencies, research institutions, universities, or industries. In such collaborations, the development process of the system gets divided among project partners. Although an agency manufactures a hardware component, for example, it may not develop the accompanying control software. Another institute located in a different location might be responsible for the software components. In such a case, the software integration can be troublesome. In order to properly test communication modules of an OBSW, a Hardware-in-the-Loop (HiL) test environment is necessary, where all required hardware components are present. 

Duplication of the missing hardware for each development site is often unfeasible due to their high complexity and manufacturing cost. When a peripheral hardware is missing, OBSW developers use mock-up methods to mimic the input/output signals of the hardware. Without deep domain knowledge, mock-up methods cannot account for the dynamic behavior of the system. Often, they produce only a random value within a given range or just return a default value. Using mock-up methods in testing the complex software may lead to incorrect test results. OBSW developers have to deal with this kind of shortcomings.

In this paper, we address this problem by presenting a methodology to synthesize a model with the data collected from the real payload hardware using Machine Learning (ML) techniques. The black-box model can be used to communicate with the OBSW on behalf of the real hardware to test the OBSW functionalities. We model the payload hardware along with its environment which includes modeling the behavior of sensors and actuators connected to the device over an extended period of time. We achieve this by reformulating the problem into a time series prediction problem (temporal sequence modeling), so that we can exploit well-studied ML algorithms from the field. Specifically, we explore the state-of-the-art deep learning algorithms from the Recurrent Neural Network (RNN) family.


