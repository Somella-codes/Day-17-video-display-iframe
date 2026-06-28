# Day-17-video-display-iframe had me stressed 😅

**The Challenge**
FCC: Build a page that displays 3 YouTube videos using only HTML `iframe`. 
No CSS. No JS. Just structure.

**What Went Wrong**
I copied 3 random YouTube links first... and got "Video unavailable" on all of them 🙃 
I thought I broke my code. 

The code passed FCC’s tests, but the preview wouldn’t load there. It only ran properly when I opened `index.html` in Spck Editor on my phone.

**What I Learned**
1.  **The Embed Rule**: YouTube needs `/embed/VIDEO_ID` in the `src`. `/watch?v=` will never work inside an iframe.
2.  **Embedding Settings**: Creators can block their videos from being embedded. That’s why freeCodeCamp’s own videos work best.
3.  **Environment Matters**: FCC’s preview can block iframes for security. A local browser or Spck Editor shows the real result.
4.  **Accessibility Matters**: Every `iframe` needs a `title`. Screen readers depend on it. Also set `width` + `height` to avoid layout shift.
5.  **Semantic HTML**: The whole thing has to be `main` > `section` > `h2` > `p` > `iframe`. That order was literally a test case.

**How It Looks in Spck**
![Video Display Screenshot](Screenshot_20260626_212222_Spck%20Editor.jpg)

**Tech Stack**
`HTML5` | `iframe` | `Semantic Tags` | Tested in `Spck Editor`

**Wanna see the code?** 
👉 [index.html](./index.html)

