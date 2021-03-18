# JDRenderEngine
Touchdesigner Render Engine by Jeremy dePrisco

Purpose:

A quick way to render time-synced audio/visual content in Touchdesigner.
If you like this tool, then buy me a coffee:

https://www.buymeacoffee.com/jeremydeprisco

Background:
	
I came to Touchdesigner from timeline-based video editing in programs like iMovie, Adobe Premiere and Davinci Resolve. For a few years I also built patches in Magic Music Visualizer. I was always frustrated by the UI of iMovie and similar programs. I never found their UX very good coming from the audio world. I also disliked how they managed project data, creating a whole new project with every iteration of a piece.

I liked the scene creation features of Magic Music Visualizer, though these too were quirky. As primarily an audio artist, I wanted a quick way to render content I was creating in Touchdesigner. Out of the box, Touchdesigner didn't have anything that checked the boxes for me, so I decided to build something.

As I dove deeper into Touchdesigner during a 6-month intensive study under lockdown, I realized that I could mostly replace iMove or similar tools. I probably wouldn't go back to Magic (though I still think it's a brilliant program, and I still liked the scene creation/logic features.

Of course, all of these tools could still be used in various combinations depending on the creative need, but I was looking for a “one stop shop”.

Thus my work began, in January 2021, on what I would call the “Render Engine”, specifically to solve certain problems I was encountering for content development. By March 2021 I had a working proof of concept, and opened up testing with a fellow audio artist (Breakfast). By working on visual content for him, I was able to refine the tool further.

If you like this tool, then buy me a coffee:
https://www.buymeacoffee.com/jeremydeprisco

Primary Use Case:

The primary use case for my Render Engine is for an audio artist who has a piece of music/audio that they want to sync to visuals. Those visuals may be prepared within Touchdesigner or elsewhere.

I know what you are thinking... there are already numerous VJ and Movie Scene transition tools out there. Yes, there are. I've tried most of them, and found many to be brilliant in their own right. Many were also over (or under) built for what I needed, and some simply didn't approach the problem from the same angle.

A Note about Audio Reactivity!
This tool is NOT for audio reactivity! There are dozens of audio reactivity approaches that one can use. I've explored most of the ones on YouTube. My goal is not to repeat that work here. Each piece of audio is different. As the artist will find, audio reactivity is *very* program dependent. A pulse/beat-driven audio reactive technique simply doesn't make sense for ambient music. If you want a more generative or random approach, then you might try different techniques. In my own work, I usually combine a beat-oriented approach with something that uses frequencies. But again, that material is covered elsewhere.

Features:

What the Render Engine IS about is easy reproducible rendering of a project. You should only come to the Render Engine after you have:

  1. Complete audio track
  2. Timings for your scene changes
  3. Visual content prepared elsewhere (other Touchdesigner project output or generative components)
  4. Intro and outro content (title slide, credits, etc)

The Render Engine is designed for quick generation of a completed piece after you have done all the creative work on the audio and visuals to your liking. So in that sense, it is more of a utility. But as a creative programmer and multimedia artist, I've always seen these sorts of utilities as creative tools that can be bent to the creator's will just as much as any other tool.

How to use:

Before you continue, please not that what I call a "Scene" here is any separate piece of content. If you want to use one Scene that has within it a bunch of evolving changes, you can do that. If you want to transition from one piece of content to another, you can do that as well. A Scene can hold your intro title slide, or your outro credits. It's up to you.

I've started with 12 scenes because for the material I was creating (songs 3-4 min long) that seemed to be more than enough. But the tool is scalable if you pay attention to the construction. I've tried to comment as much as possible within the scripts.

1. Select your audio file from the audiofileIN CHOP
2. Replace the Scene placeholders with your content
3. Set your scene time transitions in the table provided
4. Set any additional time in the addtime Math CHOP
5. Use Keyboard 2 key to reset all of the scripts.
6. Use Keyboard 1

I usually like to set the preview output to full screen on another monitor while I render.

The panic button (Key 2) is critical because your timing may not be correct at first. Rather than waiting for the entire thing to render, you can stop as soon as you notice an issue, tweak the results, and then start the render again. This is the main thing missing when you render in iMovie and similar programs.

Enhancements:

If you like this tool, then buy me a coffee:

https://www.buymeacoffee.com/jeremydeprisco

Depending on interest, I will endeavor to expand this tool with some other ideas I've had while making the initial release. If you'd like to collaborate on this project, then feel free to get in touch as well.

Version Details:
Current released version 1.0
This tool was built on the non-commercial version of Touchdesigner
Latest version compatible: 
2021.11180 on Mac on High Sierra

Special thanks to Dr. Matthew Ragan for his many tutorials. Dr. Ragan is one of (if not *the*) best Touchdesigner *teacher* hands-down.

I also used the Zap Studio frame calculator during initial testing, and you may find it helpful as well:
https://www.zapstudio.net/framecalc/
