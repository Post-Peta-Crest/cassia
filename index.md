---
title: Project CASSIA
---
Framework for Administration of Social Simulations on Massively Parallel Computers


# Team Description

* PI: Itsuki Noda (National Institute of Advanced Industrial Science and Technology)
* co-PI: Nobuyasu Ito (University of Tokyo, Riken), Kiyoshi Izumi (University of Tokyo), Hiromitsu Hattori (Ritsumeikan University), Tomio Kamada (Kobe University), Hideyuki Mizuta (IBM)
* Research Period: 2012--2017
* [Research highlights in PDF]({{ site.baseurl }}/leaflet.2017.1023a.byNoda.pdf)

# Published Software

* [OACIS](https://github.com/crest-cassia/oacis)
  / [(mirror@RIKEN)](http://www.r-ccs.riken.jp/jp/k/software/)
* [CARAVAN](https://github.com/crest-cassia/caravan)
* [X10 libraries](http://x10-lang.org/)
* [XASDI](http://x10-lang.org/xasdi/) 
* [Plham](https://hub.docker.com/r/oacis/oacis_jupyter_plham/)
* [CrowdWalk](https://github.com/crest-cassia/CrowdWalk)
* [ADVENTURE Mates](http://adventure.sys.t.u-tokyo.ac.jp/jp/download/Mates.html)

---

# Overview

Project CASSIA (Comprehensive Architecture of Social Simulation for Inclusive Analysis) aims to develop a framework to administer to execute large-scale multiagent simulations exhaustively to analyze socially interactive systems. The framework will realize engineering environment to design and synthesize social systems like traffics, economy and politics.
The framework consists of:
* __MASS Planning Module__: a manager module conducts effective execution plans of simulations among massive possible conditions according to available computer resources.
* __MASS Parallel Middleware__: an execution middleware provides functionality to realize distributed multi-agent simulation on many-core computers.

![CASSIA framework]({{ site.baseurl }}/img/cassia-framework.png)


# OACIS & CARAVAN

__OACIS__ (Organizing Assistant for Comprehensive and Interactive Simulations) is a job management software for large-scale simulations. It controls a large number of simulation jobs executed in various remote servers, keeps these results in an organized way, and manages the analyses on these results.

![OACIS framework]({{ site.baseurl }}/img/oacis-framework.png)

__CARAVAN__ provides more powerful scalability for exhaustive simulation. These functionalities are especially beneficial for the complex simulation models having many parameters for which a lot of parameter searches are required.

![CARAVAN framework]({{ site.baseurl }}/img/caravan-framework.png)


# XASDI

__XASDI__ is the Large-scale agent-based social simulation framework with billions of distributed agents that provides  easy-to-use API bridge with Java and X10-based runtime for high scalability. XASDI environment executes various social simulations written in Java with distributed agents  and managers written in X10.

![XASDI]({{ site.baseurl }}/img/xasdi-framework.png)


# Plham and X10 extention

__Plham__ is a platform for large-scale and high-frequency artificial market simulation.  It consists of models of markets for each stocks and three types of agents (high-freq. traders, short-term and long-term traders).


![Plham]({{ site.baseurl }}/img/plham-overview.png)

![X10lib]({{ site.baseurl }}/img/x10-management.png)

In order to enhance parallelism of computation, we introduce asynchronous computation in agents and communication between agents/markets, and provide high-level library to program them.
 
We succeeded to re-generate several market phenomena like flash-crash and effects of  risk management with Value at Risks, which are useful to analyze soundness of markets.

![phase diagram]({{ site.baseurl }}/img/phase-diagram.forMarket.png)


# Evacuation Simulation
CASSIA Framework can illustrate a trade-off structure in planning of evacuations from disasters.  Optimization in disaster responses is serious requirements for local governments. But, such optimization includes multiple objective functions.  So, the important issue is how to understand trade-off structures of such multi-objective functions over large number of policy options.

We apply our framework to evaluate evacuation plans, which have over 300 control parameters, to find out such trade-off.  We implement NSGA-II algorithm to search optimal structures over large parameter spaces, and utilize the performance of K-computers to speed-up the process.

![Nishiyodogawa Area]({{ site.baseurl }}/img/nishiyodogawa_area.png)
![NSGA-II module]({{ site.baseurl }}/img/nsga-ii.module.forOACIS.png)

![Result 1]({{ site.baseurl }}/img/result-1.nsga-ii.png)
![Result 2]({{ site.baseurl }}/img/result-2.nsga-ii.png)




---

![CASSIA logo]({{ site.baseurl }}/img/cassia-draw-2014.0614a.png)
