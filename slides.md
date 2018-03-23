<!--
$theme: default
footer: @catrope | @SFOpenVoting
-->

## [#SFOpenVoting]()

## San Francisco's free software voting system

#### LibrePlanet 2018
##### Roan Kattouw

---
<!-- page_number: true -->

# Why a free software voting system?
* What is a voting system?
* Why is free software (especially) important here?
* What software exists already?
* What are we doing in San Francisco?

---
# Why use software for elections?

---
![](images/big-ballots-are-back.png)


---
# November 2016 election
* 3 federal offices (President+VP, Senate, House)
* 3 state offices (Assembly, Senate, Judge)
* 4 city/regional offices
* 17 statewide propositions (51 through 67)
* 25 city/regional propositions (A through X and RR)
* 4-page double-sided ballot, 5 pages in some districts
* 414k votes -> ~1.8M ballot cards

---
# Ranked choice voting
![](images/ranked-choice.png)
* Board of Supervisors (30k-40k voters per district)
* Mayor (~200k voters)
* Requires algorithm to compute result

---
# Reasons to use software
* Managing large amounts of data
    * 50+ contests w/ ~400k votes each
    * Ranked-choice elimination rounds
* Inputting all that data
* Reducing voter error
    * Warn against / prevent invalid votes
* Accessibility features

---
# Types of voting systems
* Hand-counted paper ballots
* Paper ballots with optical scan
* Direct recording (levers)
* Direct recording electronic (DRE)
    * With or without voter-verified paper audit trail (VVPAT)

---
# DREs without paper trail are bad
* Even if the software is free and open! (Which it isn't)
* No way to audit the results
* Still used in NJ, DE, SC, GA, LA
    * VA decertified theirs in 2017
    * GA-6 and NJ-Gov elections used these
    * Coalition for Good Governance sued Georgia over DREs (Curling v. Kemp)
* Banned in many countries, unconstitutional in Germany

---
# Using software safely
* Use paper ballots
* Audit everything
    * CA: 1% audit
    * Emerging: Risk-Limiting Audit (RLA)
* Publish data
    * SF: detailed ranked-choice data
    * Future: images of every ballot scanned

---
# What we use in San Francisco
* Proprietary system by Dominion (now Sequoia)
* Hand-marked paper ballots optically scanned at the precinct
* DREs with paper trail for accessible voting
* Vote-by-mail ballots scanned at City Hall

---
<img src="images/scanner.png" width=800>

---
# Voting system hardware
* Accessible voting device
* Precinct ballot scanner
* Central ballot scanner for vote-by-mail


---
# Voting system software
* Ballot layout
* Ballot scanning and interpretation
* Ballot adjudication
* Tabulation
    * Non-trivial for ranked-choice elections
* Results reporting
* Audit assistance

---
# Problems with proprietary systems
* Expensive (SF: $10M up front + $1.1M/year)
* Source code kept secret from public and city govt
* Making changes is hard / impossible
* Small market: 3 major vendors
* Vendor lock-in
* Security issues

---
# Free software is important here
* Election software is critical infrastructure
* Trust in election integrity is important
* Antiquated voting tech is a problem
    * Often too expensive to replace

---
# Practical advantages of free software
* Cheaper over time and across jurisdictions
* Innovation and adaptation easier and cheaper
* Investment for the common good
    * Developing jurisdiction spends more, others save
    * Need state/federal funding


---
# Other free software efforts

---
# Prime III / One4All
* Used in New Hampshire since 2016
* Prime III is GPLv3; One4All is NH's augmented version
* Accessible voting using COTS hardware
* Prints ballots; does not count votes
* QR code scanner to print pre-filled ballot from phone

---
![](images/one4all.jpg)

---
# ColoradoRLA
* Software facilitating risk-limiting audits
* Built in 2017 by FreeAndFair for Colorado under AGPLv3
* Statistical method to verify optical scan accuracy

---
# Risk limiting audits
* Software interpretation of ballot linked to ballot ID
* Small # of ballot IDs randomly selected
* Physical ballots located and compared to interpretation
* Repeat until probability of winner being wrong is low enough

---
# Other projects
* Travis County, TX: STAR-Vote
    * Design for a full voting system
    * "with a view toward ultimately" releasing as free software
    * Abandoned in 2017
* Los Angeles County, CA: VSAP
    * Full "voter-centered" redesign
    * Being developed, parts submitted for certification
    * Conflicting statements about free licensing
    * "open source stack/platform", "publicly owned code"

---
# San Francisco's project

---
# SF project goals
* Free software from the start (GPLv3)
* Commercial, off-the-shelf (COTS) hardware
* Openly licensed documentation (CC-BY-SA)
* Cheap and easy to reuse
* Set a model for state, country

---
# SF project history

* 2005 - Activists first introduce idea
* 2008 - BoS creates Voting Systems Task Force (VSTF)
* 2011 - VSTF recommends open source
* 2014 - Unanimous Board of Supervisors Resolution
* 2015 - Unanimous Elections Commission Resolution
* 2016 - Mayor & BoS budget $300K for planning phase
* 2017 - Commission forms Technical Advisory Committee
* 2017 - Planning RFP issued; consulting firm Slalom selected

---
# (Some) Supporters

![](images/supporters.png)

---
# Press coverage
<img src="images/sf-examiner.png" height="600">

---
# Current status

* OSVTAC meeting monthly, developing recommendations
* Procuring interim system (likely proprietary)
* Budget season is in full swing
* OSVTAC recommended funding for:
    * Hiring a project lead
    * Developing the first iteration

---
# Proposed first iteration
* Focus on vote-by-mail ballots (63% in 2016)
    * Scanner hardware+software
    * Software for layout encoding, tabulation, results reporting
    * (+batch management, auditing)
* ~6 devices instead of ~600
* Controlled conditions, highly trained operators
* Easier to phase in than precinct scanners, accessible devices

---
# Recent events
* Slalom report published
* Commission voted to request $4M from the city
* CA Clean Money Campaign pushing for state matching funds
    * 2:1 match, up to $8M

---
# How you can help

* In SF: ask Mayor & BoS to support funding
* In CA: ask Assembly & Senate to support matching funds
* Provide tech feedback to OSVTAC: https://osvtac.github.io
    * Recommendations on Github, open to PRs
* Spread the word
* Build interest in your community / pass a resolution

---
## Roan Kattouw

* roan.kattouw@sfgov.org (committee)
* roan.kattouw@gmail.com (personal)
* [@catrope]()


## SF Open Source Voting Technical Advisory Committee

* https://osvtac.github.io


<br/>
<br/>
CC-BY-SA 4.0<br/>
Includes material by Chris Jerdonek