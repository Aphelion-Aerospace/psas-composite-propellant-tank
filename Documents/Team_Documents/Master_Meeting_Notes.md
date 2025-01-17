#2017-04-27 

**Results from last week’s workflow:**

Chris:  Gasket markdown procedure pushed, CAD Readme started, modified gasket mocked up, just needs to be cut, templates will be cut as soon as acrylic arrives.

Weldon:  Beginnings of procedure template started, brought it up to his work contact, sounds like she is willing to read through things/help approve the process/template to make it more professional.  Still needs to tolerance shrink fit designs

Alex: Sealant arrived, did some endcap/ring shrink fit calcs, ordering etc..

Francesca: Git updated, analysis converted to jupyter notebook, outside testing places contacted

Russell:  Need a bit more time on shrink fit calcs, shrink fit CAD (it is "finalized", has floating dimensions, how much you intend to compress liner, & how much to interfere Al parts)...added delta of compression to the PTFE in the layout sketch. Russell will be running comparison calcs against alex’s

Neil: FEA (modeled 6 ply 0,90,-90 CF epoxy tube with 4000N static loading on one side to begin flight sims, deformation in the .001" range), documentation/organization

**Discussion:**

-Are we going to etch these PTFE tubes?

  -leaning towards maybe etching 2? And incorporating an etched design into a flat end cap, like our very first design iteration, so we have something to try f the sheet liner fails

 ETCH 2 

	-CAD is done already, need STEP file or part file sent off to protolabs to get ordered/quoted

	-means when tubes get here we need to get them turned around and sent off for etching ASAP

	-Chris is getting ball rolling on etching

	-Shear analysis needs to be completed on adhesive surface in general (peeling tension)

-Still need to figure out bridge material/method for sheet design, mats we have may not work

-Add keyway to shrinkfit design to get stuff lined up?

  -this will be dependent likely on experiments below:

-Russell is emailing prof at PCC to see if we can use their laser extensometer(?) for measuring strain of shrinkfit stuff, measuring diamater of cap etc accurately

-Machine faux endcap/ring to test shrink fitting (Fri morning?)

  -Get model made and sent to Mike to see how toleranced it can be on the CNC

-Additionally, try turning down PTFE tube on lathe this day (4/28)

  -Probably worth trying to investigate if it is possible to turn down ourselves

  -Will need to get ahold of LN2 for shrink testing with faux rings etc

  -Need LN2 receptacle for submersion purposes

-Cut our own rings/ptfe and submerge in LN2 and measure ourselves? (per Chris, would like to run this experiment to determine our own coefficients to compare to research)

-Bag Design?

  -Let’s go ahead and investigate this

-Final report lead:Neil/weldon/francesca?

-Need to discuss shrink fit design(done)

**Task designation/discussion:**

*Since no meeting with Dr Jiao this week, let’s go ahead and do this preliminarily today so that Friday can be a workflow day.*

Prelim tasks (pending discussion):

  -More FEA (Neil/Alex/francesca)(ck)

	-Thermal strain hand calcs @ adhesive interface (alex/russell)(ck)

	-Start final report formatting/outline/info: Need final report lead: (neil/weldon?)(ck)

	  -develop & talk to gerry + dr jiao to see if it is in-line with what they want

	-Material properties workbook so it is all in one place and we don’t have to reference stuff in multiple locations (alex has started this already) (done, please update as we go)

	-Ring machining capability in house, with Al stock we already have on CNC?(chris/weldon) (will be decided tomorrow)(ck)

	  -likely will need like 30 min of CAD (russell) to alter design to make it more just a flat top ring, the going into the shop with Kris to get it done on mastercam

		-Shrink fit cap will likely be basically same geometry

	-Develop outline/documentation procedure for Layup (weldon/neil?)(ck) weldon should have talked with his work contact already at this point

	-Prep experimental procedure/documentation etc for hydro/ln2 testing on layups so this is more a fill in the blank process (francesca has a test excel doc)(weldon) (should be done before end of weekend)(ck)

-Drawings out for CAD stuff as well to be sent to protolabs (Russell)(ck)

-prepping layup procedures, gaskets cut, templates cut (chris)(ck)

-bridge design on how to hold it, pop can?  Needs investigation for layup (chris)(ck)

-clean up CAD naming scheme, rename CAD folders to be inline with part folders etc (chris./russell)(ck)

-additional analysis if required (russell)(ck)

-Francesca: documentation.fea,coupon tester guys, jupyter notebook (ck)

*If parts get here:*

	LAYUPS:

   -2 layup squads?

  	-if parts here, likely to at LEAST 1 layup on thurs or fri to start accelerating the timeline



# **2017-04-16**

Updates:  What’d we get done this week?

* CAD finalized (for the time being), Technical drawings completed
	* FEA Full modeling process started (Meeting with John/Ian) (Neil/Alex/Francesca)
		* Further contact from Ian regarding analyzing buckling of composites (this is probably beyond the scope of this project), try to learn as much as we can about the weave, core, elastic modulus, & try to define the sandwich as a whole as opposed to each individual layer.
	* Potential Sealant found (Per Russell)
	https://www.wrmeadows.com/poly-jet-lox-low-modulus-joint-sealant/
	* Chris is setting up a time w/ MELT to do PTFE laser cutting test
	* Contacted Masterbond (adhesive is expensive), Jupyter notebook tutorial started/pushed to git,
	* What Weldon accomplished this week: (started collecting eqns for stress analysis on flat plate end cap) (basically just prep work & some minor analysis at this point so far)
		* Weldon has FE exam this week so some of this time will be committed to that

Part numbering convention:
####-A (first two digits are type of part, i.e. rings or end cap...etc, last two digits are iteration #)
* Liner: 01 series          Example: 0101 is first liner iteration, 0102 is second liner iteration
* Rings: 02 series
* End cap: 03 series
* Al Tape: 04 series
* PRV pipe: 05
* Gasket: 06
	Letters refer to various versions, such as tube liner vs sheet with seam liner
Example: 0201-A is ring designed for sheet liner iteration 1, 0201-B is ring designed for tube liner iteration 2.

> A=Sheet liner, B=Tube liner
	
	

**Thoughts:**  
 
* 2nd iteration ring designs?  Pretty good idea, let’s start to analyze for 2nd iteration of ring designs.  This design would alleviate any Etching concerns as it could be accomplished with virgin PTFE + additional gasket.
 
* How do we show a FS=2 empirically for this tank, or on sealant?  We will have to break a lot of tanks….

* Previous teams’ book as a reference..(now around our work area)  they did a TON of work on the airframe stuff, there is likely a lot of data we can simply reference to speed things along

* Focusing on the procedure being scalable is a good idea.  Even though we do not know for certain what the scaled up model will be, we can just choose something arbitrary (aka 10”) so show that things will scale down the line.


For next week: (....) designation afterwards for my purposes only ~NB
	
  * Start researching LOX compatibility more thoroughly (pushed)
	
  * Being FEA full modeling (Neil/Alex/Francesca?) (pushed)
	
  * Order caulking/sealant/permabond this week (ig)
	
  * Order some of those teflon bags to investigate if it will be feasible to include (ig)
	
  * Send off designs/drawings to be machined (1 or 2 replicates?) to begin stage 1 prototyping.  Stage 1 will help us develop the layup procedure for this tank (which is one of the major deliverables for PSAS) as well as providing us with burst test data. (Chris/Weldon) (ig)
	
  * Drawings of 0201A and 0201B will be finalized before 5pm tomorrow (4/17) (Chris)(ig)
	
  * We need to get our hands on LOX and start doing compatibility testing….developing testing procedures/what test? (Need to go to liquid test stand meetings since they are really close to getting some LOX)(If nothing else, let’s get regular contact with them to make sure they can order enough for us to be able to use) (pushed)
	
  * coupled with obtaining LOX, we need to develop what tests we want to do with it, as well as procedures/safety etc regarding LOX testing….(pushed)
	
  * worried about LOX ignition, and oxidation
	
  * Testing etched surface in contact with LOX to see if there is any chemical incompatibility
	
  * Further refine heat transfer analysis (Alex/Russell)(pushed)
	
  * Prelim gasket stress analysis (Russell is waiting on that gasket book, won’t be here for another 5 days or so) (Russell)(solved)
	
  * For all analysis, start moving towards converting to Jupyter Notebook (per Francescas tutorial stuff on git/drive)
	
  * Chris is setting up time w/ MELT for PTFE test laser cutting, as well investigating what scrap acrylic is around for cutting templates.  If nothing else, can go to TAP plastics and just buy some(pushed)
	
  * Consider using  keg ball-lock connector/fitting, keep on back burner for now we will investigate more later (pushed)
	
  * Schedule another LN2 testing time for perform further tests (pushed)
	
  * Literature research party, literary research for composite material
	
  * Start experimental lab write up documentation procedure(from last weeks list)(pushed)
	
  * Spray on chemical insulation research (from last weeks list)(pushed)
	
  * Convert all of these ‘tasks’ to the issues tab on Git, & keep converting everything to Git (Neil)(done)
	
  * Potentially start working on 2nd iteration ring/endcap design (Russell)(pushed)
	
  * Are there any additional things we need to consider/develop for hydrotesting?

** Task focus: **

  Russell- Ht xfer/gasket analysis, then CAD (pushed)

  Alex- Ordering, Heat xfer refinement (pushed)

  Weldon-Stress analysis started last week (FE is on wed, so likely will not be accomplished until wed/thurs) (pushed)

  Chris-Finish drawings/get sent off, get MELT stuff arranged (pushed)
	
  Francesca-LOX compatibility research/cals, transport theory (pushed)
	
  Neil- Git,  get FEA started, manage stuff, help out with analysis etc (pushed)
	
	



# **2017-04-09**

Thermal Cycling experiment completed on Fri 17/04/07
	-No visible delamination or issues after submitting test coupons to 1/3/5 full thermal cycles.  All seemed to hold up well, if possible would like to generate more (more than simply 3 preferably to get some actual statistical data) coupons to run either another thermal cycling with LN2 or LOX if possible.
	-Old module frame from crush test was also submitted to Thermal Cycling, this was submerged for ~10-15min, and the ring/module/adhesive all held up very well when submitted to LN2.  Results promising, again, no visible delamination/damage/etc.

Alex made contact with Robert Watzlovick (Guy from that website who did the DIY rocket that we went over in a meeting with Dr Jiao)
-He said his LOX tank failed at cryo temps, we will maintain contact as he was interested in our project.

Problems:  Let’s make a list, as per suggestion by Gerry.
-Obtaining Liner (in general).  Get sheet/tubes here to be worked
-Etching is dangerous! (http://www.plasticsmag.com/features.asp?fIssue=jul/aug-01&aid=3284)
-Budget: need to spend all of it.  Order more stuff, maybe order stuff for EFS if they need anything?
-Machining endcaps/rings, in house/sending off designs
-More stress analysis/calculations
-PTFE machining, PTFE problems...Effing PTFE….
-How do we machine our gaskets?
-Where can we get LOX? Can someone help us with this test? Where do we test?
-How do we perform stress analysis on the composite layers? (contact Ian Zabel)
-FACTOR OF SAFETY OF AT LEAST 2.0 (COLLECTIVE) + calcs to back up
-PRV/Fittings for end caps
-..

PTFE Machinability, how do we go about it?  Create matrix and figure out our BEST working 
option so that we can make the best possible decision to move forward with (as per suggestion by Erin)
Let’s iteratively work on this for a week or since we are waiting on the stupid tubes/rods anyway, and we are at least running tests with a bridge design using PTFE sheet instead.  The matrix for analysis on the BEST possible method is on drive, so if we can formulate the matrix and then sit down and smash through it here in the next week or so that’d be great.  This is in order to determine the BEST possible option of how to machine or turn down PTFE to a thickness/workable form that we want, rather than just moving forward with something that we think “yea this will probably work” & screwing ourselves.

What else can we accomplish this week?  What other decisions need to be made?

-Alternate adhesive -> HYPERLINK "http://www.masterbond.com/articles/applications-research-labs-and-commercial-use-ep21tcht-1?utm_source=ep21tcht-1-researcharticle&utm_medium=email&utm_content=ep21tcht-1-researcharticle&utm_campaign=cart"ep21tcht-1
Recommended by Masterbond given our application (data sheet in materials folder) 
 	-Will call Monday (Francesca) to request sample adhesive.

-Getting designs sent off to be machined
-Need to get this done by Wed 17/04/12.  Let’s get rings/endcaps moving forward.
Liner
-Layup procedure with sheet as opposed to PTFE tube
	-Bridge design idea or try to chamfer ptfe and adhere PTFE to PTFE?  Likely would need a self etching we could do here to accomplish the latter.

-Investigating DIY PTFE etching procedure to save time
	-Bonding primer/adhesive
	http://www.permabond.com/2015/06/10/bonding-ptfe-industrial-adhesive/
	-Customizable teflon bonding kit
	http://reltekllc.com/productlist/teflonbondingkit.aspx

-Etch 3-4 ptfe tubes when they arrive in 2 weeks 

-TO DO THIS WEEK:  Order Permabond alternate etching and some virgin PTFE sheet (even just janky samples) to perform this ‘in house’ etching/adhesion

CAD (Russell/Me(Neil), think you can jump on this and try and get it done by midweek?)
- We need to finish CAD and send it off to a machine shop
-CHANGES: Offset portion, we do not need to have the offset on the lapping portion with a PTFE bridge design, can revert to the previous airframe ring design (ish)
-BRIDGE DESIGN:  Needs to be finalized.  A few different options are available, over/under design? How to adhere? Etc..

Machining
-Gaskets need to get machined.
-Designs sent off, practice machining in house.


Looking forward

-I’d like to get our first layup done here in 1.5-2 weeks.  This means getting designs sent off, gaskets fabricated, hardware ordered (if changed), valves figured out, & a PTFE sheet mounting method finalized to try (if we want to do a layup with PTFE in it, otherwise we can do one without and do a burst test just on the CF tank layup.

-Perform stress analysis on endcap/fasteners/rings.  Likely should do FEA & back of the envelope calculations to try and nail down factor of safety of at least 2 (per PSAS)
-Meeting with Erin/Andrew on Thursday 17/04/13 @ 1pm after our meeting with Dr Jiao, in the LiD.  Erin will be walking us through a markdown format procedure for GIT. We will also discuss purchasing additional material that PSAS can use after our project is over. As well, we can take care of that first assignment for Gerry since we have to meet with our sponsor and write something up, so we need to prep that.  
-Additionally, need to finalize a few items to give to PSAS for the leadership meeting on wed 17/04/12 so they can present some of the stuff we are doing.

-We still have a substantial budget.  We need to spend ALL OF IT.  Start ordering/organizing/thinking about additional/extra materials etc to burn through this remaining budget.  Maybe even can order stuff for EFS team if they need something.

TASKS
-Neil/Russell-CAD (done)
-Neil - Prelim FEA on endcap stress analysis, Experimental write ups for past/future experiments (need proper documentation) (doneish)
-Alex -Ordering many things/Al Sheet for endcaps & test coupons, getting the ball rolling on sending designs off to be machined so it’s ready to go come CAD finalization, lab write up for thermal cycling of coupons (nearly done)
-Chris - emailing MELT to see if they are comfortable lasering PTFE, as well acrylic template for cutting for layups, formal quotes for PTFE etching, PTFE gasket machining (done)
-Weldon - back of the envelope stress analysis calcs for flat endcap/bolt sizing (???)
-Francesca - Heal up, can help Neil with FEA, talk about what else to get done during meeting tomorrow (Monday 17/10/04 with Neil/Russell) Convert current analysis to Jupyter notebooks, setup Jupyter/Git tutorial - transition to Git as primary team storage mechanism.Contact masterbond for sample adhesive. Research sprayon chemical insullation. (mostly done)


	


# **2017-04-03**

-Set date for thermal cycling of test coupons T7.1-T7.3, Friday? Earlier if possible?
	-Friday before 4pm, let’s get this arranged

-Release valve/adhesive results from last week, which do we move forward with/get ordered.
	-Waiting on quote about adhesive, seems interesting let’s try and move forward

-What else still needs to be ordered?  Need to get everything on it’s way.
	-Returning heat gun accessories 
	-Machine time quotes w/ CAD designs

-CAD updated/machine shop found?
	-Alex found machine shop that seems feasible, for both metal and plastics, let’s move on this

-Prep items/discussion for assumed Thurs meeting with Dr Jiao.  Likely show test coupons, discuss what has been ordered, show faux tensile testing experiment from finals week etc.
	-Do we need to reserve room for this timeslot again? As well we need to check with Dr Jiao if 12pm still works for her this term.
	-Room already reserved, good to go

-Beginning of “down time” where we are waiting for parts, what can we accomplish? Machine shop work on rings/end caps?

-Other topics/concerns?

Additional topics to take care of:

-Talk to Mike about boring out PTFE

Chris: PTFE- if quotes come in at same time, get from both vendors
	-OD:3”

# **2017-03-27**

Need to set date/time, how about Sunday @ 6pm, or Monday @ 6pm?

This agenda serves as a guide/preliminary decision making prior to the meeting, just to get all of us thinking about what needs to be done so that we can finalize and move forward during our meeting here in the next few days.

There are a few items/decisions that need to be finalized, as well, we need to move forward asap to the prototyping stage.

Ordering:  We need to get things ordered ASAP.  With this term coming to a close, and lead times stacking up, we need to get everything that we need ordered and on it’s way.  Hopefully we can get everything finalized and ordered by the end of the week, 3/31/17.  Preferably, we need to order enough key items so that when things arrive in 2-3 weeks we can construct at minimum 2 or 3 prototypes for testing. With how much time we have left coupled with lead times for all of these materials/parts, if something needs to be changed we will likely only have time for 1 iteration if we only order enough for 1 or 2 prototypes at a time.  Things that still need to be ordered with extensive lead times are as follows:

	-Nomex
	-PTFE
	-Teflon bag liner(http://www.welchfluorocarbon.com/custom-manufacturing/heat-sealing/)
	-Aluminum for in house machining
	-Mating Rings
	-Endcaps
	-Additional fasteners/fittings for hydro testing
	-???

In regards to the list above, we can move on to a few discussion items/decisions as detailed below.

Mating Rings, Endcaps, In-House Machining

In-House Machining:  I do believe this is a good idea for the low cost, open source nature of this project.  However, there will be a fairly steep learning curve as none of us have extensive machining experience, not to mention we will need to arrange time with Mike/others in the machine shop to show us everything/supervise etc.  As well, we are working within some tight tolerances so there will definitely have to be some practice involved.  It has been discussed between a few of us already that we may want to lean towards sending off designs to a local shop to have them do it for us.  I propose that we do both.  Since lead times are involved, I propose we send off designs to a machine shop (minimum 2 replicates so we can construct at least 2 prototypes) to be professionally machined.  This is so at the very least we will be able to have in our possession rings/caps that WILL work within our tolerances.  This will require CAD models being finalized/drawings created by early in the week so that we can get quotes and send off to a shop.  Since this will likely involve at least a week or 2 lead time, we can get ahold of aluminum and use this time to try and beat the learning curve in the machine shop and practice fabricating pieces ourselves.  


 
Name Agree Disagree Comments  
 
Neil +    
 
Russell +    
 
Alex +    
 
Francesca +    
 
Chris +    
 
Weldon     

Mating Rings:  These designs are nearly final, though with Alex discovering the Teflon Heat Liner ( http://www.welchfluorocarbon.com/custom-manufacturing/heat-sealing/), it makes me think this may in fact be a cheaper and quicker option than the PTFE, while still achieving the same desired effect & quality of tank.  If we elect to use this ‘teflon bag’, it means that the ring designs will change slightly.  As mentioned above, I think we could in fact do both, especially if we send off designs to a machine shop.  We will just have them fab the 2 different designs, and we can compare layup procedures/effectiveness of each if we construct both models.  This can also be accomplished by us in the machine shop while we are waiting on lead times.  These are the designs that I am thinking of:

 (1) Same PTFE design with offset lapping portion to allow PTFE to be inner layer of the tank:





(2) Alternate design for Teflon Bag, with no offset portion, similar to below:



Using this secondary design with a teflon bag, we could even potentially ‘double line’ the interior, incorporating one layer into a layup, and then lining the inside of the tank a second time post curing process.


 
Name Agree Disagree Comments  
 
Neil +    
 
Russell +  I think we exhaust the liner possibilities before giving up and moving to the bag. I think there is a possibility that we can lay up onto a thicker tube, then bore it out afterward with the challenge of getting a good surface finish.  
 
Alex +  Our current liner design is the better option, but at least the bag can serve as a backup.  
 
Francesca +  ^This^  
 
Chris +    
 
Weldon     

End Caps:  As discussed preliminarily between a few of us, I think the end cap design can be simplified to just a flat plate design.  Under our operating pressures having a curved geometry for an end cap is likely unnecessary, as the stress concentrations will be occurring at the joining interface and fasteners of the tank.  Not to mention a flat end cap would be much easier to machine, both in house and by a machine shop.  We could move forward with this alteration of a design for at least the initial prototyping stage, and if it appears that we need to alter them back to a curved geometry then we have that possibility. 


 
Name Agree Disagree Comments  
 
Neil +    
 
Russell +  What Francesca said, but we can always use a nipple with gaskets and nuts, which won’t handle as much pressure, but may handle enough  
 
Alex +    
 
Francesca +  If we are doing a flat plate, I think we should consider shaving down a thicker plate to allow for a thin wall with a thicker center-section that can be tapped through and used to mount inlet/release valves  
 
Chris +    
 
Weldon     


Additional Considerations:  If we can get everything ordered and underway, we will have a couple weeks of just waiting around for things to get here.  During this time, as mentioned above we can work in the machine shop, but as well work on acquiring additional necessary resources, as well as performing tests.  More coupons can be created for thermal cycling, which means we can find a source of liquid nitrogen for said testing (hopefully from the PSU chem department for ease of access), as well as methodology and a location to be able to perform these tests.  Also, if we can get a sample of the teflon bag in our possession rather quickly it would be nice to run a set of coupons using this material as we have with the PTFE to see how it holds up against METLBOND and the CF curing procedure.

Adhesive:  Need to look into backup adhesive (do some research into company Masterbond), in case METLBOND isn’t going to cut it..

DECISIONS:

-Move forward with Flat End Cap
-Move forward with 0.25” wall thickness PTFE, 3” ID, with etching, get quote, get it rdy to order asap (5 replicates)
-Fab 2 designs, one for teflon bag, one current design

# **2017-03-09**
--------------------------------------------------------------------
**Progress**

On 3/5 we did some test layups with the virgin side of PTFE to assess the melt bond’s ability to adhere.

One PTFE on aluminium

One PTFE on carbon fiber

One PTFE on nomex

Additional test measurements on the shrink tape

**Updates **

*(short statement of results we can talk about process after the meeting if anyone has questions)*

Additional test measurements on the shrink tape (needs to be re-done, failure during heating process)

All adhesive failed on virgin side as expected

Erin want’s us to to 3 inch

He wants us to go simple with caps

We will have to explain to Gerry that are design considerations are being shortened.

**Weldon**

**Francesca**

**Neil**

Concerns with METLBOND 1515 & LOX

*From Metlbond Data Sheet… see meeting_notes/media/media folder for image01*

Would like to run simple test with coupons + metlbond asap, (ex submerging in small amount of LOX) to test degradation/speed of potential failure...may not have immediate effect and will work out OK

**Russell**

**Chris**

**Alex **

Got budget done. Let’s start spending money.

No overhead taken out of the award

Check the units on the ipython notebook optimization

[*www.Watzlavick.com/robert/rocket/rocket1*](http://www.watzlavick.com/robert/rocket/rocket1)

**Whats Next?**

(Time to make decisions on what we need to do next week)

# **2017-03-02**
---------------------------------------------------------------------------

**Progress**

On 2/26 we did some test layups with the chemical etched PTFE to assess the melt bond’s ability to adhere.

One PTFE on aluminium

One PTFE on carbon fiber

One PTFE on nomex

We also did some preliminary test measurements on the shrink tape

**Updates **

(short statement of results we can talk about process after the meeting if anyone has questions)

Weldon

I’ve been sick most of the week, and haven’t made much progress. I should have the notes from the safety training up in the next couple hours. I’m also putting the finishing touches on the documentation procedures. I’ve been gathering safety documentation as well. I’m also trying to gather documentation on standard LOX tanks and filling procedures.

Francesca

Neil

Russell

Chris

Alex

**Whats Next?**

(Time to make decisions on what we need to do next week)

#**2017-02-23**
--------------------------------------------------------------

**Progress**

**What we said we would do**

Alex- Weight reduction on cad models, follow up on contacts for quotes on donations

Russell- More research on PTFE, Spend some time looking at strength and permeability.

What is the pressure from shrink tape?

Baseline thickness of PTFE liner

Weldon- going to chem safety training contact gas suppliers, put together a documentation standard

Neil- FEA heat transfer analysis

Francesca- FEA play around with different materials , abstract for AIAA, meeting tuesday about python.

Chris - Get quotes for PTFE liner, What kind of surface treatment do we use, Continue to move things to github and make issues.

**Alex**

**What did you do?**

Looked at aluminum suppliers and possible endcap manufacturing options.

**What do you need?**

Get together and talk about design

**Whats next?**

Send budget to jun

**Chris**

**What did you do?**

We have samples!

Requested quotes from APT and these guys.

[*http://catalog.fluoropolymerproducts.com/viewitems/all-categories-molded-teflon-cylinders/ries-molded-teflon-cylinders-molded-ptfe-cylinders?&bc=100%7C3001036&os=y*](http://catalog.fluoropolymerproducts.com/viewitems/all-categories-molded-teflon-cylinders/ries-molded-teflon-cylinders-molded-ptfe-cylinders?&bc=100%7C3001036&os=y)

[*http://www.enflo.com/products/molded-ptfe-cylinders/*](http://www.enflo.com/products/molded-ptfe-cylinders/)

[*http://technetics.com/products/ptfe-polymer-solutions/ptfe-shapes/rod-and-cylinders/*](http://technetics.com/products/ptfe-polymer-solutions/ptfe-shapes/rod-and-cylinders/)

**What do you need?**

**Whats next?**

**Call enflo about Molded PTFE Cylinders (1-713-983-4201)**

**Neil**

**What did you do?**

[***https://drive.google.com/open?id=0B26o6W76DxOec291OEVBQlhRY0k***](https://drive.google.com/open?id=0B26o6W76DxOec291OEVBQlhRY0k)

Made SS thermal stress FEA

Deflection as a result of cryo cooling

Found out how to move solid models to abacus

Worked on AIAA abstract

**What do you need?**

Solid models

**Whats next?**

Vibrations?

**Francesca**

**What did you do?**

Working on AIAA

**What do you need?**

**Whats next?**

**Russell**

**What did you do?**

Sizing for the thickness of liner

Back of envelope calculations based on a 1mm material thickness.

6\*7\*.04 cylinder is about .41 lbs

Permeability 5.86cm^2 O2 lost per hour (possibly not an issue)

Yield strength of PTFE about 182 psi at 175 c (from linear interpolation)

> Max pressure on cylinder is about 2.4 psi (we won’t be able to layup on this)

Insulation properties (not great at the thickness we are looking at)

> [*https://drive.google.com/open?id=0B80-Nm0s3cT6VXhIdFNLOGdUNmM*](https://drive.google.com/open?id=0B80-Nm0s3cT6VXhIdFNLOGdUNmM)

Take away

PTFE will only be useful as a LOX barrier. Go as thin as possible!

**What do you need?**

**Whats next?**

**Weldon**

**What did you do?**

I went to the chemical safety training. Some good information there about safety and emergency services. I’m working on writing up a sheet of notes for easy reference.

Started work on a documentation procedure document. Not quite finished yet.

Have been researching LOX suppliers, storage containers, and filling procedures. I’ll put together a sheet about this as well (likely I’ll get this done just after I get the documentation procedure finished up).

**What do you need?**

**What’s next?**

Finish creating the documentation procedure, and follow it while producing note sheets on the safety training and general LOX information.

Follow up on some research concerning regulations and codes associated with the use of LOX as part of the fuel mixture for LV4.

Explore concerns about how long the LOX will remain in it’s liquid state under the current design conditions.

> What issues might need to be addressed if the pressure of the expanding gas exceeds the design pressure?
>
> Would that cause any catastrophic problems in the fuel pump system?

# **2017-02-16**
----------------------------------------------------------------------------
Alex showed off some designs he modeled

Need holes and weight reduction (we still need to refine the thickness)

Now that we have a model we can get a quote for PTFE liner

Indium lining of interface

Do we want to account for insulating materials

> Foam or vacuum
>
> With such a small gap will insulation actually help
>
> Nomex will also help insulate
>
> Let's not worry about it

Limiting factor for aluminum is how thin we can machine it

Thin wall pressure vessel calculations

For the pressure we are going for the an aluminum tank would be very thin

Permiability of O2 through PTFE

What we are looking at is at room temperature

Document everything

Nasa want reports from us

Show them that we are doing things

They want “nuggets”

Test coupons

How are we going to create them ?

What are the specks of the test coupons for testing?

Lab in ondine does not want a bunch of students to using the lab.

Perhaps they will do the testing for us.

This would be great!

It would be great if testing was our least concern

How do we want to test them

Margaret is our contact for money.

Lets buy stuff local if we can and reduce shipping cost

Prototyping

How are we going to load the tank with pressure

Will it seal cold?

Air gas and matheson

Let's talk to them and get some info

Talk to them online

**What will we get done this next week**

Can we find someone to stamp out an aluminum endcap?

What sizes do they have available?

We can then order more than one

Alex- Weight reduction on cad models, follow up on contacts for quotes on donations

Russell- More research on PTFE, Spend some time looking at strength and permeability.

What is the pressure from shrink tape?

Baseline thickness of PTFE liner

Weldon- going to chem safety training contact gas suppliers, put together a

Neil- FEA heat transfer analysis

Francesca- FEA play around with different materials , abstract for AIAA, meeting tuesday about python.

Chris - Get quotes for PTFE liner, What kind of surface treatment do we use, Continue to move things to github and make issues.

# **2017-02-09**
------------------------------------------------------------------
What have we done, what will we do, is there anything holding us back?

[***Action Plan***](https://drive.google.com/open?id=1IFkCph4sUu5lX_zHoPREmssZP85U279T_9PHecbIcHA)

**Contacts**

Made contact with APT Teflon working on getting samples(most likely get them) They may be able to manufacture a liner that we can then layup on top of. (potentially).

Made contact with Jerry from 3M aerospace tapes and adhesives department. Looking into scotch weld. (Haha)

**Modeling**

Has anyone modeled anything yet?

No

**Finances**

We were told by Andrew that if there are more financial concerns they should be directed towards him.

We have to pay for shipping of samples andrew is paying with cc

**Documentation**

GIThub tutorial in the rocket room 1 pm, 2/9

Let’s get some end cap drawings

**Design**

[*https://drive.google.com/open?id=0B\_82kiJ5gcsyR2Eya3JLbmswQUE*](https://drive.google.com/open?id=0B_82kiJ5gcsyR2Eya3JLbmswQUE)

-Arbitrary tank design dimensions: **4’’ inside diameter, 8-¾’’ inside long** or 6’’ diameter, 13 inch long

-**Tank working pressure around 3 atm**

-Pump team is optimizing pump to work with tank pressure between 2 - 3 atm

- Timeline to complete design phase in 6 weeks

What do we need to accomplish?

Who is going to accomplish these tasks?

-we may need a thermal buffer at the ends

-what kind of shape

With regards to thermal coefficient (show in our design that we are considering this)

How much will the hemisphere contact

> **Timeline**

16 weeks to get everything done

Iteration every 2 weeks. By the third iteration hopefully we will nail down our design 2/16

When we send thing to manufacturing we will plan what we will do while we wait

**Presentation **

Problem 1: thermal expansion diff (Francesca)

Problem2 : How do we manufacture (interfacing and manufacturing)

If we can just layup everything in one piece (Neil)

Problem 3: seal (Weldon)

**Meeting With Jun**

We have leveraging for money

Too many tests can be a waste of our time

We should be confident with our design

Lets only do meaningful tests

Do we have potential vendors

Machine science( has helped PSAS)

ProtoLabs

Check Ebay or alternative sources (can we recycle things?)

Can we find a teflon tube somewhere else

**Things to do**

1.  Presentation slides: Neil, Francesca, Weldon

2.  Team Contract Revision: Chris, Russell, Alex

3.  Test meltbond

Test every one of our interfaces individually

-machine shop to cut Al

(alex will come in tomorrow)

-Layup on Sunday: Alex, Francesca, Neil, Chris

9 Am

4) FEA Donut thermal analysis: Neil, Francesca

5) Design Options: decision made during 2/16 meeting

#**2017-02-02**
-------------------------------------------
-   We meet trishia

    -   Requirements for OSGS

    -   We need to come up with the matching funds

    -   Alex has been great

    -   She has concerns with the budget

        -   We were awarded 8000 trisha thought we needed to raise 24,000

        -   We clarified that we have a bunch of donated materials

        -   Maybe get a contract from psas

        -   We purchase through psas for the 2000

        -   **We need to talk to andrew (get a contract for $2136)**

        -   **We need to make trisha’s job easier**

            -   Trisha has less worried now

        -   **No spending OSGS funds yet**

        -   Is someone going to take a cut out of our money?

            -   Subcontract

            -   Overhead

            -   We may see less than 8,900

            -   Probably 5%

            -   We need to be very careful with spending and documentation to make the university and NASA happy

            -   Boeing has was compensated last year for their donation

            -   Make lasting relationships and good connections to open bridges and keep them up.

    -   Team roles

        -   We need to come up with a way to evaluate members

        -   Let’s get rolling on this 16 weeks left

    -   What should jun expect next week

        -   We are doing a layup on sunday 9AM

        -   **We should meet more.**

        -   Do we want to make Gerry happy or PSAS

            -   Making gerry happy will fall in

        -   Make a plan for who will do what

        -   Not everyone needs to do everything

    -   Action plan

        -   We have a list of tasks that we need to do lets divide the tasks by subteams.

    -   Jun’s question

        -   Do we want to look into professional manufactures with the money we have?

        -   Then maybe we could compare what we have

        -   This is not an option for our final deliverable

    -   Jun’s research

        -   Liquid nitrogen is colder

            -   **We need a way to test for micro diffusion**

            -   There are still safety concerns with LN

    -   **We should reach out to companies that are already making tanks (LOX and nitrogen and also composite tanks.**

#**2017-01-26 Meeting with jun**
----------------------------------------------
-   Jun’s said some things

    -   We are ahead of most groups

    -   Has contacts we might be able to use for materials

        -   They have already helped PSAS once let's convince them to do it again.

        -   If you can’t supply materials can we talk to someone who was apart of the project with NASA

-   Presentation

    -   Jun’s comments

        -   How do we measure the pressure

            -   Russell has a plan using his own equipment

        -   Test one at a time and improve from that until the fabrication is perfected

            -   Alex “we can practice layup procedure”

        -   So prototype?

        -   Safety committee we need to notify someone

            -   She said that she can do it

            -   Can we bring samples somewhere to test?

        -   Jun likes the idea of letting professionals handle the LOX

        -   PAy attention to how much epoxy we use (maybe less is more)

        -   Add more to the reading list. (EXPAND the list)

        -   We can tour her lab any time

            -   (Next Tuesday)

        -   Record everything we do every time we layup( time, temp amount of epox, etc.)

            -   Change one thing at a time

            -   Have a methodical way of laying up

    <!-- -->

    -   Other things about presentation

        -   Epoxy is reactive

        -   Material selection has been done by erin (PTFE is ideal place to start)

            -   We might be able to get someone to machine for us

        -   Stuck with aluminum endcaps.

        -   Tank inside the module is not what erin wants. We make the module the tank.

        -   Opt program has given us dimensions

        -   We may share LOX resource with other PSAS team

        -   Thin aluminum liner(back up)

        -   Sketch tank design for a week Starting today!

        -   Add layup challenges to GANNT

<!-- -->

-   We talked about lab space

    -   Laser fire

    -   We need to be able to have access to the room

# **2017-01-12**
-------------------------------------------------------
>
> First meeting with Professor Jun Jiao.
>
> Main topic: Oregon Space Grant Consortium project proposal.
>
> -Quantify 2:1 funding from PSAS crowdfunding donations.
>
> -Emphasize that we are building off of a previous capstone and we have available resources and support.
>
> -Define clear team member roles
>
> -Provide team member info to show that we are an impressive group
>
> *1/11/2017 12:00 PM -- Google Hangout Meeting with Alex, Joseph, Russell, and Francesca*
>
> OSGC Proposal
>
> Discussed how to move forward with OSGC proposal:

-   We will be sticking with Jun Jiao as Advisor - Alex is emailing her, providing her with additional information so she can complete her letter before Friday. Probably no meeting due to snow - we are offering to meet via video chat tomorrow (Thursday, the 12th)

<!-- -->

-   Trying to model our proposal after fuel pump team’s - Alex is emailing them to see if they will allow us to look at their draft.

<!-- -->

-   Still waiting on email response from Andrew with clarifying questions about proposal (matching funds, etc).

<!-- -->

-   Russell is taking lead in researching materials and quotes to add to BOM - anyone with time to do so should try and contribute to BOM.

<!-- -->

-   Agreed to ‘meet’ up again at 9PM to discuss progress.

> Contacts: contact sheet added by Alex to drive- everyone should add their email and phone \#
>
> Reminder: Please add weekly availability to ‘availability’ doc, if you haven’t already.
>
# *2017-01-05**
>
> Oregon Space Grant Paper
>
> http://spacegrant.oregonstate.edu/student-research-projects
>
> -We need to start writing (due Jan. 13)
>
> -We need to come up budget
>
> -materials
>
> -AIAA registration
>
> -Faculty support options
>
> -Gerry
>
> -Weislogel
>
> -Raul Cal
>
> -Andrew (if necessary)
>
> -Wern
>
> We should write the faculty support letter.
>
> Material
>
> Find pricing for liner test materials:
>
> -PTFE
>
> -ETFE
>
> -PET
>
> -cryogel as an insulation layer/barrier
>
> -We can create test strips to test adhesion
>
> Design
>
> We have to figure out an endcap design
>
> -does it depend on the material we select
>
> Schedules
>
> -Enter winter term weekly schedule into google sheet
>
# **2016-11-15**
------------------------------------------------------------
> Rocket Capstone
>
> Target altitude of 100km
>
> Build a hobby rocket that will go to space
>
> Rocket equation V=Veln(mo/mf)
>
> Tank Prototype

-   Small scale test tank that demonstrates the design

-   Not responsible for plumbing

    -   There is help available

    -   We do need a fill valve and purge valve

    -   Machine endcaps with gasket

-   We have an idea

    -   On diameter (about 10”)

    -   Flow rate

    -   Volumes

-   Rocket equation V=Veln(mo/mf)

    -   The only change in mass is in the tank

-   Without the fuel pump we would need about 700 psi

    -   Shoot for at least 50 psi (more is better)

-   End caps do not need to be a composite

    -   Bolted on maybe, or something else any ideas?

-   Low tech

-   Composites are stronger and lighter

-   Hydrotesting will need to be done

-   We will also need to do a cryo fill

    -   We can observe the behavior of our lining and its interaction with the composites

-   Internal geometry

    -   Baffles

        -   Slosh

        -   Vortex

-   Make lots of prototypes and test them

-   Lots of materials properties data has been collected

-   We want a 2.5 factor of safety

    -   We will need to estimate the in flight loading

> BIG PROBLEMS

-   Epoxy is not LOX safe

    -   We will need some sort of liner

        -   No diffusion or leaks or bad things will happen

        -   Watch the interfaces for leaks

-   Account for thermal contraction and expansion

    -   Perhaps have a slightly larger liner than shell to allow for shink

> Document everything

-   Open source project

-   We want to leave something that future generations can benefit from

> This is not a project for someone who wants an easy one. Lots of time will need to be put into this
>
> Neil *NAB2@pdx.edu*
>
> Francesca *FF2@pdx.edu*
>
> Michael *mboyles@pdx.edu*
>
> Jonathan *balogh@pdx.edu*
>
> Musallam *alzamel@pdx.edu*õ



