---
title: 'The BECCAL Experiment Design and Control Software'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - Arnau Prat
  - Jan Sommer,
  - admin
  - Tobias Franz
  - Hauke Muentinga
  - Andreas Gerndt
  - Daniel Luedtke

# Author notes (optional)
author_notes:
  - 'Equal contribution'
  - 'Equal contribution'

date: '2021-03-06T00:00:00Z'
doi: '10.1109/AERO50100.2021.9438129'

# Schedule page publish date (NOT publication's date).
publishDate: '2021-06-07T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
publication: In *2021 IEEE Aerospace Conference*
publication_short: In *AERO 2021*

abstract: 'This paper presents the software responsible for the design and execution of the experiments in the Bose-Einstein Condensate and Cold Atom Laboratory (BECCAL)mission, an experiment with ultra-cold and condensed atoms on the International Space Station. The software consists of two parts: the experiment control software and the experiment design tools. The first corresponds to the software running on the payload and is in charge of controlling and executing the experiments, while the latter are the tools used by the scientists to create the experiment definition that will be later uploaded to the instrument to be executed. To overcome the challenge of developing software with such complexity, it was decided to follow a model-driven development approach. Several domain-specific languages (DSLs) have been created to allow scientists to describe their experiments in a domain-specific way. These descriptions are then uploaded and executed by different interpreters onboard. The paper details the architecture of the experiment control software and the different modules that compose it, as well as the developed languages and tools used to describe new experiments. The paper also discusses and evaluates some important aspects of the software, such as how resilient it is to failures, as well as the advantages and disadvantages of the selected approach compared to other approaches used in similar missions. The developed software will also be used for the MAIUS-2/3 missions.'

# Summary. An optional shortened abstract.
summary: 'This paper details the software architecture for the BECCAL mission on the ISS developed using a model-driven development approach and domain-specific languages.'

tags:
  - BECCAL
  - Bose-Einstein-Condensate
  - Flight Software

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://elib.dlr.de/142735/1/paper.pdf'
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

