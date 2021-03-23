# JDRenderEngine
Touchdesigner Render Engine by Jeremy dePrisco

## Purpose:

A quick way to render time-synced audio/visual content in Touchdesigner.
If you like this tool, then buy me a coffee:

https://www.buymeacoffee.com/jeremydeprisco

## Background:
	
I came to Touchdesigner from timeline-based video editing in programs like iMovie, Adobe Premiere and Davinci Resolve. For a few years I also built patches in Magic Music Visualizer. I was always frustrated by the UI of iMovie and similar programs. I never found their UX very good coming from the audio world. I also disliked how they managed project data, creating a whole new project with every iteration of a piece.

I liked the scene creation features of Magic Music Visualizer, though these too were quirky. As primarily an audio artist, I wanted a quick way to render content I was creating in Touchdesigner. Out of the box, Touchdesigner didn't have anything that checked the boxes for me, so I decided to build something.

As I dove deeper into Touchdesigner during a 6-month intensive study under lockdown, I realized that I could mostly replace iMovie or similar tools. I probably wouldn't go back to Magic (though I still think it's a brilliant program, and I still liked the scene creation/logic features.

Of course, all of these tools could still be used in various combinations depending on the creative need, but I was looking for a “one stop shop”.

Thus my work began, in January 2021, on what I would call the “Render Engine”, specifically to solve certain problems I was encountering for content development. By March 2021 I had a working proof of concept, and opened up testing with a fellow audio artist (Breakfast). By working on visual content for him, I was able to refine the tool further.

If you like this tool, then buy me a coffee:
https://www.buymeacoffee.com/jeremydeprisco

## Primary Use Case:

The primary use case for the JDRenderEngine is for an audio artist who has a piece of music/audio that they want to sync to visuals. Those visuals may be prepared within Touchdesigner or elsewhere. The JDRender Engine is mostly geared toward the generation of a final file from *generative* content that you've already programmed elsewhere, but want to present in some scene-based format.

I know what you are thinking... there are already numerous VJ and Movie Scene transition tools out there. Yes, there are. I've tried most of them, and found many to be brilliant in their own right. Many were also over (or under) built for what I needed, and some simply didn't approach the problem from the same angle. almost every tool that I came across assumed that the user wanted to work with pre-rendered content. And while you can still do that here, that is not the focus.

A Note about Audio Reactivity!
This tool is NOT for audio reactivity! There are dozens of audio reactivity approaches that one can use. I've explored most of the ones on YouTube. My goal is not to repeat that work here. It's easy to tap off the audio coming in to run through whatever reactive tools you like to use (see the ForReact Null CHOP).

As the artist will find, audio reactivity is *very* program dependent because piece of audio is different.  A pulse/beat-driven audio reactive technique simply doesn't make sense for ambient music. If you want a more generative or random approach, then you might try different techniques. In my own work, I usually combine a beat-oriented approach with something that uses frequencies. But again, that material is covered elsewhere.

## Features:

What the JDRenderEngine IS about is easy reproducible rendering of a project. You should only come to the JDRenderEngine after you have:

  1. Complete audio track
  2. Timings for your scene changes
  3. Visual content prepared elsewhere (other Touchdesigner project output or generative components)
  4. Intro and outro content (title slide, credits, etc)

The JDRenderEngine is designed for quick generation of a completed piece after you have done all the creative work on the audio and visuals to your liking. So in that sense, it is more of a utility. But as a creative programmer and multimedia artist, I've always seen these sorts of utilities as creative tools that can be bent to the creator's will just as much as any other tool.

Scene and current time (in seconds) are provided via a heads-up display that can be used as a preview or rendered with the actual content. The default output for the Moviefileout TOP does not include this overlay, but it's easy to change.

Crucially, I provided a "panic button" so you can stop and re-render easily. Lots of under the hood scripting is taken care of so you can focus on the creative part!

## How to use:

Before you continue, please not that what I call a "Scene" here is any separate piece of content. If you want to use one Scene that has within it a bunch of evolving changes, you can do that. If you want to transition from one piece of content to another, you can do that as well. A Scene can hold your intro title slide, or your outro credits. It's up to you.

I've started with 12 scenes because for the material I was creating (songs 3-4 min long) that seemed to be more than enough. But the tool is scalable if you pay attention to the construction. I've tried to comment as much as possible within the scripts.

By default, I've set Scene 1 as a title slide, which runs for 300 frames (5 sec) with no music.
Music starts on Scene 2.
Scene 10 is the credits slide, which runs for 300 frames (5 sec) by default.
Scene 11 is a blackout slide, hardcoded for 1 sec.

All of these parameters can be changed, but there is no UI yet to do so. See enhancements below.

1. Select your audio file from the RENDERAUDIO CHOP - note that I've provided the option of switching to a test file for testing without rendering. But the render process relies on the file in the RENDERAUDIO CHOP
3. Replace the Scene placeholders with your content
4. Set your scene time transitions in the table provided
5. Set any additional time in the addtime Math CHOP. Default is 300 frames (5 sec) for intro, and 300 frames for outro, totalling 600 frames.
6. Locate the scenepreview node and set it to view (handy for previewing on a second monitor to watch your render).
7. Use Keyboard 2 key to reset all of the scripts.
8. Use Keyboard 1
9. Watch your render take place!

I usually like to set the preview output to full screen on another monitor while I render.

The panic button (Key 2) is critical because your timing may not be correct at first. Rather than waiting for the entire thing to render, you can stop as soon as you notice an issue, tweak the results, and then start the render again. This is the main thing missing when you render in iMovie and similar programs.

See the example render MOV. I had to doengrade it to 480p for Github, but otherwise this is a good start.

{Link to Youtube will go here}

## Enhancements:

If you would like to see enhancements to the JDRenderEngine, then buy me a coffee:

https://www.buymeacoffee.com/jeremydeprisco

Depending on interest, I will endeavor to expand this tool with some other ideas I've had while making the initial release.
If you'd like to collaborate on this project, then feel free to get in touch as well.

## Version Details:

Current released version 1.0
This tool was built on the non-commercial version of Touchdesigner
Latest version compatible: 
2021.11180 on Mac on High Sierra

Special thanks to Dr. Matthew Ragan for his many tutorials. Dr. Ragan is one of (if not *the*) best Touchdesigner *teacher* hands-down.
The OP Snippet for series segment timing was used, but a lot more work was done before I even discovered that example.

I also used the Zap Studio frame calculator during initial testing, and you may find it helpful as well:
https://www.zapstudio.net/framecalc/

## LICENSING:
Since we are artists/programmers and not lawyers, I trust you will give credit where credit is due and respect the licence:

GNU General Public License v3 (GPL-3)

This means that if at some point you would like to use this tool in a commercial endeavour or you do not want to disclose the source code you will get in touch first, so a fair arrangement can be made. Contact info below.

## Thanks for visiting!

You can learn more about my other projects here:

Music:
https://jeremydeprisco.bandcamp.com/

https://www.jeremydeprisco.net/

Other stuff:
https://www.jeremydeprisco.com/

Contact:
https://twitter.com/jeremydeprisco
https://www.jeremydeprisco.net/contact

LinkedIn:
https://www.linkedin.com/in/jjdeprisco/

Indeed:
https://my.indeed.com/p/jeremyd-180u8qq

Fiverr:
https://www.fiverr.com/shivasongster?up_rollout=true
