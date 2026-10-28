KAASHII — VISIBLE MESSAGE COLOURS (CH 3 + 4)  +  DARK PATCHES ON THE BACKGROUND

Nothing was removed or changed anywhere else: fonts, layout, text, buttons, navigation, animations, music are as before.

1) MESSAGE BOX COLOURS (chapter 3 moods + chapter 4 gifts)
   Every message box has the same style: tinted fill + coloured border + glow, one colour per option.
   Chapter 3 : Dil heavy hai -> aqua blue | Bahut thak gayi hoon -> amber | Akela feel ho raha hai -> mint | Kuch cute chahiye -> pink
   Chapter 4 : Kind words -> pink | Biryani break -> saffron | Purple & green -> violet-to-green | Ghumne ka mood -> teal
               Soft day -> golden yellow | Care note -> pink | Cute cats -> lime | Sirf Aapka Raaz -> sky blue
   To change a colour: edit the r,g,b numbers in the "--tc" lines in the CSS block "VISIBLE MESSAGE BOX COLOURS".

2) BACKGROUND DARK PATCHES (new, v4 - stronger so they really show on a phone)
   A few soft patches of deep indigo-navy (rgb 24,8,92), with clear gaps of lighter sky between them:
   left (middle) | right (middle) | a light one in the centre | left (lower) | right (bottom).
   The top is untouched (already dark). No continuous border band.
   They sit on the sky photo but UNDER the stars, petals, hearts and the card.
   Added: one CSS block "BACKGROUND ONLY" at the end of <style>, and one line <div class="sky-shade"></div> right after <body>.
   Each "radial-gradient(ellipse WIDTH HEIGHT at X Y, ...)" line is one patch (all in % of the screen):
   first alpha number = strength (higher = darker), WIDTH/HEIGHT = size, X Y = position. Delete a line to remove that patch.

IF IT LOOKS UNCHANGED AFTER UPLOADING: GitHub Pages / the phone browser can keep showing the old file for a few minutes.
Open the site with ?v=4 added at the end of the link, or clear this site's data in Chrome, then check again.

Replace the repository index.html with this index.html. Keep purple-sky.jpg and music.mp3 in the repository root.
