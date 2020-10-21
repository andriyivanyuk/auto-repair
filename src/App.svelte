<script>
  import Backdrop from "./components/Backdrop.svelte";
  import Header from "./components/header.svelte";
  import AboutUs from "./components/aboutUs.svelte";
  import Carousel from "./components/Carousel.svelte";
  import Services from "./components/services.svelte";
  import Appointment from "./components/appointment.svelte";
  import Footer from "./components/footer.svelte";

  let backdrop;

  const images = [
    {
      path: "/assets/img/carousel/1.jpg",
      id: "image-one",
    },
    {
      path: "/assets/img/carousel/2.jpg",
      id: "image-two",
    },
    {
      path: "/assets/img/carousel/3.jpg",
      id: "image-three",
    },
    {
      path: "/assets/img/carousel/4.jpg",
      id: "image-four",
    },
    {
      path: "/assets/img/carousel/5.jpg",
      id: "image-five",
    }
  ];
  const handleBackdropData = (e) => {
    backdrop = e.detail;
  }
</script>

<style>
</style>

<Backdrop on:backdrop={handleBackdropData}/>
<Header
  {backdrop}/>
<AboutUs />
<Carousel 
   imageWidth={350}
   imageSpacing={10}
  {images}>
</Carousel>
<Services />
<Appointment />
<Footer />
