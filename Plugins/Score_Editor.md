# Score Editor
The score editor is a simple dialog that allows you to insert score into a page using **GNU Lilypond**.

In order to be able to use this plugin you must have GNU Lilypond installed and the following command must be available on your system: "``lilypond"``. You can control the look of the scores using the special template "``_Score.ly"``. 

**Dependencies:** This plugin requires GNU Lilypond to be installed. In specific the "lilypond" command should be available in the system path.

Syntax
------

Refer the References section for information on GNU Lilypond syntax.

Following are a few examples generated by the plugin:

### Example 1: Pachelbel's Canon
![](./Score_Editor/score.png)
	\relative c {
	        \clef bass
	        \key d \major
	        \time 4/4
	
	        d4 a b fis
	        g4 d g a
	}


### Example 2: With Chords, Staff and Lyrics
![](./Score_Editor/score001.png)
	<<
	    \chords {
	        c1:m7 f2:7 c2
	    }
	    \relative c'' {
	        g2 es8( c4) es8
	        f8 es d c~ c2
	    }
	    \addlyrics {
	        You are
	        the sky and my rain,
	    }
	>>


### Example 3: With multiple Staffs
![](./Score_Editor/score002.png)
	hornNotes =
	  \relative c {
	    \time 2/4
	    R2*3
	    r4 f8 a cis4 f e d
	  }
	
	bassoonNotes =
	  \relative c {
	    \clef bass
	    r4 d,8 f gis4 g b bes
	    a8 e f4 g d gis f
	  }
	
	
	<<
	  \new Staff \hornNotes
	  \new Staff \bassoonNotes
	>>


### Example 4: With Strumming rhythm and FretBoard
![](./Score_Editor/score003.png)
	<<
	  \new ChordNames {
	    \chordmode {
	      c1 | f | g | c
	    }
	  }
	  \new FretBoards {
	    \chordmode {
	      c1 | f | g | c
	    }
	  }
	  \new Voice \with {
	    \consists "Pitch_squash_engraver"
	  } {
	    \relative c'' {
	      \improvisationOn
	      c4 c8 c c4 c8 c
	      f4 f8 f f4 f8 f
	      g4 g8 g g4 g8 g
	      c4 c8 c c4 c8 c
	    }
	  }
	  \new Voice = "melody" {
	    \relative c'' {
	      c2 e4 e4
	      f2. r4
	      g2. a4
	      e4 c2.
	    }
	  }
	  \new Lyrics {
	    \lyricsto "melody" {
	      This is my song.
	      I like to sing.
	    }
	  }
	>>


Template
--------

The Score plugin's template has following three variables to customize your GNU Lilypond document, used for generating the score images:

* **include_header:** Common include header section to include GNU Lilypond predefined files or add common definitions.
* **include_footer:** Common include footer section to define standard footer section to be included in the GNU Lilypond document.
* **score:** The actual user input in Insert/Edit dialog box in used.


Feel free to tailor the template file for your needs.

GNU Lilypond Version
--------------------

Syntax of GNU Lilypond could change with new releases, and these changes need not be backward compatible. For this reason, the version of GNU Lilypond when the score was created is inserted into the score text by the plugin.

When a different version of GNU Lilypond is installed, the plugin would use ``convert-ly`` (packaged with GNU Lilypond) to convert the score file to be compatible with installed version before rendering the score.

References
----------


* Quick introduction to text input in GNU Lilypond (<http://lilypond.org/text-input.html>)
* Learning Manual for GNU Lilypond (<http://lilypond.org/doc/v2.14/Documentation/learning/index.html>)
* Notation reference for GNU Lilypond (<http://lilypond.org/doc/v2.14/Documentation/notation/index.html>)
* Snippets database for GNU Lilypond (<http://lilypond.org/doc/v2.14/Documentation/snippets/index.html>)
* Other manuals for GNU Lilypond (<http://lilypond.org/manuals.html>)

