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

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">09:00</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/david_held.png" alt="David Held">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">David Held</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987747/selfsupervised-3d-perception-for-autonomous-driving?ref=folder-105306" target="_blank"><i>Self-supervised learning for autonomous driving</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">09:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/melanie_zeilinger.png" alt="Melanie Zeilinger">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Melanie Zeilinger</p>
<p style="margin:0 0 0 10px; font-size:10px;">ETH Zürich</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987741/learning-for-high-performance-yet-safe-control?ref=folder-105306"><i>Learning for High Performance yet Safe Control</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">10:00</div>
<div class="schedule-table-eventcol">Social + Poster Session</div>
<!--div class="schedule-table-contentcol">Paper IDs: 1, 2, 3, 4, 5, 6, 9, 10, 13, 17, 18, 21, 22</div-->
<div class="schedule-table-contentcol"><b>Gathertown</b> and in-person displays</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">11:00</div>
<div class="schedule-table-eventcol">Spotlight Talks</div>
<!--div class="schedule-table-contentcol">Content</div-->
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Zijian Guo</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987752/constrained-modelbased-reinforcement-learning-via-robust-planning?ref=folder-105306"><i>#16: Constrained Model-based Reinforcement Learning via Robust Planning</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Linrui Zhang</p>
<p style="margin:0 0 0 10px; font-size:10px;">Tsinghua University</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987764/saferlkit-evaluating-efficient-reinforcement-learning-methods-for-safe-autonomous-driving?ref=folder-105306"><i>#12: SafeRL-Kit: Evaluating Efficient Reinforcement Learning Methods for Safe Autonomous Driving</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">11:30</div>
<div class="schedule-table-eventcol">Autonomous Racing Virtual Challenge: Contributed Talks</div>
<!--div class="schedule-table-contentcol">Content</div-->
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Shivansh Beohar</p>
<p style="margin:0 0 0 10px; font-size:10px;">IIIT Allahabad</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987763/solving-learntorace-autonomous-racing-challenge-by-planning-in-latent-space?ref=folder-105306"><i>#11: Solving Learn-to-Race Autonomous Racing Challenge by Planning in Latent Space</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">James Bockman</p>
<p style="margin:0 0 0 10px; font-size:10px;">U Adelaide</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987768/the-edge-of-disaster-a-battle-between-autonomous-racing-and-safety?ref=folder-105306"><i>#14: The Edge of Disaster: A Battle Between Autonomous Racing and Safety</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">12:00</div>
<div class="schedule-table-eventcol">Lunch Break</div>
<!--div class="schedule-table-contentcol">Content</div-->
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">13:30</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/peter_stone.png" alt="Peter Stone">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Peter Stone</p>
<p style="margin:0 0 0 10px; font-size:10px;">UT Austin; Sony AI</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987742/reward-misdesign-for-autonomous-driving-and-accumulating-safety-rules-from-catastrophic-action-effects?ref=folder-105306"><i>Reward (Mis)design for Autonomous Driving and Accumulating Safety Rules from Catastrophic Action Effects</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol">14:00</div>
<div class="schedule-table-eventcol">Spotlight Talks</div>
<!--div class="schedule-table-contentcol">Content</div-->
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Weiran Yao</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987757/distributionaware-goal-prediction-and-conformant-modelbased-planning-for-safe-autonomous-driving?ref=folder-105306"><i>#23: Distribution-aware Goal Prediction and Conformant Model-based Planning for Safe Autonomous Driving</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">&nbsp;</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
&nbsp;
</div>
<div style="display:inline-block; width:150px; line-height:1.4; margin:0 0 0 40px">
<p style="margin:0 0 0 10px;">Zuxin Liu</p>
<p style="margin:0 0 0 10px; font-size:10px;">CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol" style="margin:0 0 0 35px;"><a target="_blank" href="https://slideslive.com/38987751/on-the-robustness-of-safe-reinforcement-learning-under-observational-perturbations?ref=folder-105306"><i>#15: On the Robustness of Safe Reinforcement Learning under Observational Perturbations</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">14:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/todd_hester.png" alt="Todd Hester">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Todd Hester</p>
<p style="margin:0 0 0 10px; font-size:10px;">Amazon Scout</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987743/multimodal-sensor-fusion-for-the-amazon-scout-robot?ref=folder-105306"><i>Multi-modal sensor fusion for the Amazon Scout robot</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">15:00</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/chelsea_finn.png" alt="Chelsea Finn">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Chelsea Finn</p>
<p style="margin:0 0 0 10px; font-size:10px;">Stanford + Google Brain</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987744/robots-that-learn-to-be-safe?ref=folder-105306"><i>Robots that Learn to Be Safe</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">15:30</div>
<div class="schedule-table-eventcol">Social + Poster Session</div>
<!--div class="schedule-table-contentcol">Paper IDs: 1, 2, 3, 4, 5, 6, 9, 10, 13, 17, 18, 21, 22</div-->
<div class="schedule-table-contentcol"><b>Gathertown</b> and in-person displays</div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">16:30</div>
<div class="schedule-table-eventcol">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/andrea_bajcsy.png" alt="Andrea Bajcsy">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Andrea Bajcsy</p>
<p style="margin:0 0 0 10px; font-size:10px;">UC Berkeley / CMU</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987745/practical-safety-assurances-for-dynamic-humanrobot-interactions?ref=folder-105306"><i>Practical Safety Assurances for Dynamic Human-Robot Interactions</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol" style="vertical-align: 10px;">17:00</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/jeff_schneider.png" alt="Jeff Schneider">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Jeff Schneider</p>
<p style="margin:0 0 0 10px; font-size:10px;">Carnegie Mellon University</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987746/safety-and-reinforcement-learning-for-selfdriving-cars?ref=folder-105306"><i>Reinforcement Learning for self-driving cars</i></a></div>
</div>

<div class="schedule-table-row-even">
<div class="schedule-table-timecol" style="vertical-align: 10px;">17:30</div>
<div class="schedule-table-eventcol"><div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:60px;">
<img style="width:50px; height:50px; position: relative; bottom: 10px;" src="{{ site.baseurl }}/assets/images/speakers/sergey_levine.png" alt="Sergey Levine">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Sergey Levine</p>
<p style="margin:0 0 0 10px; font-size:10px;">UC Berkeley</p>
</div>
</div>
</div>
<div class="schedule-table-contentcol"><a target="_blank" href="https://slideslive.com/38987748/learning-plannable-representations-and-planning-with-learnable-skills?ref=folder-105306"><i>Learning Plannable Representations and Planning with Learnable Skills</i></a></div>
</div>

<div class="schedule-table-row-odd">
<div class="schedule-table-timecol">18:00</div>
<div class="schedule-table-eventcol">Conclusion</div>
<div class="schedule-table-contentcol">Closing Remarks</div>
</div>

</div>

<!--Poster Presentation Gathertown link: https://app.gather.town/app/wLuHBtWDuNBoHgun/SL4AD%2022  -->

## Speakers

<div style="display:block; padding:10px 0 0 0; width:900px;">

<a href="https://www.ias.informatik.tu-darmstadt.de/Team/GeorgiaChalvatzaki" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/Georgia_Chalvatzaki.jpeg" alt="Georgia Chalvatzaki">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Georgia Chalvatzaki</p>
<p style="margin:0 0 0 10px; font-size:10px;">Full Professor<br>TU Darmstadt</p>
</div>
</div>
</a>

<a href="https://yonatanbisk.com/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/Yonatan_Bisk.jpeg" alt="Yonatan Bisk">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Yonatan Bisk</p>
<p style="margin:0 0 0 10px; font-size:10px;">Assistant Professor<br>Carnegie Mellon University</p>
</div>
</div>
</a>

<a href="https://dorsa.fyi" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/dorsa_sadigh.jpeg" alt="Dorsa Sadigh">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Dorsa Sadigh</p>
<p style="margin:0 0 0 10px; font-size:10px;">Assistant Professor<br>Stanford University</p>
</div>
</div>
</a>

<a href="https://jimfan.me/" target="_blank" class="speaker_profile">
<div style="display:inline-block; width:270px; margin:20px 0 0 0;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/speakers/Jim_Fan.jpeg" alt="Linxi 'Jim' Fan">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Linxi 'Jim' Fan</p>
<p style="margin:0 0 0 10px; font-size:10px;">Research Scientist<br>NVIDIA AI</p>
</div>
</div>
</a>

</div>

## Organizers

<div style="display:block; padding:10px 0 0 0; width:900px;">

<a href="https://scholar.google.com/citations?user=6tiiQtgAAAAJ" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/andrew_melnik.jpeg" alt="Andrew Melnik">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Andrew Melnik</p>
<p style="margin:0 0 0 10px; font-size:10px;">Postdoc<br>Bielefeld University</p>
</div>
</div>
</a>

<a href="https://krishanrana.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/krishan_rana.jpeg" alt="Krishan Rana">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Krishan Rana</p>
<p style="margin:0 0 0 10px; font-size:10px;">Postdoc<br>QUT</p>
</div>
</div>
</a>

<a href="https://www.linkedin.com/in/jonmfrancis/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/jonathan_francis.jpeg" alt="Jonathan Francis">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Jonathan Francis</p>
<p style="margin:0 0 0 10px; font-size:10px;">Senior Research Scientist<br>Bosch Research</p>
</div>
</div>
</a>

<a href="https://ishikasingh.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/ishika_singh.jpeg" alt="Ishika Singh">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Ishika Singh</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD Student<br>USC</p>
</div>
</div>
</a>

<a href="https://guanzhi.me/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/guanzhi_wang.jpeg" alt="Guanzhi Wang">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Guanzhi Wang</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD Student<br>Caltech</p>
</div>
</div>
</a>

<a href="https://www.linkedin.com/in/norman-di-palo/?originalSubdomain=uk" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/norman_di_palo.jpeg" alt="Norman Di Palo">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Norman Di Palo</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD Student<br>Imperial College London</p>
</div>
</div>
</a>

<a href="https://vidhijain.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/vidhi_jain.jpeg" alt="Vidhi Jain">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Vidhi Jain</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD Student<br>CMU</p>
</div>
</div>
</a>

<a href="https://www.linkedin.com/in/quanting-xie-4197a814a/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/quanting_xie.jpeg" alt="Quanting Xie">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Quanting "Daniel" Xie</p>
<p style="margin:0 0 0 10px; font-size:10px;">MS Student<br>CMU</p>
</div>
</div>
</a>

<a href="https://yaqi-xie.me/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/yaqi_xie.png" alt="Yaqi Xie">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Yaqi Xie</p>
<p style="margin:0 0 0 10px; font-size:10px;">Postdoc<br>CMU</p>
</div>
</div>
</a>

<a href="https://jeffreyyh.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/yafei_hu.png" alt="Yafei Hu">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Yafei "Jeffrey" Hu</p>
<p style="margin:0 0 0 10px; font-size:10px;">PhD Student<br>CMU</p>
</div>
</div>
</a>

<a href="https://nikosuenderhauf.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/niko_sünderhauf.png" alt="Niko Sünderhauf">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Niko Sünderhauf</p>
<p style="margin:0 0 0 10px; font-size:10px;">Professor<br>QUT</p>
</div>
</div>
</a>

<a href="https://nikosuenderhauf.github.io/" target="_blank" class="organiser_profile">
<div style="display:inline-block; width:270px;">
<div style="display:inline-block; width:101px;">
<img style="width:100px; height:100px; position: relative; bottom: 40px;" src="{{ site.baseurl }}/assets/images/organizers/danica_kragic.png" alt="Danica Kragic">
</div>
<div style="display:inline-block; width:150px; line-height:1.4;">
<p style="margin:0 0 0 10px;">Danica Kragic</p>
<p style="margin:0 0 0 10px; font-size:10px;">Professor<br>KTH</p>
</div>
</div>
</a>

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
