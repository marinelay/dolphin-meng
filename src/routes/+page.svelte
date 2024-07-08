<script>
    import { Carousel } from 'flowbite-svelte';
    import images from './imageData/images.json';
    import { Heading, P, Button } from 'flowbite-svelte';
    import { ArrowRightOutline } from 'flowbite-svelte-icons';

    import { Blockquote } from 'flowbite-svelte';
    import { QuoteSolid } from 'flowbite-svelte-icons';

  </script>
  
  <div class="text-center">
    <Heading tag="h1" class="mt-8 mb-4" customSize="text-4xl font-extrabold  md:text-5xl lg:text-6xl">
        돌고래 사랑단
    </Heading>
    <P class="text-center mb-6 text-lg lg:text-xl sm:px-16 xl:px-48 dark:text-gray-400">
        우리 맹맹이 귀엽죠?
    </P>
    <!-- <Button href="/">
      Learn more
      <ArrowRightOutline class="w-6 h-6 ms-2" />
    </Button> -->
  </div>

  <div class="max-w-4xl container">
    <Carousel {images} let:Indicators let:Controls duration="3000">
        <Controls class="items-center"/>
        <Indicators />
    </Carousel>
  </div>


  <figure class="mt-8 mx-auto max-w-screen-md text-center">
    <QuoteSolid class="mx-auto mb-3 w-12 h-12 text-gray-400 dark:text-gray-600" />
    <Blockquote alignment="center" size="2xl">
        돌고래의, 돌고래에 의한, 돌고래를 위한
    </Blockquote>

  </figure>
  

<style>
    .container {
        margin: 0 auto;
    }
</style>