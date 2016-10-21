# PLOVER

![plover_icon](https://github.com/openeventdata/PLOVER/blob/master/plover_icon175.png "PLOVER logo")

PLOVER—Political Language Ontology for Verifiable Event Records—is a
next generation political event coding specification under development by the
Open Event Data Alliance (http://openeventdata.org/) which is intended
to replace the earlier
[CAMEO] (http://eventdata.parusanalytics.com/data.dir/cameo.html)
system. The major features of PLOVER include:

-  A set of standardized names ("fields") for JSON
   (http://www.json.org/) records are specified for both the core event
   data fields and for extended information such as geolocation and
   extracted texts. Most of these fields are optional but standardized
   field names will allow for the development of common utilities, which
   cannot be done with the current proliferation of incompatible CSV and
   tab-delimited formats.
-  Only the 2-digit event 'cue categories' have been retained from
   CAMEO: our hope is that these are sufficiently broad and distinct
   that it will be possible to achieve a reasonably high level of human
   inter-coder agreement— hence "verifiable"—on the coding categories,
   and that can be consistently implemented, across all categories, in
   automated systems. These are defined in much greater detail than they
   were in WEIS and CAMEO. Details 
-  The CAMEO 01 and 02 categories dealing with comments have been
   eliminated.
-  A new category has been added for criminal behavior.
-  The WEIS/CAMEO YIELD category has been split into verbal (CONCEDE) and material (RETREAT) components.
-  A "context" field is available, along with standard values, to handle
   contexts such as disease, natural disaster, elections, parliamentary
   processes and cyber-security.
-  The complexity of substate actor codes has been limited, and the
   allowable substate modifiers have been substantially simplified.
-  Standard optional fields have been defined for some categories -- in particular a "mode" field which can provide
   much of the 3- and 4-digit detail found in CAMEO -- and
   the "target" is optional in some categories.
-  In the near future, we are hoping to make available a large corpus of
   "gold standard records" for validation purposes: these will include
   Spanish and Arabic cases as well as English. The release
   documentation includes the English-language gold standard records
   from the CAMEO manual.
-  The PLOVER documentation is licensed under a Creative Commons
   Attribution-ShareAlike 4.0 International License.

PLOVER is currently under development but we anticipate the release of
documentation before the end of 2016. Watch this space for further
developments.

PLOVER in a nutshell
====================

CAMEO code | CAMEO text | PLOVER category |
--- | --- | --- |
01 | MAKE PUBLIC STATEMENT | dropped |
02 | APPEAL | dropped |
03 | EXPRESS INTENT TO COOPERATE | AGREE |
04 | CONSULT | CONSULT |
05 | ENGAGE IN DIPLOMATIC COOPERATION | SUPPORT |
06 | ENGAGE IN MATERIAL COOPERATION | COOPERATE |
07 | PROVIDE AID | AID |
08 | YIELD (081 to 083) | CONCEDE |
08 | YIELD (084 to 087) | RETREAT |
09 | INVESTIGATE | INVESTIGATE |
10 | DEMAND | DEMAND |
11 | DISAPPROVE | DISAPPROVE |
12 | REJECT | REJECT |
13 | THREATEN | THREATEN |
14 | PROTEST | PROTEST |
15| EXHIBIT FORCE POSTURE | MOBILIZE |
16 | REDUCE RELATIONS | SANCTION |
17 | COERCE | COERCE |
18 | ASSAULT | ASSAULT |
19 | FIGHT | FIGHT |
20 | USE UNCONVENTIONAL MASS VIOLENCE | FIGHT |
-- | no CAMEO equivalent | CRIME |

PLOVER quad categories
----------------------

Quad category | PLOVER categories |
--- | --- |
Verbal cooperation | AGREE, CONSULT, SUPPORT, CONCEDE |
Material cooperation | COOPERATE, AID, RETREAT, INVESTIGATE |
Verbal conflict | DEMAND, DISAPPROVE, REJECT, THREATEN, SANCTION |
Material conflict | PROTEST, CRIME, MOBILIZE, COERCE, ASSAULT, FIGHT |


Why "PLOVER"?
=============

[Plovers](http://www.rspb.org.uk/discoverandenjoynature/discoverandlearn/birdguide/name/r/ringedplover/)
(Charadriidae) are a globally-distributed family of short-billed
gregarious wading birds who spend their lives frantically poking through
endless stretches of sand and muck trying to find something of interest.
It is difficult to imagine a better analogy to the process of coding
event data.

Description of files in repository
==================================

* PLOVER_GSR_CAMEO.txt

   This is a JSON file of the example sentences from the CAMEO 1.1b3 manual classified by PLOVER categories. The CAMEO LaTeX markup indicating source, target and event texts has been converted to a simple in-line markup. This initial post does not have markup for sectors, modes or contexts: we expect to add this at a later date.



Copyright © 2016, Open Event Data Alliance

Last update: 21 October 2016

