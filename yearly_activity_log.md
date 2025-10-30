# 2007

This document is for explicit, personal notes about things you did in specific years. Use it to record detailed memories, events, and accomplishments for each year. 

---

## Instructions
- Write your notes explicitly for each year.
- Do not modify or edit existing entries unless you want to update your own log.
- This is a personal memory log for your reference only.

---

## Example Format

### 2025
- [Your notes for 2025]

### 2024
- [Your notes for 2024]

### 2023
- [Your notes for 2023]

---

## Your Log

### 2025

### 2024

### 2023

### 2022

### 2021

### 2020

### 2019

### 2018

### 2017

### 2016

### 2015

### 2014

### 2013

### 2012

### 2011

### 2010

### 2009

### 2008

### 2007

2007
I was working with something called Debussy, potentially to see RTL hierarchy?
I was wroking on validating padscan chains and create collateral for PythonSV and mixed signal validation. Worked with designers to pull changes and regenerate collaterals that fed tools. 

Subject: Monthly Report WW02’07
Summary:
IO/Parametric Queue:
WDC B0 Bin13 op7721 SBL -- WW50'06: Several lots failed class SBL due to BIN13. Package FA submitted some units for Silicon FA since they did not find evidence on a package defect. Units were check on the CMT and failures were reproduced. Units are failing the Ron-Rodt parametric measurements but are passing all the BIN13 functional tests. According with results units were failing for a few micro amps at hot temp. Compensation machine were checked and it was OK, not leakage was found on the failing pins. Data analysis over all the failing units showed that there is a strong package commonality which is affecting specific SLI panel locations and specific signals. Customer was notified and units were sent back to Package FA since no silicon malfunction was found. Cased was closed as customer support.
CTN B3 Bin11 op7751 ITR -- WW48'06: One unit failed the EQA test during PRQ. Unit was characterized at lab and it was observed that TDO_2 was 1 ohms over the max impedance limit. QRE wanted to discard a signature like the one observed in WDC a while ago due to a TP issue. However, it is a valid failure and it is not related to WDC BIN11 issue. This unit is out of range based on EMTS levels. Customer was notified and it was explained that FA to isolate 1 ohm is practically impossible. This unit was probably marginal at class and got a little bit of degradation and now if failing permanently. She was OK with the results, no more FA needed and case was closed as customer support.
NHM Activities:
NHM PadScan Chains Documentation: DDR padscan ordering for the latest model was already done and provided to design, however, extraction process is still complicated, manual and time consuming. The big problem right now is that when there is a new RTL model release, the ordering immediately gets obsolete since they modify adding or removing padscan cells, so it is required to redo the process again. Jonathan has been in contact with the NHM Mixed Signal Validation Team to generate to automate the process using a regression test that will check the padscan connectivity automatically. They already provide the requirements and Jonathan will work on creating the source files.
NHM IO/Parametric Tools definition: Jonathan and LuisG are working on the definition of the CSI SW tools (algorithms). First draft of RX DC tools will be defined by WW3.1 and TX DC tools on WW3.5. 

---

### 2006

### 2005

### 2004

### 2003

### 2002

### 2001

### 2000

### 1999

### 1998

# 2008

Doing system to tester I/O validation. Helping PDEs to port DFX based tests from system to TEster. Rterms, Icomps. 

wroking on Site Certifiation to HVM Gainstown. 

Involved on Early Life Test for Gainstown, provided characterization pre and post stress for critical circuits like PLL's. 

Worked on HAST stress validation
HAST stress refers to Highly Accelerated Stress Testing (or Highly Accelerated Temperature and Humidity Stress Testing).
HAST conditions typically include:
High temperature (e.g., 130°C, 140°C+)
High humidity (85% relative humidity or higher)
Elevated voltage/bias conditions
Extended duration (24-1000+ hours)
Purpose of HAST:
Accelerated aging to simulate years of field use in days/weeks
Moisture penetration testing of packaging and die
Corrosion resistance validation
Wire bond integrity under harsh conditions
Package reliability assessment
Electromigration and other failure mechanism acceleration
Common HAST variants:
HAST (temperature + humidity)
UHAST (Unbiased HAST - no electrical stress)
BHAST (Biased HAST - with electrical stress applied)
In Intel's 2007 weekly reports for products like Tylersburg, HAST results would be crucial for:
Package qualification
Reliability sign-off
Customer requirements (automotive, industrial applications)
Failure analysis and improvement
HAST is particularly important for complex chipsets like Tylersburg that need to operate reliably in various environmental conditions.

# 2009

SCAD: Spec Compliance and Debug board for JAsper Forest. 

Getting ready for jasper forest

Developing LatchUp test for Jasper FOrest IO/VCCLatchup

-----------------------------------------
WW16 monthly.

NHM Factory support:

FAB Via9 rework experiment: FAB performed an experiment to rework Via9 to a shorter height, which would allow recovering some material. Yield department requested Product FA on BIN13/11 failures in order to verify if defects were related to the rework experiment. Several failing units were analyzed but FA concluded none of them were related to a Via9 possible defect. Most of them were related to IO Back end logic which does not have interaction with any signal at Via9. Results were provided to Yield Dept and they will use it as base for WP approval for new POR.

SBTS status:

Collaterals
- 3 more ITP’s were purchased and expected to arrive in a few weeks. We will have a total 8 ITP’s in stock that will be shared between NHM, JSP, Gulftown and Clakdale. 
- New lab space was provided for stand alone systems for cache and SBTS. We will start with NHM setup for SBFT/Cache but it seems we will be short in space again when we need to configure the same setup for JSP and Clarkdale.

Gainstown/Bloomfield

PowerCycle issue
SBTS configuration is presenting a bug on power cycling. For some reason when the Power Cycle is asserted, ITP dies. Not a work stopper but it is really annoying and affects TPT since every time the user needs to change the unit, has to kill all the ITP software and then re launch everything again. It is happening on any SBTS board no matter if it uses Agilent power supply configuration or power module configuration. It seems to be a problem related to the on-board reset sequence. Issue was escalated to PNG TD and they were able to reproduce it locally which will help to debug. They are working on the issue now.

SBFT/Cache Setup
New lab space was provided to assemble SBFT and cache dedicated systems. During WW16/17 we will be moving all the workstations and systems.

Agilent Power supplies setup
We are orking on assembling and configuring Costa Rica Agilent power supplies since PNG needs the loaned PS back. It is required to configure the power on sequences and verify hardware is working. It is expected to be shipping PNG Power Supplies by mid next week.

Jasper

SBTS board development
Electrical requirements are almost done. A few pins are pending to get some information regarding its functionality but we are working with JSP design team to understand the required connection on the SBTS. It was concluded that we need to change the socket footprint since NHM debug socket is not compatible with JSP DW hardware. It is required to design SBTS board with NHM CMT Debug socket which is compatible for JSP and its DW. Board delivery is going OK in target to WW30.

JSP SBTS early Power On using NHM Board (experiment)
Most of the reworks were done on the NHM board to re route signals on the board that are different for JSP. Just a few signals are different(VTTPWRGOOD, RESET & GTLREF). However, we hit a wall regarding TAP pins. IT is required to short circuit TDI_M and TDO_M, but problem is that they are connected to a VCC plane on NHM board. We are working on possibilities to isolate those pins from the plain but it seems complicated.

JSP Socket/DW Hardware
All hardware was identified and ready for shopping basket

Clarkdale

CKD Socket/DW Hardware
All hardware was identified and ready for shopping basket

SBTS enabling
Since PNG is first site on CKD, they will fund the build of the SBTS board and provide Costa Rica with some boards. Costa Rica as a win2win deal will fund the build of Power Delivery boards and provide PNG with some boards (cost is ~ 7K).
---------------------

Raster and LYA for Memory

# 2010

2010:

Relo to Penang 21 jun: SBTS development for JKTN server.

SBTS prep for Jaketown

Sandy Bribge is coming

Worked with SmartLab vendor to define TEster API requirements for FIFA automations and test program writing for Analog I/O testing. 

Coming back to CR in December

# 2011

2011:

Super user on In-Target-Probe

Doing Jaketown

Getting ready for Hashwell Server HSWX

starting MTL TP architecture with IDUT

working with Design to ensure IDUT DFX on presilicon

PSLE 2021 Concurrent_parallel_dielet_testing

defining onlyME architecture for MTL

# 2012

2012:

PinPinder MeltDown

Sept relo to PNG

Cache L2P Logical to physical mapping

HSX PO readiness

# 2013

2013:

HSX power on

First FIVR product

Working with Elsoft to validate CombiTest DLL for SBST.

# 2014

2014:

Date    :           January 13, 2014
To        :          Jaime Castillo
From   :          Jonathan Urtecho
Subj     :          Monthly Report
________________________________________

HSX FAB C  board were shipped to all customers. PG,SC,ATD,F28 and F32 received the latest FAB C boards and Rev3 Interposers.

HSX VIXVOX presenting problems. We put VIX aside for a little bit and decided to give VOX a try to see if he had better luck but unfortunately it did not work. All CMT precondition was converted but DUT is remaining in tri-state no matter what. The only difference we have right now is the cold reset. The current SBTS reset is generated from Burn In and it seems to be different from the IO reset used on CMT. LuisE is currently working on the regeneration of this IO CMT reset for SBTS. We hope fuses and configuration will make the things work.

HSX EP Shops/Leakage enabled: JoseCh enabled the shops/leakage batch testing on the SBTS IO GUI. We defined an strategy based on limits distribution. Basically we took several units at hot and cold and did a statistics analysis of the possible limits. We are not working with sigma calculations because we don’t have a good sample to do that, instead we defined a range over and below the max/min distribution. Still marginal failures have to be process carefully but we expect to get most of the fails. In any case we can adjust the limits over the time.

Foxcon HSX A0 FACR: Six units were returned by FoxConn requesting for FA to understand if damaged was induced by them or a rel issue on those parts. FoxConn was in line down waiting for FA. Analysis revealed an EOS on five units and one passed CMT FIVR revalidation. EOS was located on the same area (DDR01) but not in the same exact pins so we presume there was a hardware commonality inducing the damage (like a bad DDR DIMM or motherboard Voltage Regulator malfunction). Additionally we observed some signatures of bad manipulation like FM, scratches and damage components but none of them related to EOS. Results were promptly sent to QSC.

PinFinder Python TIU exaction scripts needs to be enhanced. Even though designed script has been working good it requires a lot of maintenance because all the non-standard TIU components and labels. This creates some constraints because only developer can understand/make the changes which is not functional in the long run. The idea is to re-code the script with more intelligence to detect components and minimize the user inputs. Hopefully it will run transparently for CMT and HDMT

------------------------------------------------------------------------

Date    :           February 10, 2014
To        :          Jaime Castillo
From   :          Jonathan Urtecho
Subj     :          Monthly Report
________________________________________

HSX EN interposer is not functional, new board design is required. PinMap used for HSX EN interposer was incomplete and some critical pins were not connected which is a fact that totally blocks reset (FIVR’s can’t wake up). Post Morten analysis revealed a few points to be corrected: 1- PinMap from Design only had the OEM socket required pins and not all the FIVR debug/configuration used on HVM. 2 – Misunderstanding on some connection concepts between design and layout. 3 – Electrical verification failed due to bugs on scripts. New Interposers fixes are being defined and will immediately be sent to PG for corrections. INT board Re-spin will take from 5 to 6 weeks.  Actual interposers can be used as Bench Board for about 97% of the IO’s but just for Power Off characterization.

HSX VOX EP C0 almost complete: All the IO’s being tested at production are working on SBTS. All impedances are targeting what is expected by spec but there is a slight variability on SBTS. CMT is using around +/-15%  impedance target, but most likely we will have to open it a little bit on SBTS.  Still in process of collection data from more units to check variability and define limits. We have received all the units allocation for EP (M and S steps) so we will immediately validate VOX on those after LuisE’s reset generation. SBTS IO GUI still not available for VOX, but validation scripts can be used for FI meanwhile. 

HSX VIX EP C0 still in progress: No advance on this task, waiting for VOX completion.

--------------------------------------------------------------------------------

Worked on Rapid File

ittp to ITP

------------------------------------------

Transfer technology to Penang

Transfered to Oregon

# 2016

2016:

Enabled Looping on HDMT for Foundry

LADA enablement

Worked with EMIB on FPGA prodcts

Move to STTD

Started working on LnP on Verigy (SmartTest) to convert to HDMT. Using SV validation board to validate ATE content and pattern conversion.

# 2017

2017:

Started to work on DX2

vcd/evcd for non-scan and STIL for Scan

mbist_core_step00_pmovi_chkb_sof1: pmovi checker board stop on fail

Started to work on Champlain Test Chip

ARM Ananke High Performance (HP) and Low Power (LP) CPU

PMBIST using cadence design system (CDNS) for ARR

Worked with CDNS team to define content for test chip ARR, SCN , FUN.

FUN was ran using Dhrystone 

Scan/ATPG Validation Plan and Status
Here are key takeaways from Glenn’s presentation.
1. Scan test modes:
   a. Compression (preferred for pass/fail test) with OPCG disabled for stuck-at ATPG.
   b. Compression with OPCG enabled for at-speed ATPG.
   c. Fullscan (compression not enabled, preferred for debug) with OPCG disabled for stuck-at ATPG.
   d. Fullscan with OPCG enabled for at-speed ATPG.
2. Ananke quad-core: When compression mode tests fail for an Ananke cluster, we cannot tell which Ananke core(s) fail. For debug or FA/FI, we will have to do it with Fullscan mode tests.
3. Current plan is to use PLL output for at-speed scan test debug, question was raised over whether we can use PLL internal bypass with Fullscan debug tests. Glenn will follow up on this.
4. All ATPG partitions of the entire chip will be run in parallel, with ATE having the flexibility to directly drive ScanIn and strobe ScanOut for each partition.
5. Validation is underway.  Current plan is to run zero-delay GLS at fullchip, with selected SDF-annotated GLS runs later.  Intel (Arani) will provide some recommendations over validation plan.  
6. CDNS team will enable assertions to check whether Ananke Power Controls are programmed OFF during Scan & MBIST test mode sequences.
7. Path Delay ATPG: We anticipate the need of Path Delay ATPG patterns to debug potential speed path issues, had extensive discussions during “Yellow Pad” drafting phase, and captured in SOW.  Though, Glenn does not have it in his plan. He will sync up with Ricky on this request.
8. Scan Diagnosis: There is no need to generate special diagnosis ATPG patterns.  ATE test log files can be fed to CDNS Modus for logical diagnosis. To enable scan diagnosis by Intel team, tbdata for the design will be needed for logical diagnosis, and Oasis database will be needed for physical diagnosis.  

MBIST Validation Plan and Status
Here are key takeaways from Scott’s presentation.
1. Validation (RTL and selected zero-delay GLS) are done for
   a. All memories with Scan and MarchC- algorithms.
   b. Setup sequences for all 5 PLL’s (two for each Ananke cluster, and one for SoC).
   c. Error injection (forced failure).
2. Validation in progress
   a. Power On sequence for test modes
   b. SDF-annotated GLS
   c. Redundancy analysis.
3. Known issue with the combo of CDNS PMBIST and Ananke/Corinth Shared Bus prevents proper memory diagnosis when a RAM macro is split across two different “Targets”. Checkerboard data background does work properly with the upper half “Target”. Pass/fail test should work. Diagnosis (bitmapping) with other data background should also work.
4. PMBIST pattern generation and Memory Diagnosis (Bitmapping) need Modus 17.1 license, and tbdata (with description of Memory and MBIST info).
5. Memory repair analysis: Need to feed ATE test log file into Modus tool. Though, we need to get more specifics of tool and flow from CDNS AE’s.
6. Pattern generation: Scott has enabled 22 algorithms and all data background types that Intel requested for. He can generate MBIST test patterns with a single memory instance per pattern or with multiple memory instances in parallel. Intel prefer to have a single memory and a single algorithm per pattern. Concern is that test vector data volume will be huge with that preference (as each pattern will have a lengthy init sequence). 

Started to work on S22E (Memory Chip)

Chain EDToff
Chain EDTon  (onehot, individual patterns per chain and EDT logic)
Stuck at
TDF EDTon PLL
TDF EDToff PLLbyp
PDF EDToff PLL

# 2018

2018

Started working on HIPI (HDMT Integrated PLanar INterface)

# 2019

Stated to work on dekel Phy for TypC and NTC. Started to work with FirmWare validation.

Then got involved on TGL IDUT. POC

Readiness for IDUT, TPIE, Evergreen, TP POCs

# 2020

2020

Started the implementation of IDUT on TGL B-Step. TP was flipped to IDUT on Q1 and then parallelism was slowedly enabled towards PRQ

# 2021

2021:

Working on TGL IDUT validation.

Involved in POC for TGL.

Started working on Willow Cove.

Engaged in firmware development and validation for TGL.

Participated in architecture discussions for next-gen products.

Began exploring low-power validation techniques.

Collaborated with cross-functional teams for integrated validation plans.

Initiated work on security features validation for TGL.

Contributed to test planning and strategy for upcoming CPU architectures.

Focused on improving validation coverage and efficiency.

starting MTL TP architecture with IDUT

working with Design to ensure IDUT DFX on presilicon

PSLE 2021 Concurrent_parallel_dielet_testing

defining onlyME architecture for MTL

# 2022

2022:

Continued work on Willow Cove validation.

Led efforts in low-power and security features validation.

Collaborated with architecture and design teams for next-gen CPU validation.

Enhanced test methodologies and automation for efficiency.

Participated in silicon bring-up and debug for TGL.

Contributed to validation of new instruction set architectures.

Worked on improving power delivery and management validation.

Engaged in cross-platform validation efforts.

Initiated exploratory validation for post-TGL architectures.

Focused on closure of validation gaps and improvement of overall product quality.

# 2023

2023:

Focusing on next-gen CPU validation methodologies.

Exploring advanced power management features.

Enhancing security validation processes.

Collaborating on cross-architecture validation strategies.

Leading efforts in validation automation and efficiency.

Participating in architecture definition for future products.

Engaging in silicon bring-up and validation for new platforms.

Contributing to the development of next-gen validation tools and frameworks.

Working on improving validation coverage for complex CPU features.

Initiating exploratory projects for innovative validation techniques.

# 2024

2024:

Diving deep into next-gen CPU microarchitecture validation.

Pushing boundaries in power efficiency and performance validation.

Spearheading security validation for upcoming high-risk features.

Collaborating with software teams for early validation of firmware and drivers.

Leading cross-functional teams in holistic validation approaches.

Participating in industry forums for advanced validation techniques.

Exploring machine learning applications in validation.

Contributing to the development of next-gen debug and analysis tools.

Working on closure of complex validation scenarios.

Initiating projects for continuous improvement in validation processes.

# 2025

2025:

Anticipating tape-out and silicon validation for new CPU.

Focusing on validation of advanced packaging technologies.

Exploring 3D stacking and chiplet architectures.

Leading efforts in power integrity and thermal validation.

Collaborating on system-level validation for next-gen CPUs.

Participating in pre-silicon validation and emulation.

Contributing to the development of next-gen validation methodologies.

Working on improving validation efficiency and effectiveness.

Initiating exploratory projects for future CPU architectures.

Focusing on closure of all validation aspects for upcoming products.
