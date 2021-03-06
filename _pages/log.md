---
layout: default
title: IMMERSE Log
---

[My Schedule](https://jacobdbrown4.github.io/jacob_brown//pages/schedule/)
## January
* released SpyDrNet 1.10.1 for a few bug fixes
* IMMERSE 2022 application
* release SpyDrNet SHREC 1.3.0

## December
* wrote up a spydrnet wiki page about imports and *\_\_init\_\_.py* files
* reviewed ganesh's pull request for extending spydrnet classes
* released SpyDrNet 1.10.0 with extension capability

## November
* released SpyDrNet 1.9 with some of Ganesh's more minor contributions
* researched pytest and how they manage their plugins

## October
* met with Ganesh Gore (U of U phd student)
* made a suggestion to Ganesh about storing href information (see github issue 155)
* released the last independent version of SpyDrNet SHREC
* worked on reviewing Ganesh's code and helping him with his contributions
* updated SpyDrNet Bootcamp wiki page with more info to help new students

### Week 23-24:
* Worked on missing netlist issue

### Week 22: September 20, 2021
* Worked on getting spydrnet ready for a release
* Found what is causing the big netlists to be missing from the example netlists
* Worked on the SpyDrNet SHREC dependent branch

### Week 21: September 13, 2021
* Worked on spydrnet example netlist issue
* Worked on SpyDrNet_SHREC dependent (version that depends on Spydrnet TMR repo)

### Week 20: September 6, 2021
* Met with Dr. Wirthlin about things to do for the next few weeks
* Looked into spydrnet example netlist issue

### Week 19: August 30, 2021
* **Weekly Goals**:
  * make a plan for what to do during this semester
* **What I Did**:
  * started documenting the problem with the reduction voters and a fix to the code to fix it

### Week 18: August 23, 2021
* **Weekly Goals**:
  * work on improving documentation/tests/etc.
  * finish making a version of SpyDrNet SHREC that relies on SpyDrNet TMR
  * figure out what else I can do next
* **Monday, Tuesday**:
  * worked on pytests
  * wrote up two page summary of accomplishments this summary and submitted it on learning suite
* **Wednesday, Thursday**:
  * rewrote on of the drc checks, check_connections_after_replication_and_insertion. Made it a little more clear, and a lot faster.
  * worked on version of SpyDrNet SHREC that is dependent on SpyDrNet TMR
* **Friday**:
  * met with Andrew about adding his partial tmr scripts to the spydrnet shrec repository, as well as other things

### Week 17: August 16, 2021
* **Weekly Goals**:
  * work with Ben to finish setting up SpyDrNet TMR and hopefully release it
* **Monday**:
  * added .is_unique() attribute to both netlists and instances in the ir
  * started documenting the example netlists but didn't get too far
  * got travis ci working for spydrnet tmr
* **Tuesday**:
  * fixes, additions, and changes in SpyDrNet TMR in preparation for the release
* **Wednesday**:
  * released SpyDrNet TMR with Ben
* **Thursday**:
  * got accesss to the fpga server and started looking at Andrew's work
  * worked on fixing the bug in finding reduction voter points 
  * worked on making a version of SpyDrNet SHREC that relies on SpyDrNet TMR
* **Friday**:
  * improved drc_apply_nmr
  * worked on the reduction voter bug more

### Week 16: August 9, 2021
* **Weekly Goals**:
  * work with Ben to separate SpyDrNet SHREC and SpyDrNet TMR
  * finish case study analysis for ethics group and turn it in
  * tests
* **Monday**:
  * added test for is_top_instance in spydrnet
  * added a design rule check for uniquify_nmr_property()
* **Tuesday**:
  * added .get_driver() attribute wire in spydrnet
* **Wednesday**:
  * added test got .get_driver()
* **Thursday**:
  * added more tests to spydrnet to improve code coverage
  * started reviewing what Ben had pushed to the spydrnet_tmr repo and started helping him with that
* **Friday**:
  * moved my updated code from SHREC over to the TMR repo
  * worked on the documentation and making sure it'll build

### Week 15: August 2, 2021
* **Weekly Goals**:
  * catch up with Ben and make a plan for what we want to do for the next SpyDrNet SHREC release
  * keep working on other DRC checks
  * note: I will be out of town Tuesday-Thursday
* **Monday**:
  * tools meeting
  * met with Ben, showed him my progress, and made a plan for SpyDrNet, SpyDrNet SHREC, and SpyDrNet TMR
* **Tuesday**:
  * worked on making insert_organs() able to support input pins
  * added is_top_instance as an attribute to instances in spydrnet
* **Wednesday**:
  * out of town
* **Thursday**:
  * out of town
* **Friday**:
  * insert_organs() should now be able to support both output and input pins.
  * insert_organs() can now be used to insert single reduction voters as well
  * made identify_reduction_points() compatible with insert_organs()

### Week 14: July 26, 2021
* **Weekly Goals**:
  * SpyDrNet SHREC documentation
  * finish the check for surface_pins() and think of other checks to do
  * work on case study for ethics broader impacts group
* **Monday**:
  * finished making drc_surface_pins. I added it to surface_pins(). It will run the check after surface_pins executes to see if the pins were successfully surfaced. If it finds a problem, it will print a warning.
  * worked on other documentation
  * started making a function that will go back through a design that has been replicated and voters inserted and then see if there are any spots where reduction voters got missed.
* **Tuesday**:
  * finished making a function that identifies reduction voter insertion points. 
  * added an example showing the drc in action.
* **Wednesday**:
  * wrote a function that finds the highest fanout flip flops in a design and returns their output pins. This is a simple voter insertion point algorithm
  * worked on SpyDrNet SHREC documentation
* **Thursday**:
  * made an organ that contains both a voter and a detector. Not sure how helpful that is but it was cool. It will vote like normal and also signal if that particular TMR domain is different from the majority vote.
  * worked on documentation
* **Friday**:
  * made a drc check for insert_organs()

### Week 13: July 19, 2021
* **Weekly Goals**:
  * finish cleaning up the drc code and finalize it
  * keep working on SpyDrNet SHREC documentation
  * do a spydrnet shrec release? Find a day to do that
  * do a spydrnet release? Find a day to do that
* **Monday**:
  * tools meeting
  * added the script for replicating 'nexys4ddr' to the SpyDrNet SHREC examples
  * worked on other documentation
  * added documenation for the DRC
* **Tuesday**:
  * SpyDrNet 1.8.3 release
  * worked on more spydrnet shrec docs
* **Wednesday**:
  * SpyDrNet SHREC 1.1.0 release
  * worked on documentation
  * meetings
  * travis CI should now be set up for SpyDrNet SHREC and good to go
* **Thursday**:
  * added some tests to spydrnet shrec and improved some of the existing ones
  * worked on the shrec documentation
* **Friday**:
  * started working on a small check to make sure surfaced_pins() works

### Week 12: July 12, 2021
* **Weekly Goals**:
  * learn more of the spydrnet SHREC functions (like pin_clock_domain_analysis, find synchronizers, surface_pins, etc.) and learn what they do to help in making documentation
  * finish reading the TMR paper
  * keep working on the nexys4ddr.edf and make sure it works through SpyDrNet SHREC
  * plan the next spydrnet release with the edf parser fix
* **Monday**:
  * worked on more SpyDrNet SHREC including making a surface_pins() example
* **Tuesday**:
  * added a little more to the documentation
  * worked on making the drc faster (it takes a while on big designs)
* **Wednesday**:
  * made drc faster and cleaned up the code
* **Thursday**:
  * did not work
* **Friday**:
  * did not work

### Week 11: July 5, 2021
* **Weekly Goals**:
  * figure out the possible bugs in SpyDrNet SHREC with Andrew
  * test my design rule check with more designs
  * actually work on my case study analysis for Ethics broader impacts group
* **Tuesday**:
  * worked on SpyDrNet SHREC documentation a little bit
  * looked at the bug and documented more examples in preparation for meeting with Andrew about it
  * spent some time looking through the apply_nmr() function in SpyDrNet SHREC. Found out that the problem isn't a bug in spydrnet SHREC but is from a bug in SpyDrNet, probably the EDIF parser.
* **Wednesday**:
  * looked through the EDIF parser a little bit
  * tried to figure out what pin_clock_domain_analysis in SpyDrNet SHREC does
  * read a bunch of the TMR paper (Jonathan Johnson)
* **Thursday**:
  * Did not work
* **Friday**:
  * spent some time messing around with surface_pins.py in SpyDrNet SHREC to try to figure out what it does and how it works
  * met with Andrew about spydrnet SHREC in general
  * met with Dallin about edif parser bug. He fixed it.
  * worked with Dr. Wirthlin, Andrew, and Dallin on getting the nexys4ddr.edf design to go through SpyDrNet SHREC

### Week 10: June 28, 2021
* **Weekly Goals**:
  * add docstring to pin_clock_domain_analysis and find_synchronizers functions explaining what the functions do
  * work on more tests for SpyDrNet SHREC
  * work on other parts of the SpyDrNet SHREC documentation
* **Monday**:
  * tools meeting
  * worked on making a design rule check that works for every example
* **Tuesday**:
  * worked half day
  * worked on making more little design rule check functions
* **Wednesday**:
  * improved one of my drc functions. Found a bug from it too, actually.
* **Thursday**:
  * worked on drc and started testing it with some bigger designs.
  * started installing Vivado 2019.1 to build Andy's RISC-V design
* **Friday**:
  * triplicated a ECEN 220 project and ran the drc on it. Found some interesting things (possibly bugs in the replication)
  * tried building Andy's tcl and python scripts but got stopped by errors 
  * found and contacted Dallin about a bug in the SpyDrNet edif parser.

### Week 9: June 21, 2021
* **Weekly Goals**:
  * look for other things that need to be added to the SpyDrNet SHREC documentation
  * improve docstrings on some of the SpyDrNet SHREC functions
  * come up with other checks/tests for SpyDrNet SHREC
* **Monday**:
  * fixed a part of the function used in the test I made last week
  * spent some time learning more about cables and wires in the SpyDrNet IR
  * then I added index() to wire documentation for SpyDrNet
* **Tuesday**:
  * met with Jordi to go over the release process
  * improved the spydrnet example I made (display_info)
  * experimented with accessing properties and other useful information of instances
  * added a test to feed the check_replication_by_step the wrong stuff and make sure it returns false
  * added a test to SpyDrNet SHREC to check the properties of instances in a replicated netlist against the properties of instances in an original netlist
* **Wednesday**:
  * added example to show uniquify_nmr_property() working
  * added test to test uniquify_nmr_property() function
* **Thursday**:
  * Did a small SpyDrNet release with Jordi and Ben
* **Friday**:
  * met with Ben and Andrew
  * worked on SpyDrNet SHREC tests

### Week 8: June 14, 2021
* **Weekly Goals**:
  * Come up with another TMR and DWC example that is slightly more complicated
  * finish presentation and present on Wednesday
  * add the rest of the SpyDrNet SHREC classes and functions to the documentation 
  * figure out what else needs to be added to SpyDrNet SHREC documentation
* **Monday**:
  * finished adding SpyDrNet SHREC classes and functions to documentation
* **Tuesday**:
  * added a little more to my presentation and practiced it
  * tried different things with SpyDrNet SHREC 
* **Wednesday**:
  * finalized presentation and presented it
  * other meetings
* **Thursday**:
  * added check_replication_by_step (module that will make sure the partitions in an original and modified design match up) to SpyDrNet SHREC tests
* **Friday**:
  * did not work

### Week 7: June 7, 2021
* **Weekly Goals**:
  * Keep working on SpyDrNet SHREC documentation: tutorial, start other parts
  * work on SpyDrNet SHREC example
  * get better at doing TMR and DWC for designs
  * work on IMMERSE presentation
  * work on ethics case study
* **Monday**:
  * tutorial page
  * meeting
  * Google guest speaker
* **Tuesday**:
  * worked on ethics case study presentation
  * finished simple TMR and DWC examples
  * finished SpyDrNet SHREC tutorial page
  * worked on SpyDrNet SHREC presentation
* **Wednesday**:
  * finished ethics case study presentation
  * presented ethics case study presentation in ethics impact group
  * other IMMERSE meetings
* **Thursday**:
  * added several pages to SpyDrNet SHREC documentation including ones about organs, functions, and voter algorithms.
* **Friday**:
  * worked on presentation
  * worked on another way to check the replication tool

### Week 6: May 31, 2021
* **Weekly Goals** :
  * spend some more time learning about TMR in SpyDrNet SHREC
  * work on SpyDrNet SHREC tutorial and examples with Ben
  * continue reading TMR paper
  * work on ethics case study
  * finish Bootcamp Vivado activities
  * figure out what to do next for SpyDrNet
* **Monday**:
  * HOLIDAY
* **Tuesday**:
  * tools meetings
  * worked on making a function to look at the paths in a circuit and compare it with itself after TMR (to see if the paths still exist). Basic way to check TMR tool
* **Wednesday**:
  * finished function that will load all the built in SpyDrNet example netlists, triplicate them, insert voters, and then make sure that the same paths in the modified netlist exist in the original netlist
  * meetings
  * worked on IMMERSE presentation
* **Thursday**:
  * finished up improving SpyDrNet tutorial
  * started working on SpyDrNet SHREC tutorial
  * spent some time learning the TMR tool
* **Friday**:
  * worked on IMMERSE presentation
  * added a page for voters and detectors in the documentation
  * tried out doing DWC

### Week 5: May 24, 2021
* **Weekly Goals** :
  * continue reading the TMR paper
  * explore SpyDrNet SHREC tools more
  * finish doing the new release with Ben, Jordi, and Dallin
  * continue working on SpyDrNet SHREC documentation - work with Ben
  * after new release for SpyDrNet, figure out where to go next
* **Monday**:
  * finished the 1.8.1 release
  * Bootcamp - FPGA Overview
  * worked on improving SpyDrNet tutorial
* **Tuesday**:
  * worked on improving SpyDrNet tutorial
  * looked at some issues on the SpyDrNet github
  * added instance_count function to the SpyDrNet SHREC example plot_generic_tmr.py
  * experimented with and learned more about SpyDrNet 'getter' functions and their parameters
* **Wednesday**:
  * worked on improving SpyDrNet tutorial
  * meetings
  * Bootcamp - Vivado
  * reviewed Vivado basics
* **Thursday**:
  * started working on a simple tmr example
  * worked on improving SpyDrNet tutorial
  * made small edits throughout the SpyDrNet documentation (mostly typos and such)
  * started working through the Bootcamp Vivado activities about tcl and testbenches
* **Friday**:
  * edited typos in INSTALL.rst of SpyDrNet
  * met with Andrew Keller and Ben to discuss more things about SpyDrNet SHREC
  * worked on making a function to look at the paths in a circuit and compare it with itself after TMR (to see if the paths still exist) 

### Week 4: May 17, 2021
* **Weekly Goals** :
  * add the two functions to help show the SpyDrNet flatten and uniquify examples working
  * help with the SpyDrNet 1.8.1 release. Learn how to do a release.
  * begin documenting SpyDrNet Shrec with Ben - make a plan for what each page will have 
  * write and submit summer proposal paper for IMMERSE
  * participate in Bootcamp and do the follow up activities to learn more
  * read up about TMR (the paper Jordi shared)

* **Monday**:
  * added function to SpyDrNet Flatten Netlist example to show the hierarchy of the netlist before and after flattening
  * added function  to SpydrNet Make Unique Instances example to show the definitions in each library before and after making each instance a unique definition
  * added functions to minimal.py to display the netlist created from scratch 
  * tools meeting
  * Bootcamp - unit testing
  * typed up research proposal paper
  * began reading paper about DWC
* **Tuesday**:
  * added display_info.py to examples - it contains 3 functions to help display netlist information. I originally added them to minimal.py but then took them off and did this instead
  * added a little more explanation to some of the example functions as well to explain the part I added (the functions to print the netlist hierarchy or libraries and definitions before and after to show it working)
  * experimented with pytest
  * finished and submitted research proposal
  * finished reading the DWC paper and began reading TMR paper
  * explored the TMR tool a little bit
* **Wednesday**:
  * wrote function to display number of times each primitive is instanced before and after triplicating. 
  * meetings
  * Bootcamp - documenting/Sphinx
  * spent some time looking at visualization tool from JensRestemeier in SpyDrNet issue #130
* **Thursday**:
  * added instance_counting function to display_info example
  * added link to JensRestemeier's visualization tool repo to display_info example
  * worked on SpyDrNet SHREC install page
  * worked on ethics case study
* **Friday**:
  * meet with Andrew and Ben over Zoom to learn more about SpyDrNet SHREC
  * Bootcamp - Docker
  * started doing new release with Jordi and Ben - merged all our branches

### Week 3: May 10, 2021

* **Monday**:
  * tools meeting
  * Bootcamp - Python
  * kept working on beginning learning SpyDrNet documentation
  * improved print connections function for netlists
  * read articles for Ethics
* **Tuesday**:
  * finished functions for displaying design information
  * cleaned up Learning SpyDrNet google doc
  * made more edits to mostly spelling in documentation
  * made markdown version of cheat sheet
  * reviewed other SpyDrNet examples in the documentation 
  * finished reading articles for Ethics
* **Wednesday**:
  * added definitions cheat sheet and tips for learning spydrnet to the wiki
  * also learned more markdown as I did that
  * meetings
  * Bootcamp - python
* **Thursday**:
  * added personal website link to CCL website
  * python bootcamp follow up activity - csv_parser
  * learned about is_downto, is_scalar, and lower index from Dallin
  * looked through spydrnet wiki and read all that
* **Friday**:
  * got set up with the spydrnet-shrec repo
  * learned about hierarchal references
  * came up with a list with Ben of starting points for spydrnet-shrec documentation
  * experiment with the TMR tool with Ben
  * Bootcamp - Python

### Week 2: May 3, 2021

* **Monday**:
  * tools meeting
  * bootcamp - VSCode
  * worked on assigned SpyDrNet issues
* **Tuesday**:
  * got started on fixing minor errors in SpyDrNet documentation
  * worked on Issue #130 for SpyDrNet
  * figured out parts of SpyDrNet like instances, references, children, parents
  * tried out SpyDrNet by parsing my FourFunctions project from 220
* **Wednesday**:
  * began documenting things I've done to learn SpyDrNet
  * meetings
  * Bootcamp - make
* **Thursday**:
  * learned more about cables, wires, ports, and pins in SpyDrNet
  * wrote functions to display information about netlists
* **Friday**:
  * continued to learn cables, wires, ports, pins
  * talked to Dallin about inner pins, outer pins, metadata, EDIF.properties and Verilog.properties dictionaries
  * practiced writing various python functions to show connectivity of design
  * Bootcamp - CMake

### Week 1: April 26, 2021
 
* **Monday**:
  * computer setup
  * linux tutorial
* **Tuesday**: 
  * linux tutorial
  * website setup
  * started looking at spydrnet
  * other various computer setup things
* **Wednesday**: 
  * meetings
  * BootCamp - Git
* **Thursday**:
  * learn Git
  * finished website setup
  * ethics outreach reading 
* **Friday**:
  * met with Dallin about SpydrNet
  * learned more SpydrNet
  * ethics outreach reading
  * BootCamp - Github
