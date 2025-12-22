<script lang="ts">
  import { InstagramIcon, FacebookIcon, MailIcon } from '@lucide/svelte/icons';
  import logo from '$lib/assets/ku-logo.png';
  import img_about from '$lib/assets/about.jpg';
  import img_nordic_punch from '$lib/assets/nordic-punch.png';
  import img_roller_derby from '$lib/assets/roller-derby.jpg';
  import img_start from '$lib/assets/start.jpg';
  import img_support from '$lib/assets/support.jpg';
  import img_thanks from '$lib/assets/thanks.jpg';
  
</script>

<div class="flex flex-col">
  <!-- Page header -->
  <div class="flex flex-col gap-16 items-center white-block">
    <div class="flex gap-12">
      <img class="rounded-2xl" src={img_start} alt="Jammer skating" width="540px" />
      <div class="flex flex-col justify-between">

        <div class="flex">
          <div class="flex flex-col gap-2">
            <div class="header-style">
              Kalmar Union
            </div>
            <div class="subheader-style">
              The Nordic open-gender roller derby national team
            </div>
          </div>
          <img class="w-36 h-36" src={logo} alt="Kalmar Union logo" />
        </div>

        <div class="grid grid-cols-2 gap-x-4 gap-y-6">
          <a class="link-style" href="#about">ABOUT US</a>
          <span class="link-style-no-underline">MERCH (COMING SOON)</span>
          <a class="link-style" href="#support">SUPPORT OUR JOURNEY</a>
          <a class="link-style" href="#nordic-punch">THE PUNCH</a>
          <a class="link-style" href="#roller-derby">WHAT IS ROLLER DERBY?</a>
          <a class="link-style" href="#thanks">HELP AND SPONSORS</a>
        </div>
      </div>
    </div>
    <div class="flex gap-8">
      <a href="https://www.facebook.com/kalmarunion.nordic" target="_blank"><FacebookIcon size=36 /></a>
      <a href="https://www.instagram.com/kalmarunion.rd" target="_blank"><InstagramIcon size=36 /></a>
      <MailIcon size=36 />
    </div>
  </div>

  <!-- About us -->
  <div id="about" class="flex gap-12 gray-block">
    <div class="flex flex-col gap-10">
      <div class="header-style">
        We are the<br />Kalmar Union
      </div>
      <div class="body-style">
        <p>
          The Nordic countries have a long history as much of infighting as cooperation. With the open-gender roller derby national team Kalmar Union,
          we build the basis for a new Nordic roller derby culture.
        </p>
        <p>
          We're here to strengthen the sport across borders and inspire future generations of Nordic roller derby
          by competing under the same banner at <a href="https://worldcup.mrda.org/" target="_blank">World Cup 2026</a>.
        </p>
        <p>
          Our name stems from 1937, when Europe's first queen regent,
          <a href="https://en.wikipedia.org/wiki/Margaret_I_of_Denmark" target="_blank">Margrete</a>,
          gathered the whole Nordics under her rule. Some 500 years later we're together again!
        </p>
      </div>
    </div>
    <img class="rounded-2xl" src={img_about} alt="Oslo tryouts" width="540px" />
  </div>

  <!-- Support -->
  <div id="support" class="flex gap-12 white-block">
    <img class="rounded-2xl" src={img_support} alt="Scrimmage" width="540px" />
    <div class="flex flex-col gap-10">
      <div class="header-style">
        Support our journey!
      </div>
      <div class="body-style">
        <p>
          Want to support our journey to the World Cup or our work to build Nordic roller derby?
        </p>
        <ul>
          <li>See something cool in our webshop? Buy it!</li>
          <li>Donate via crowd funding (exclusive perks!)</li>
          <li>Volunteer at one of our events (email to check)</li>
          <li>Spread the word about our team, for instance by sharing our social media content with friends</li>
        </ul>
        <p>
          Representing a company that may have something to offer us? Email us about ideas for collaboration!
        </p>
      </div>
    </div>
  </div>

  <!-- Nordic Punch -->
  <div id="nordic-punch" class="flex gap-12 gray-block">
    <div class="flex flex-col gap-10">
      <div class="header-style">
        The great Nordic Punch
      </div>
      <div class="body-style">
        <p>
          You don't want to miss this! Four open-gender roller derby national teams meet for battle in Gothenburg 7&mdash;8 March:
          Wales Roller Derby Cymru, Power of Scotland, Team Spain and Kalmar Union
        </p>
        <p>
          The World Cup in Orléans, France in April/May 2026 will be the first in 8 years to invite all genders to the track.
          This tournament less than two months before is a great chance to get a feeling of the strength of some of the central European competitors.
          Unable to go to World Cup? Come to Gothenburg for at a taste of the action, or follow the live stream on YouTube!
        </p>
        <p>
          You can get the last updates in the Punch Facebook event
        </p>
      </div>
    </div>
    <img class="rounded-2xl" src={img_nordic_punch} alt="Nordic Punch poster" width="540px" />
  </div>

  <!-- What is Roller Derby -->
  <div id="roller-derby" class="flex gap-12 white-block">
    <img class="rounded-2xl" src={img_roller_derby} alt="Scrimmage action shot" width="540px" />
    <div class="flex flex-col gap-10">
      <div class="header-style">
        What is roller derby anyway?
      </div>
      <div class="body-style">
        <p>
          Roller derby is a contact sport on quad roller skates. Two teams play against each on an oval track for 2x30 minutes.
          Each team has five on the track at the time. One player on each team, the jammer, has a star on their helmet.
          They score points by passing the other team's blockers (i.e. the rest of the players).
        </p>
        <p>
          The sport has been a safe space for the queer community since the beginning, and it is known worldwide as an inclusive community.
          Local leagues can follow the WFTDA gender policy or be open to all (OTA, or open-gender). The rules on the track are the same.
        </p>
      </div>
    </div>
  </div>

  <!-- Thanks -->
  <div id="thanks" class="flex gap-12 gray-block">
    <div class="flex flex-col gap-10">
      <div class="header-style">
        Thank you!
      </div>
      <div class="body-style">
        <p>
          Thanks to local derby leagues for helping out, first and foremost Västsvenska Roller Derby Sällskapet, Oslo Roller and Copenhagen Ladybugs!
          Ladybugs are hosting our money, and we are very thankful for that. The national skating associations are offering support,
          financially or in other ways.
        </p>
        <p>
          Thanks to Denise Azimarev for taking all the action photos on this website!
        </p>
        <p>
          Want to sponsor us? We'll add you to this list and share on social media, get in touch to hear what we can offer!
        </p>
      </div>
    </div>
    <img class="rounded-2xl" src={img_thanks} alt="Gothenburg tryouts" width="540px" />
  </div>
</div>
