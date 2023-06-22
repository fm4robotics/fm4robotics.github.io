---
layout: article
title: Foundation Models for Robotics (FM4R)
excerpt: CoRL 2023 Workshop
menu: true
show_info: true
titles:
  en      : &EN       Home
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
key: page-home
article_header:
  type: overlay
  theme: dark
  align: left
  actions:
    - text: 6 Novenmber 2023 | Atlanta, Georgia, USA
  background_image:
    src: /assets/images/atlanta_image.jpeg
#    gradient: 'linear-gradient(135deg, rgba(52, 140, 96, 0.4), rgba(136, 73, 107, 0.4))'
---

<style>
.schedule-table-heading {
    display: inline;
    font-weight: bold;
    font-size: 20px;
    color: #999999;
    padding:0 0 20px 0;
}

.schedule-table-timecol {
    padding:0 50px 0 50px;
    display:inline;
}

.schedule-table-eventcol {
    display:inline;
    display:inline-block;
    inline-size: 300px;
}

.schedule-table-contentcol {
    display:inline;
    display:inline-block;
    inline-size: 250px;
    font-size:14px;
    line-height: normal;
}

.schedule-table-row-even {
    display:block;
    width:800px;
    background-color: #EEEEEE;
    padding:10px;
}

.schedule-table-row-odd {
    display:block;
    width:800px;
    padding:10px;
}

.article__header--overlay .overlay {
    min-height: 36rem;
    padding-top: 5rem;
    padding-bottom: 5rem;
}

.article__header {
    margin: 0 0 0 0;
}

.article__header h1 {
    display: inline;
    font-size: 2.5em;
    letter-spacing: -0.04em;
    line-height: 0.9;
    text-shadow: -20px -8px 17px rgb(0 0 0 / 30%);
    word-wrap: break-word;
}

.overlay__excerpt {
    margin: 20px 0 0 0;
}

ul.menu li::after {
    content:"6 Novenmber 2023 | Atlanta, Georgia, USA";
}

ul.menu a {
    display: none;
}

.pc-column {
    width:270px;
    display:inline-block;
    vertical-align: top;
}

.pc_list_item {
    display:inline-block;
    width:200px;
}

.organiser_profile {
    font-weight:normal;
    color: black;
}

.organiser_profile a:link a:visited a:hover a:active {
    font-weight:normal;
    color: #000000;
}

.organiser_profile p {
    font-weight:normal;
    color: #000000;
}

.logos-organizers {
    display: flex;
    align-items: center;
    flex-direction: row;
    flex-wrap: nowrap;
}

.img-fluid {
    max-width: 100%;
    height: auto;
}

img {
    vertical-align: middle;
    border-style: none;
}
</style>

<script>
  var x = setInterval(function() {
    var d = new Date();
    var n = d.toLocaleTimeString("en-US", {timeZone: "America/New_York", hour: '2-digit', minute:'2-digit', hour12: false})
    document.getElementById("edt").innerHTML = n
  }, 1000);
</script>

<script>
  var x = setInterval(function() {
    var d = new Date();
    var n = d.toLocaleTimeString("en-US", {timeZone: "Europe/Vienna", hour: '2-digit', minute:'2-digit', hour12: false})
    document.getElementById("cet").innerHTML = n
  }, 1000);
</script>

<script>
  {%- include scripts/lib/swiper.js -%}
  var SOURCES = window.TEXT_VARIABLES.sources;
  window.Lazyload.js(SOURCES.jquery, function() {
    $('.swiper-demo').swiper();
  });
</script>

<script>

  var countDownDate = new Date("Feb 15, 2022 23:59:59 UTC").getTime();  
  countDownDate = countDownDate + 1000 * 3600 * 12


  var x = setInterval(function() {


    var now = new Date().getTime();


    var distance = countDownDate - now;


    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);


    var countdown = days + "d " + hours + "h " + minutes + "m " + seconds + "s ";


    if (distance < 0) {
      clearInterval(x);
      countdown = "(expired)";  
    }

    document.getElementById("countdown").innerHTML = countdown

  }, 1000);
</script>

<br>

## About

Welcome to the 1st Workshop on <i>Foundation Models for Robotics</i> (FM4R), co-located with the 7th International Conference on Robot Learning (CoRL 2023), to be held on November 6th, 2023 in hybrid? format.

Foundation models represent a new paradigm shift in artificial intelligence, defined by the training of large-scale models on internet-scale datasets. These models encapsulate a broad spectrum of general knowledge, and can be adapted or fine-tuned for specific downstream tasks or applications. Examples of such models include CLIP, SAM, VILD, GPT, BLIP, LLaMa, DINO, VPT, I-JEPA, PALM-E, and others. The era of foundation models is marked by significant advancements in a multitude of domains such as language processing, image generation, visual perception, and multisensory integration.<br>

The aim of this workshop is to spark the integration of foundation models into the field of robotics. We hypothesize, based on recent findings, that integrating these models could revolutionize the way we address robotics challenges, offering multifaceted, modular, and generalizable solutions that can unlock opportunities for innovation that were previously unreachable. In this workshop, we will embark on an exploration of the untapped potential of foundation models in robotics. We will scrutinize how the extensive knowledge contained in foundation models can be leveraged to effectively tackle diverse robotics tasks. Moreover, we strive to garner a collaborative workshop that will drive the evolution of modular robotics solutions that can be easily recreated for cumulative research.<br>


### Topics covered

<div>
<div style="width:49%; display:inline-block; font-size:14px; vertical-align:top">
<ul>
<li>Adapting foundation models for robotics</li>
<!-- <li>Safety verification, certifying learning-based control under dynamical uncertainty, dependability analysis</li>
<li>Robustness to out-of-distribution road scenes</li>
<li>Learning vehicle dynamics at high-speeds and in unstable regimes</li>
<li>Vision-based perception and scene understanding for autonomous driving</li>
<li>Representation learning for visuomotor control</li>
<li>Transfer learning; simulation to real-world; meta-learning; domain adaptation; *-shot learning; self/semi/weakly-supervised learning; multi-task learning</li>
<li>End-to-end and real-time autonomous driving systems</li>
<li>Novel automotive sensors and their applications</li>
<li>Trajectory forecasting; Behavior prediction of pedestrians, vehicles, and animals</li>
<li>Explainability in autonomous driving</li>
<li>Learning to drive via imitation learning</li>
<li>Learning to drive via distribution awareness</li> -->
</ul>
</div>
<div style="width:49%; display:inline-block; font-size:14px; vertical-align:top">
<ul>
<li>Pretraining and representation learning for robotics</li>
<!-- <li>Classical planning and control for autonomous driving</li>
<li>Cooperative and competitive multi-agent systems</li>
<li>Visual grounding and its application to autonomous driving</li>
<li>Vision-language navigation for autonomous driving</li>
<li>Audio-visual navigation for autonomous driving</li>
<li>Neuro-symbolic approaches in autonomous driving; Knowledge representation and reasoning</li>
<li>Auditory perception (detection, tracking, segmentation, motion estimation, etc)</li>
<li>Brain-inspired autonomous control systems</li>
<li>Human factors in autonomous driving</li>
<li>AI ethics in autonomous driving</li>
<li>Autonomous driving datasets, simulation, evaluations, and metrics</li>
<li>Connected autonomous driving, vehicle-to-vehicle, vehicle-to-infrastructure communication, digital twins</li>
<li>Autonomous driving for traffic management and emission reduction; intelligent transportation systems</li> -->
</ul>
</div>
</div>

## Dates

Note: all deadlines are in <b>Anywhere on Earth</b>.

### Paper Submission

<div>
<b>Submissions open:</b> 1 October 2023<br>
<!-- <b>Submissions due:</b> <p style="display:inline; text-decoration:line-through;">20 May 2022</p><p style="display:inline; color:red;">&nbsp;27 May 2022</p><br> -->
<b>Submissions due:</b> 15 October 2023<br>
<b>Notification:</b> 20 October 2023<br>
<b>Camera Ready</b>: 25 October 2023<br>
<b>Oral/Poster video upload</b>:  30 October 2023
</div>

### Workshop Event

<b>Date:</b> 6 November 2023

## Schedule

Friday, 6 November 2023. All times are in Eastern Daylight Time (EDT). Current time is <span id="edt"></span>.

<div style="display:block; width:900px; padding:20px; border:solid 4px #CCCCCC;">
<div class="schedule-table-heading" style="margin-left:57px; display:inline-block; inline-size:100px;">Time</div>
<div class="schedule-table-heading" style="display:inline-block; inline-size:295px;">Event</div>
<div class="schedule-table-heading">Content</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">08:50</div>
<div class="schedule-table-eventcol">Welcome</div>
<div class="schedule-table-contentcol">Opening Remarks</div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">09:00</div>
<div class="schedule-table-eventcol">Invited Talk #1</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">09:30</div>
<div class="schedule-table-eventcol">Invited Talk #2</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">10:00</div>
<div class="schedule-table-eventcol">Lightning Talks</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">11:00</div>
<div class="schedule-table-eventcol">Poster Session / Coffee Break</div>
<div class="schedule-table-contentcol"></div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">12:00</div>
<div class="schedule-table-eventcol">Invited Talk #3</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">12:30</div>
<div class="schedule-table-eventcol">Lunch Break</div>
<div class="schedule-table-contentcol"></div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">13:30</div>
<div class="schedule-table-eventcol">Invited Talk #4</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">14:00</div>
<div class="schedule-table-eventcol">Invited Talk #5</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">14:30</div>
<div class="schedule-table-eventcol">Spotlight Talks</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">15:30</div>
<div class="schedule-table-eventcol">Poster Session / Coffee Break</div>
<div class="schedule-table-contentcol"></div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">16:30</div>
<div class="schedule-table-eventcol">Invited Talk #6</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">17:00</div>
<div class="schedule-table-eventcol">Panel Discussion</div>
<div class="schedule-table-contentcol">TBD</div>
</div>

<div class="schedule-table-odd-even">
<div class="schedule-table-timecol">18:00</div>
<div class="schedule-table-eventcol">Conclusion</div>
<div class="schedule-table-contentcol">Closing Remarks</div>
</div>

</div>


<!-- ## Program Committee -->

<!-- column 1 -->
<!-- <div class="pc-column">
<ul>
<li>Arav Agarwal (<b>ER</b>, <b>TR</b>)</li>
<li>Eren Aksoy</li>
<li>Raghuram Mandyam Annasamy</li>
<li>Tiago Cortinhal</li>
<li>Xiaoxiao Du (<b>TR</b>)</li>
<li>Isht Dwivedi</li>
<li>Hesham Eraqi</li>
<li>Xiangyu Gao</li>
<li>Sahika Genc (<b>ER</b>)</li>
<li>S. Alireza Golestaneh (<b>TR</b>)</li>
</ul>
</div> -->

<!-- column 2 -->
<!-- <div class="pc-column" style="margin:0 30px 0 0;">
<ul>
<li>David Held (<b>SMR</b>)</li>
<li>Todd Hester (<b>SMR</b>)</li>
<li>Zehao Huang</li>
<li>Fabian Hüger</li>
<li>Arec Jamgochian (<b>TR</b>)</li>
<li>Rowan McAllister (<b>SMR</b>)</li>
<li>Kunal Menda</li>
<li>Aarati Noronha</li>
<li>Praveen Palanisamy</li>
<li>João Pinho (<b>ER</b>)</li>
</ul>
</div> -->

<!-- column 3 -->
<!-- <div class="pc-column">
<ul>
<li>Daniele Reda</li>
<li>Nazmus Sakib</li>
<li>Pranjay Shyam</li>
<li>Mark Schutera</li>
<li>Zhaoen Su</li>
<li>Ram Vasudevan</li>
<li>Yujie Wei</li>
<li>Weiran Yao</li>
</ul>
</div> -->

---

<!-- <b>ER</b> — <i>Recognises PC member who served ("+" additionally) as an Emergency Reviewer.</i><br> -->
<!-- <b>TR</b> — <i>Recognises PC member who, according to Chair ratings, ranked in the Top 15% of Reviewers.</i><br> -->
<!-- <b>SMR</b> — <i>Recognises PC member who agreed to provide their services as a Senior Meta-Reviewer.</i> -->

<!-- ## Sponsors -->

<!-- <img src="{{ site.baseurl }}/assets/images/sponsors/sponsor_banner.png"> -->
<!--
<div class="col-lg-12 col-xl-6">
            <div class="logos-organizers">
              <div class="logo-organizer">
                <img class="img-fluid" src="{{ site.baseurl }}/assets/images/sponsors/arrival_logo.png">
              </div>
              <div class="logo-organizer">
                <img class="img-fluid" src="{{ site.baseurl }}/assets/images/sponsors/cmu_logo.png">
              </div>
              <div class="logo-organizer">
                <img class="img-fluid" src="{{ site.baseurl }}/assets/images/sponsors/aicrowd_logo.png">
              </div>
              <div class="logo-organizer">
                <img class="img-fluid" src="{{ site.baseurl }}/assets/images/sponsors/aws_logo.png">
              </div>
              <div class="logo-organizer">
                <img class="img-fluid" src="{{ site.baseurl }}/assets/images/sponsors/bosch_logo.png">
              </div>
            </div>
          </div>
-->
<!--
<div style="width:900px; display:inline-block;">
<img style="height:100px; width:186px;" src="{{ site.baseurl }}/assets/images/sponsors/arrival_logo.png">
<img style="height:100px; width:157px;" src="{{ site.baseurl }}/assets/images/sponsors/cmu_logo.png">
<img style="height:100px; width:100px;" src="{{ site.baseurl }}/assets/images/sponsors/aicrowd_logo.png">
<img style="height:100px; width:98px;" src="{{ site.baseurl }}/assets/images/sponsors/aws_logo.png">
<img style="height:100px; width:272px;" src="{{ site.baseurl }}/assets/images/sponsors/bosch_logo.png">
<img style="height:100px; width:354px;" src="{{ site.baseurl }}/assets/images/sponsors/honda_logo.png">
</div>
-->
