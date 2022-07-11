---
layout: default
title: Home
---

## Welcome to my fundraising page

Hello! I'm Noah and I'm 6 years old.

I am raising money for my school <a href="https://www.birkenshawprimary.org.uk/" target="_blank">Birkenshaw C.E. (C) Primary School</a> to support the funding of the annual leasing of the minibus. The minibus has been a fabulous addition to school and benefited children across all year groups. 

The minibus costs school £5000.00 each school year and I, amongst other children in school are raising a small amount money each with the hope that it collectively contributes towards a larger amount to keep the minibus going for our next school year.

Our school have set the **2022 Challenge** which within the last month before the end of the school year they are encouraging the children to raise **at least £20.22**!

It would be awesome if you could help me & the school reach our targets by donating any little amount you can afford, whether that be 20p, 50p, £1 or more!

Thank you for visiting and look forward to drawing your idea.

### How am I going to raise the money?
After I have received your sponsorship and donation I will attempt to draw a picture of your choosing & post it on my website for the world to see. My favourite things to draw at the moment are Sonic The Hedgehog, Numberblocks & The Solar System. But I am up for a challenge, so please don't let these things limit your choices of things for me to draw.

### How can you sponsor me?
1. Complete the <a href="/schoolbus/sponsor">sponsorship form</a> with your Name, Address (for GiftAid) and your picture request.
2. Send your donation to my Dads <a href="https://paypal.me/andyboot" target="_blank">PayPal.me page</a>.
3. I will draw & upload your requested picture and post here along with your name.

### THANK YOU
Noah would like to thank everybody who donated, got involved and helped exceed the target which his school had set.
<img src="https://noah-boot.github.io/schoolbus/assets/images/posts/Scan%20-%202022-07-11%2019_49_29.jpeg" />

### Gallery

{% if site.posts and site.posts.size != 0 %}

<!-- Posts Index
================================================== -->
<section class="recent-posts">

    <div class="row listrecent">

        {% for post in site.posts %}

        {% include postbox.html %}

        {% endfor %}

    </div>

</section>

{% else %}

No pictures just yet, check again later. Or, why not be my first sponsor!?

{% endif %}
