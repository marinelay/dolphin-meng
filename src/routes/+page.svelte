<script>
    import { Carousel } from 'flowbite-svelte';
    import images from './imageData/images.json';
  </script>
  
  <div class="max-w-4xl">
    <Carousel {images} let:Indicators let:Controls duration="3000">
        <Controls />
        <Indicators />
    </Carousel>
  </div>