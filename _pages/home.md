---
layout: default
permalink: /
title: Home
nav: true
nav_order: 1
img: think.jpg
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 5
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3 # The number of links after the current page
---

<div class="post">

{% assign blog_name_size = site.blog_name | size %}
{% assign blog_description_size = site.blog_description | size %}

  <div class="header-bar">
    <h1>{{ site.blog_name }}</h1>
    <h2>{{ site.blog_description }}</h2>
  </div>

  <div class="tag-category-list">
    <ul class="p-0 m-0">      
        <li>
          <!-- <i class="fa-solid fa-hashtag fa-sm"></i> -->
          Workshop proposed to: <a href="https://www.ro-man2024.org/" target=_blank>roman24</a>
        </li>
          <p>&bull;</p>
          <i class="fa-solid fa-pin fa-sm"></i> <p> 26th August 2024</p>
        <p>&bull;</p>
        <i class="fa fa-place" aria-hidden="true"></i> <p> Pasadena California, USA</p>
    </ul>
  </div>
  

<!-- <div style="text-align: center;"><p><h3>Personalisation in robotics is...</h3></p></div> -->
<!-- <div style="margin-top: -15px; text-align: center;"><p><h3><span id="typing-text"></span></h3></p></div> -->
</div>



<div class="row m-3">
  <div class="col-sm-9">
    <h3>Abstract</h3>
      <p class="main-description">
      The importance of personalisation in Human-Robot Interaction has already shown its advantages in multiple scenarios and will become a prevalent direction for the field.
      Robots are required to adapt their behaviour in both short- and long-term interactions.
      In the short term, as the interactions are very often limited in time, robots need to learn from scratch the user's preferences and adapt quickly to them. In the long term, users' needs may change and robots need to continuously adapt in a way that keeps them engaged and interested over time.
      Personalisation can greatly improve short- and long-term interactions in various real-world scenarios by fostering trust and rapport, increasing adherence to the interaction, enhancing engagement through tailored content, and improving task performance. 
      Nonetheless, it is essential to consider whether and to what extent personalisation can be beneficial for interactions and users. Robots developed as end-to-end systems for conducting social interactions can amplify cultural biases, gender and age stereotypes. Therefore, it is crucial to discuss when personalisation is desired or required, and when it should be avoided. 
      In contexts such as healthcare and education, personalisation can lead to inadequate care or support and lower acceptance of the professionals who use the technology (teachers and healthcare professionals). Additionally, collecting personal data to provide tailored assistance can raise privacy concerns, as many machine learning algorithms are not transparent to users. Furthermore, deep learning algorithms may amplify existing biases, hindering the primary goal of making interactions more engaging and trustworthy.

      <br>
      The workshop explores the complex area of personalisation and behavioural adaptation in social human-robot interaction (HRI), examining both their benefits and drawbacks. It provides a forum for a diverse group of researchers from various fields, including psychology, neuroscience, computer science, robotics, and sociology, to come together. 
      </p>
  </div>

  <div class="col-sm-3">
  {% if page.img %}
    <img class="caption__media" data-interchange="
    {% for img in page.img %}
      [{{site.baseurl}}/asset/img/{{img[1]}} ({{img[0]}})]
      {% unless forloop.last %}, {% endunless %}
    {% endfor %}
    ">
  {% endif %}
  <img class="card-img" src="{{ site.baseurl }}/assets/img/{{ page.img }}" alt="image">
  </div>

  <div class="col-sm-12">
  <h3>Goal</h3>
  <p class="main-description">
  The workshop aims to lay the foundations for a potential <b>journal publication</b>, using the insights and discussions generated during the sessions. Participants will be encouraged to actively contribute to the journal to ensure diverse perspectives and comprehensive coverage of the topics discussed, thereby increasing the impact of the results. For this reason, the workshop program will alternate interactive activities with panel sessions and keynote presentations. This will enhance the comprehension of the topic while maintaining an engaging structure for the audience.
  </p>

  <p>Contact us at: <a href="mailto:warn-workshop@proton.me">warn-workshop@proton.me</a></p>
  </div>
</div>

<hr>

<div id="container-header">

  <div class="row m-3">
    <div class="col-sm-12" style="text-align: -webkit-center;">
      <p>Lessons learned from <a href="https://sites.google.com/view/warn-roman23/home" target=_blank>past</a> edition. Aspects of personalization in robotics.</p>
    </div>
    <div class="col-sm-6" style="text-align: -webkit-center;">
      <b>Positive</b>
      <p><span id="pro-text"></span></p>
    </div>
    <div class="col-sm-6" style="text-align: -webkit-center;">
      <b>Negative</b>
      <p><span id="cons-text"></span></p>
    </div>
  </div>

<hr>
  <div class="row m-3">
  <div class="col-sm-12">
      <h3>Our presenters</h3>
      </div>
      <div class="card-group mt-3 mb-5">
        <div class="col-sm-3">
          <div class="card m-1 p-1 h-100">
            <a href="https://laurelriek.org/" target=_blank>
              <img src="{{ site.baseurl }}/assets/img/lr.jpg" class="card-img-top speaker-img" alt="Lauriel">
            </a>
            <div class="card-body" style="padding-bottom: initial;">
              <h5 class="card-title">Lauriel Riek</h5>
              <p class="card-text">Professor of Computer Science and Engineering</p>
              <p class="card-text">UC San Diego</p>
            </div>        
          </div>
        </div>
        <div class="col-sm-3">
          <div class="card m-1 p-1 h-100">
            <a href="https://emmanuel-senft.github.io/" target=_blank>
              <img src="{{ site.baseurl }}/assets/img/es.jpg" class="card-img-top speaker-img" alt="Emmanuel">
            </a>
            <div class="card-body" style="padding-bottom: initial;">
              <h5 class="card-title">Emmanuel Senft</h5>
              <p class="card-text">Research Scientist and Group Leader</p>
              <p class="card-text">Idiap Research Institute</p>
            </div>        
          </div>
        </div>
        <div class="col-sm-3">
          <div class="card m-1 p-1 h-100">
            <a href="" target=_blank>
              <img src="{{ site.baseurl }}/assets/img/ukf.png" class="card-img-top speaker-img" alt="TBD">
            </a>
            <div class="card-body" style="padding-bottom: initial;">
              <h5 class="card-title">Presenter TBD</h5>
            </div>        
          </div>
        </div>
        <div class="col-sm-3">
          <div class="card m-1 p-1 h-100">
            <a href="" target=_blank>
              <img src="{{ site.baseurl }}/assets/img/ukm.png" class="card-img-top speaker-img" alt="TBD">
            </a>
            <div class="card-body" style="padding-bottom: initial;">
              <h5 class="card-title">Presenter TBD</h5>
            </div>        
          </div>
        </div>
  </div>
  </div>
<hr>
<p>Brought you by</p>

<div class="card-group mt-3 mb-5">
  <div class="card m-1 p-1">
    <a href="http://www.perseo.eu">
      <img src="{{ site.baseurl }}/assets/img/perseo.png" class="card-img-top" alt="Perseo">
    </a>
  </div>

  <div class="card m-1 p-1" style="align-self: flex-start; background:red;">
    <a href="https://www.iri.upc.edu/">
      <img src="{{ site.baseurl }}/assets/img/iri.png" class="card-img-top" alt="IRI">
    </a>
  </div>

<div class="col">
  <div class="row">
    <div class="card m-1 p-1" style="align-self: flex-start;">
      <a href="http://www.unina.it">
        <img src="{{ site.baseurl }}/assets/img/unina.png" class="card-img-center" alt="Federico II">
      </a>
    </div>
  </div>
  <div class="row">
    <div class="card m-1 p-1" style="align-self: flex-start;">
      <a href="http://www.unibz.it">
        <img src="{{ site.baseurl }}/assets/img/unibz.png" class="card-img-center" alt="UniBZ">
      </a>
    </div>
  </div>
</div>

  <div class="card m-1 p-1" style="align-self: flex-start;">
    <a href="https://www.uni-augsburg.de/">
      <img src="{{ '/assets/css/aus.png' | relative_url | bust_file_cache }}" class="card-img-center" alt="AusburgUni">
    </a>
  </div>

</div>
<hr>
</div>



<!-- Load library from the CDN -->
<script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>

<!-- Setup and start animation! -->
<script>
   var pro = new Typed('#pro-text', {
    strings: ["Acceptance", "Usability", "Comfort", "Increased Enjoyment", "Familiarization"],
    typeSpeed: 50,
    // startDelay: 100,
    backDelay: 4000,
    fadeOut: false,
    backSpeed: 40,
    smartBackspace: true,
    loop: true,
    showCursor: false
  });

  var cons = new Typed('#cons-text', {
    strings: ["Risk of unpredictable behaviours", "Stereotyping", "Deception", "Introduction of Biases", "Risk of Manipulation"],
    typeSpeed: 50,
    // startDelay: 100,
    backDelay: 4000,
    fadeOut: false,
    backSpeed: 40,
    smartBackspace: true,
    loop: true,
    showCursor: false
  });
</script>



