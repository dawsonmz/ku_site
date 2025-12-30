<script lang="ts">
  let { id=null, img_left=false, img, img_alt_text, heading, body } = $props();
</script>

<div {id} class="{img_left ? 'bg-white' : 'bg-(--support-color-gray)'}">
  <div class="block-sizing">
    <div class="flex gap-4 lg:gap-6 xl:gap-8">
      {#if img_left}
        <img class="max-md:hidden image-style" src={img} alt={img_alt_text} />
      {/if}
      <div class="max-md:flex max-md:flex-col max-md:gap-6">
        <div class="header-style">
          {@render heading()}
        </div>
        <img class="md:hidden rounded-2xl w-fit" src={img} alt={img_alt_text} />
        <div class="body-style md:mt-9">
          {@render body()}
        </div>
      </div>
      {#if !img_left}
        <img class="max-md:hidden image-style" src={img} alt={img_alt_text} />
      {/if}
    </div>
  </div>
</div>
