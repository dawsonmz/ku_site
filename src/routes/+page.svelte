<script lang="ts">
  import { InstagramIcon, FacebookIcon, MailIcon } from '@lucide/svelte/icons';
  import { enhance } from '$app/forms';
  import logo from '$lib/assets/ku-logo.png';
  import img_about from '$lib/assets/about.jpg';
  import img_nordic_punch from '$lib/assets/nordic-punch.png';
  import img_roller_derby from '$lib/assets/roller-derby.jpg';
  import img_start from '$lib/assets/start.jpg';
  import img_support from '$lib/assets/support.jpg';
  import img_thanks from '$lib/assets/thanks.jpg';
  import Block from '$lib/components/block.svelte';
</script>

<div class="flex flex-col">
  <div class="block-sizing flex flex-col gap-8 md:gap-12 lg:gap-16">
    <div class="flex gap-4 md:gap-6 lg:gap-8">
      <img class="max-md:hidden image-style" src={img_start} alt="Jammer skating" />
      <div class="flex flex-col justify-between gap-6">
        <div class="flex">
          <div>
            <div class="header-style">
              Kalmar Union
            </div>
            <div class="subheader-style mt-2 lg:mt-3 xl:mt-4">
              The Nordic open-gender roller derby national team
            </div>
          </div>
          <img class="w-26 h-26 lg:w-32 lg:h-32 xl:w-36 xl:h-36" src={logo} alt="Kalmar Union logo" />
        </div>

        <div class="grid grid-cols-2 gap-2 lg:gap-4 xl:gap-5">
          <a class="link-box" href="#about">ABOUT US</a>
          <span class="link-box-no-underline">MERCH (COMING SOON)</span>
          <a class="link-box" href="#support">SUPPORT OUR JOURNEY</a>
          <a class="link-box" href="#nordic-punch">THE PUNCH</a>
          <a class="link-box" href="#roller-derby">WHAT IS ROLLER DERBY?</a>
          <a class="link-box" href="#thanks">THANKS AND SPONSORS</a>
        </div>
      </div>
    </div>
    <div class="flex self-center gap-8">
      <a href="https://www.facebook.com/kalmarunion.nordic" target="_blank"><FacebookIcon size=36 /></a>
      <a href="https://www.instagram.com/kalmarunion.rd" target="_blank"><InstagramIcon size=36 /></a>
      <a href="mailto:kalmarunionrd@gmail.com"><MailIcon size=36 /></a>
    </div>
  </div>

  <div id="newsletter" class="bg-(--primary-color)">
    <div class="newsletter-block text-(--support-color-gray) py-4">
      <form method="post" action="https://mailing.kalmarunion.eu/subscription/form" use:enhance>
        <div class="body-style mb-3">
          Join our newsletter about open-gender roller derby in the Nordics and our journey to the World Cup:
        </div>
        <div class="max-sm:grid max-sm:grid-cols-2 sm:flex gap-3 sm:max-w-60">
          <input type="hidden" name="nonce" />
          <input class="input-style" type="email" name="email" required placeholder="E-mail" />
          <input class="input-style" type="text" name="name" placeholder="Name (optional)" />
          <input id="3cdc4" type="hidden" name="l" value="3cdc4372-f6cc-45c4-92a9-1bed2f032045" />
          <input class="button-style
                        text-black
                        bg-(--secondary-color)
                        hover:bg-(--support-color-blue)
                        hover:text-(--support-color-gray)
                        active:bg-(--support-color-blue)
                        active:text-(--support-color-gray)
                        sm:ml-3"
                 type="submit"
                 value="SUBSCRIBE" />
        </div>
      </form>
    </div>
  </div>

  <Block id="about" img={img_about} img_alt_text="Oslo tryouts">
    {#snippet heading()}
      We are the<br />Kalmar Union
    {/snippet}
    {#snippet body()}
      <p>
        We're here to strengthen Nordic roller derby across borders and inspire future generations of our sport by competing under the same banner
        at the <a class="link" href="https://worldcup.mrda.org" target="_blank">World Cup</a>!
      </p>
      <p>
        The Nordic countries have a long history as much of infighting as cooperation. With the open-gender roller derby national team Kalmar Union,
        we build the basis for a new Nordic roller derby culture.
      </p>
      <p>
        Our name stems from 1397, when Europe's first queen regent,
        <a class="link" href="https://en.wikipedia.org/wiki/Margaret_I_of_Denmark" target="_blank">Margrete (or Margaret) I</a>,
        gathered the Nordic countries under her rule. Some 500 years later we're together again!
      </p>
    {/snippet}
  </Block>

  <Block id="support" img_left={true} img={img_support} img_alt_text="Oslo scrimmage">
    {#snippet heading()}
      Support our journey!
    {/snippet}
    {#snippet body()}
      <p>
        Want to support our journey to the World Cup and our work to build Nordic open-gender roller derby stronger?
      </p>
      <ul>
        <li>
          <a class="link" href="#newsletter">Sign up for our newsletter</a> to stay in touch
        </li>
        <li>
          Buy our merch (coming soon!)
        </li>
        <li>
          <a class="link" href="mailto:kalmarunionrd@gmail.com">Email us</a> about ways to volunteer or contribute
        </li>
        <li>
          Spread the word about our team by sharing our content on
          <a class="link" href="https://www.facebook.com/kalmarunion.nordic" target="_blank">Facebook</a> or
          <a class="link" href="https://www.instagram.com/kalmarunion.rd" target="_blank">Instagram</a>
        </li>
        <li>
          Represent a company that may have something to offer?
          <a class="link" href="mailto:kalmarunionrd@gmail.com">Email us</a> about ideas for collaboration!
        </li>
      </ul>
    {/snippet}
  </Block>

  <Block id="nordic-punch" img={img_nordic_punch} img_alt_text="Nordic Punch poster">
    {#snippet heading()}
      The great Nordic Punch
    {/snippet}
    {#snippet body()}
      <p>
        Four open-gender roller derby national teams meet for battle in
        <a class="link" href="https://www.facebook.com/share/17AAQ51Fzq" target="_blank">Gothenburg 7&mdash;8 March 2026</a>:
        Wales Roller Derby Cymru, Power of Scotland, Team Spain and Kalmar Union
      </p>
      <p>
        The <a class="link" href="https://worldcup.mrda.org" target="_blank">World Cup in Orléans, France in May 2026</a> will be the first in 8 years
        to invite all genders to the track. This tournament less than two months before is a great chance to get a feeling of the strength
        of some of the central European competitors. Unable to go to World Cup? Come to Gothenburg for at a taste of the action,
        or follow the live stream on YouTube!
      </p>
      <p>
        You can get the last updates in the
        <a class="link" href="https://www.facebook.com/share/17AAQ51Fzq" target="_blank">Punch Facebook event</a>.
      </p>
    {/snippet}
  </Block>

  <Block id="roller-derby" img_left={true} img={img_roller_derby} img_alt_text="Oslo scrimmage action shot">
    {#snippet heading()}
      What is roller derby anyway?
    {/snippet}
    {#snippet body()}
      <p>
        Roller derby is a contact sport on quad roller skates. Two teams play against each on an oval track for 2x30 minutes, split into jams of
        up to 2 minutes. Each team fields five players, one of whom has a star on their helmet (the jammer). They score points by passing the four
        remaining players on the other team (blockers).
      </p>
      <p>
        The sport has been a safe space for the queer community since the beginning, and it is known worldwide as an inclusive community.
        Local leagues can follow the
        <a class="link" href="https://resources.wftda.org/membership/diversity-and-inclusion/wftda-statement-about-gender" target="_blank">gender statement</a>
        of the <a class="link" href="https://wftda.com" target="_blank">Women's Flat Track Derby Association</a> or be open-gender/open to all like the
        Men's Roller Derby Association. The rules are the same.
      </p>
    {/snippet}
  </Block>

  <Block id="thanks" img={img_thanks} img_alt_text="Gothenburg tryouts">
    {#snippet heading()}
      Thank you!
    {/snippet}
    {#snippet body()}
      <p>
        Thanks to local derby leagues for helping us, especially to Västsvenska Roller Derby Sällskapet, Oslo Roller Derby and Copenhagen Ladybugs
        for hosting our events! The Ladybugs also look after our money. The national skating associations have offered support, financially or
        in other ways.
      </p>
      <p>
        Thanks to Denise Azimarev for taking the action photos on this website!
      </p>
      <p>
        Want to sponsor us? We can offer visibility on this site, in social media and in other ways.
        <a class="link" href="mailto:kalmarunionrd@gmail.com">Get in touch to hear more</a>!
      </p>
    {/snippet}
  </Block>

  <div class="bg-(--support-color-blue)">
    <div class="flex flex-col gap-4 newsletter-block text-(--support-color-gray)">
      <div class="subheader-style">
        Get updates!
      </div>
      <form method="post" action="https://mailing.kalmarunion.eu/subscription/form" use:enhance>
        <div class="body-style mb-3">
          Join our newsletter about open-gender roller derby in the Nordics and our journey to the World Cup:
        </div>
        <div class="max-sm:grid max-sm:grid-cols-2 sm:flex gap-3 sm:max-w-60">
          <input type="hidden" name="nonce" />
          <input class="input-style" type="email" name="email" required placeholder="E-mail" />
          <input class="input-style" type="text" name="name" placeholder="Name (optional)" />
          <input id="3cdc4" type="hidden" name="l" value="3cdc4372-f6cc-45c4-92a9-1bed2f032045" />
          <input class="button-style
                        text-(--support-color-gray)
                        bg-(--support-color-red)
                        hover:bg-(--secondary-color)
                        hover:text-(--support-color-dark-gray)
                        active:bg-(--secondary-color)
                        active:text-(--support-color-dark-gray)
                        sm:ml-3"
                 type="submit"
                 value="SUBSCRIBE" />
        </div>
      </form>
      <div class="body-style">
        © KALMAR UNION 2026
      </div>
    </div>
  </div>
</div>
