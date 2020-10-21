<script>
  import { flip } from "svelte/animate";

  export let images;
  export let imageWidth = 300;
  export let imageSpacing = 15;
  export let speed = 500;

  const rotateLeft = () => {
    const transitioningImage = images[images.length - 1];
    document.getElementById(transitioningImage.id).style.opacity = 0;
    images = [images[images.length - 1], ...images.slice(0, images.length - 1)];
    setTimeout(() => {
      document.getElementById(transitioningImage.id).style.opacity = 1;
    }, speed);
  };
  const rotateRight = () => {
    const transitioningImage = images[0];
    document.getElementById(transitioningImage.id).style.opacity = 0;
    images = [...images.slice(1, images.length), images[0]];
    setTimeout(() => {
      document.getElementById(transitioningImage.id).style.opacity = 1;
    }, speed);
  };
</script>

<style>
  .carousel__shell {
    background-color: #f5f5f5;
    padding: 100px 0;
  }
  .carousel-container {
    width: 100%;
    overflow-x: hidden;
    position: relative;
  }
  .carousel-images {
    display: flex;
    flex-wrap: nowrap;
    justify-content: center;
    align-items: center;
  }
  .carousel-left,
  .carousel-right {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    border: none;
    outline: none;
    padding: 15px 12px;
    background-color: rgba(249, 249, 249, 0.95);
  }
  .carousel-right {
    right: 2px;
  }
  .carousel-left {
    left: 2px;
  }
</style>

<section class="carousel__shell">
  <div class="carousel-container">
    <div class="carousel-images">
      {#each images as image (image.id)}
        <img
          src={image.path}
          alt={image.id}
          id={image.id}
          style="width:{imageWidth}px; margin: 0 {imageSpacing}px;"
          animate:flip={{ duration: speed }} />
      {/each}
    </div>
    <button on:click={rotateLeft} class="carousel-left">
      <slot name="left-control">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg">
          <g id="arrow_back_ios_24px">
            <path
              id="icon/navigation/arrow_back_ios_24px"
              d="M17.835 3.87L16.055 2.1L6.16504 12L16.065 21.9L17.835 20.13L9.70504 12L17.835 3.87Z"
              fill="#454545" />
          </g>
        </svg>
      </slot>
    </button>
    <button on:click={rotateRight} class="carousel-right">
      <slot name="right-control">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg">
          <g id="arrow_forward_ios_24px">
            <path
              id="icon/navigation/arrow_forward_ios_24px"
              d="M6.16504 20.13L7.93504 21.9L17.835 12L7.93504 2.1L6.16504 3.87L14.295 12L6.16504 20.13H6.16504Z"
              fill="#454545" />
          </g>
        </svg>
      </slot>
    </button>
  </div>
</section>
