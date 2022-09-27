# Kontakt Legato
Customizable True Legato Script

HOW TO USE:
store your legato transitions in separate groups and name them accordingly:
1) name the groups of transition samples with the amount of transition by semi-tone
	etc: group name of one octave up transitions :"+12"
	etc: group name of perfect fifth down transitions: "-7"
2) name the group with start samples as "start"
3) name the group with release samples as "release"
4) name the group with repetition samples as "0" (zero)

!!!If you have more than one layers, you can name the layers belonging to the same transition group with the same name and that will work fine.
  If you'd like to name them differently, the script must be modified.
  
!!!If a transition is more than one octave, since usually there are no samples for more than one octave legato transitions, this script (instead of triggering absurd legato transitions) triggers a release sample for the departed note and a start sample for the arrived note,  which is much similar to what would happen on a string instrument.

DEFINITIONS:

REPETITION TIME: maximum time to trigger repetition samples after releasing a key.
  If the same key is triggered "< REPETITION TIME " after releasing it, release sample will be triggered. Otherwise, start sample will be triggered.
  This should be set according to the player's & keyboard's capabilities.
  
LEGATO FADE TIME: overlap time of end of first sample and beginning of the legato sample.
  When a key is pressed while another key is still held, the first note is faded out while the legato sample of the second note is faded in.
  This should be set according to the length of the departed pitch in the legato samples of the arrived pitch.
  
RELEASE FADE TIME: overlap time of end of first sample and beginning of the release sample
  This should be set to as close to zero as possible but not so much that a click can be heard.

REPETITON FADE TIME: overlap time of end of first sample and beginning of the repetition sample
  This should normally be set to zero.
