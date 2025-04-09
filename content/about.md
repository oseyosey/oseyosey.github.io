---
title: "About"
---


<head>
    <style>
        .container {
            align: left; /* Aligns content of the container to the left */
        }
        .container img {
            width: 330px; /* Adjust this value to scale the image */
            margin-left: -5.5%; 
        }
    </style>
</head>

<!-- <img src="assets/photo_id_website.png" alt="" /> -->

<div class="container">
    <img src="/photo_id_website.png" align="left">
</div>

## Hi, I'm Junjie Oscar Yin

I conduct research in natural language processing and machine learning. 

I am an incoming PhD student at UW NLP, advised by [Hannaneh Hajishirzi](https://homes.cs.washington.edu/~hannaneh/).

Currently, I am fortunate to be collaborating with [Sasha Rush](https://rush-nlp.com/). 

In my undergraduate years at Johns Hopkins, I am grateful to be advised by [Alan Yuille](https://www.cs.jhu.edu/~ayuille/) and supported by the [Westgate Scholarship](https://apply.jhu.edu/tuition-aid/types-of-financial-aid/need-based-scholarships/westgate-scholarship/). During my studies, I spent a year at University of Oxford, where I had the privilege of being mentored by [Michael Wooldridge](https://www.cs.ox.ac.uk/people/michael.wooldridge/). 

<!-- 
I'm a Research Scientist at the [Flatiron
Institute](https://www.simonsfoundation.org/flatiron/)'s [Center for
Computational
Astrophysics](https://www.simonsfoundation.org/flatiron/center-for-computational-astrophysics/).
My main research interest is the application of probabilistic data analysis
techniques to solve fundamental problems in astronomy. These days, I'm mostly
using time domain surveys to discover new exoplanets, interpret the underlying
population of these planets, and learn more about the variability of stars. I am
also interested in the development of scientific software and open-source
practices. -->


### Publications

My list of publications is available here:


- Compute-Constrained Data Selection.\
***Junjie Oscar Yin**, Alexander M. Rush.* \
*International Conference on Learning Representations (ICLR), 2025.* \
<sup>[<a href="https://arxiv.org/abs/2410.16208">Paper</a>]</sup> <sup>[<a href="https://github.com/oseyosey/CCDS">Codebase</a>]</sup> <sup>[<a href="https://www.youtube.com/watch?v=D5bHngvcQU4&t=787s">Talk</a>]</sup> 


- ModuLoRA: Finetuning 2-Bit LLMs on Consumer GPUs by Integrating with Modular Quantizers.\
***Junjie Oscar Yin**, Jiahao Dong, Yingheng Wang, Christopher De Sa, Volodymyr Kuleshov.* \
*Transactions on Machine Learning Research (TMLR), 2024. (**Featured Paper** ; Invited to ICLR 2024)* \
 <sup>[<a href="https://openreview.net/forum?id=r9p9CV52MV">Paper</a>]</sup> <sup>[<a href="https://github.com/kuleshov-group/llmtools">Codebase</a>]</sup> <sup>[<a href="https://oseyincs.io/llmtools/">Blog Post</a>]</sup> 


- EasyRet3D: Uncalibrated Multi-view Multi-Human 3D Tracking and Reconstruction.\
***Junjie Oscar Yin**, Ting Li, Jiahao Wang, Yi Zhang, Alan Yuille.*\
*Winter Conference on Applications of Computer Vision (WACV), 2025.* \
 <sup>[<a href="https://drive.google.com/file/d/1sD4FnnmsWsr38G5RkX6-rKMJT5Qn0Thn/view?usp=sharing">Paper</a>]</sup> <sup>[<a href="https://ez3dtrackmv.org/">Project Site</a>]</sup>


- How LLM-powered Conversational Agents Influence Decision Making in Domestic Medical Triage Contexts.\
\*Catalina Gomez, *\***Junjie Oscar Yin**, Chien-Ming Huang, Mathias Unberath.* \
*Frontiers in Computer Science, 2024.* \
<sup>[<a href="https://www.frontiersin.org/journals/computer-science/articles/10.3389/fcomp.2024.1427463/full">Paper</a>]</sup>



### Recent Updates

Below you will find the most recent updates:

- 2024 Computing Research Association's (<a href="https://cra.org/">CRA</a>) Outstanding Undergraduate Researcher Award (<a href="https://cra.org/crae/awards/cra-outstanding-undergraduate-researchers/">URA</a>). *Dec 2023.*


<!-- ### Code

I write a lot of code for work and in my spare time. All my projects live in
[public repositories on GitHub](https://github.com/dfm). Here are some of my most popular research codes:

<script id="code-template" type="x-tmpl-mustache">
{{#codes}}
<li>
    <i><a href="{{homepageUrl}}">{{name}}</a></i> &mdash; {{description}}
</li>
{{/codes}}
{{^codes}}
Unable to load of software.
{{/codes}}
</script>

<ul id="codelist"></ul> -->

<!-- [on ADS](http://adsabs.harvard.edu/cgi-bin/nph-abs_connect?return_req=no_params&author=Foreman-Mackey&db_key=PRE)
but here are a few highlights: -->

<!-- <script id="pub-template" type="x-tmpl-mustache">
{{#pubs}}
<li>
    {{authorsFormat}}, {{year}}, <a href="{{url}}"><i>{{title}}</i></a>.
    {{#codeLink}}<br><small>[<a href="{{codeLink}}">code</a>]</small>{{/codeLink}}
</li>
{{/pubs}}
{{^pubs}}
Unable to load publication list.
{{/pubs}}
</script> -->




<ul id="publist"></ul>

<script src="https://unpkg.com/mustache@latest"></script>

<script>
  var codeMap = {
    "10.1086/670067": "https://github.com/dfm/emcee",
    "10.1088/0004-637X/795/1/64": "https://github.com/dfm/exopop",
    "10.1088/0004-637X/806/2/215": "https://github.com/dfm/ketu",
    "10.21105/joss.00024": "https://github.com/dfm/corner.py",
    "10.3847/0004-6256/152/6/206": "https://github.com/dfm/peerless",
    "10.3847/1538-3881/aa9332": "https://github.com/dfm/celerite",
    "10.3847/2515-5172/aaaf6c": "https://github.com/dfm/celerite-grad",
    "10.21105/joss.01864": "https://github.com/dfm/emcee",
    "10.21105/joss.03285": "https://github.com/exoplanet-dev/exoplanet"
  };

  function formatAuthors(authors) {
    authors = authors.map(author => {
      var tokens = author.split(", ");
      if (tokens.length != 2) return author;
      return tokens[1][0] + ". " + tokens[0];
    });
    if (authors.length == 1) {
      return authors[0];
    } else if (authors.length >= 5) {
      return authors.slice(0, 4).join(", ") + ", et al.";
    }
    return authors.slice(0, authors.length - 1).join(", ") + ", and " + authors[authors.length - 1];
  }

  (() => {
    var codeTemplate = document.getElementById("code-template").innerHTML;
    fetch("https://raw.githubusercontent.com/dfm/cv/main/data/repos.json")
      .then(response => response.json())
      .then(data => {
        data = data.data.user.pinnedItems.edges.map(value => value.node);
        var rendered = Mustache.render(codeTemplate, { codes: data });
        document.getElementById("codelist").innerHTML = rendered;
      })
      .catch(() => {
        var rendered = Mustache.render(codeTemplate, { codes: [] });
        document.getElementById("codelist").innerHTML = rendered;
      });

    var pubTemplate = document.getElementById("pub-template").innerHTML;
    fetch("https://raw.githubusercontent.com/dfm/cv/main/data/pubs.json")
      .then(response => response.json())
      .then(data => {
        // Only first author
        data = data.filter(value => {
          return value.authors[0].startsWith("Foreman-Mackey") && value.doctype == "article";
        });

        // Format authors
        data = data.map(value => {
          value.authorsFormat = formatAuthors(value.authors);
          value.codeLink = codeMap[value.doi];
          value.title = value.title.replace("{\\&}", "&");
          return value;
        });

        var rendered = Mustache.render(pubTemplate, { pubs: data });
        document.getElementById("publist").innerHTML = rendered;
      })
      .catch(() => {
        var rendered = Mustache.render(pubTemplate, { pubs: [] });
        document.getElementById("publist").innerHTML = rendered;
      });
  })();
</script>
