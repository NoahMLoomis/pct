---
# try also 'default' to start simple
theme: default 
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
title: Pacific Crest Trail
# https://sli.dev/features/drawing
transition: slide-left
class: text-center
# enable Comark Syntax: https://comark.dev/syntax/markdown
comark: true
---


# Pacific Crest Trail

A better way to track it

<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
transition: fade-out
background: /images/map.png
---

# The Pacific Crest Trail: 4560km hike from Mexico to Canada

<div grid="~ cols-2 gap-8" m="t-4">
<div>



- Through California, Oregon, and Washington
- 10,000 annual attempts
- 25% success rate
- Takes about 5 months to do

</div>
<div>
<img src="./images/map2.png" alt="PCT Map" class="max-h-[55vh] w-auto mx-auto object-contain" />

</div>
</div>
<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/features/slide-scope-style
-->

<!-- I left in March, finished in August, took 139 days. This time last year, I was climbing Mt Whitney-->
---
layout: image-right
image: /images/sierras.jpg
backgroundSize: 20em 
---

# This time last year

<style scoped>
img { object-fit: contain !important; }
</style>

---
---

# noah-vs-the-sun.com

<div grid="~ cols-3 gap-4" m="t-4">
    <v-click>
      <img border="rounded" src="./images/blog1.png" alt="" class="w-full h-full object-cover">
      <img border="rounded" src="./images/blog2.png" alt="" class="w-full h-full object-cover">
      <img border="rounded" src="./images/blog3.png" alt="" class="w-full h-full object-cover">
    </v-click>
</div>
---
---

# Problems with the blog

<v-click>

- In order to update the map with my location, I had to manually make a blog post.
- Markdown seemed like a great easy way to make updates — until you have to do it on your phone


</v-click>

---
---

# How can I improve it?
<v-clicks>

- Anybody should be able to use something like my custom blog
- Making a blog post just to update the location is a bit tedious
- Friends and family being notified when a new post is made would save lots of time and energy 
- I tracked all my activities on Strava, it would be great if I could use that data to update my position on the map

</v-clicks>

---
---

# So I did improve it: pct-tracker.com

<div grid="~ cols-2 gap-8" m="t-4">
<div>

<v-clicks>


- Sends emails to friends and family when you post
- Super easy to make updates from your phone
- Anyone can set it up for their own thru-hike - no coding knowledge required, just a sign up
- Optional Strava integration for automatic location updates

</v-clicks>
</div>
<div>
</div>
</div>

---
layout: center
---

# User: Friend and family

<video src="./images/family_demo.mp4" controls muted loop class="w-full rounded shadow-lg mt-4" />

---
layout: center
---

# User: PCT hiker
<video src="./images/hiker_demo.mp4" controls muted loop class="w-full rounded shadow-lg mt-4" />

---
---

# Tech stack and challenges
<div grid="~ cols-2 gap-8" m="t-4">
<div>

**Tech stack**
- NextJS
- TailwindCSS for styling
- Supabase for storage
- Vercel for deployment
- Resend for email notifications

</div>
<div v-click>

**Challenges**
- Building a user-friendly interface for non-technical users
- Strava integration and API limitations
- Getting the distance calculations done correctly based on the location provided (from strava or the user manually)

</div>
</div>

<!-- 
    At first, syncing took forever, since I was fetching all the activities from start date to end date 
    Eventually I figured out that I actually only need the latest activity, and filtered more heavily to ensure the activity took place on the pct 

-->

---
transition: slide-up
layout: image
image: /images/start.jpg
---

# Before 

---
layout: image
image: /images/end.jpg
---

# After

---
transition: slide-up
---


