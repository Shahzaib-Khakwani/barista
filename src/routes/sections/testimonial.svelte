
<script>
    // Testimonial data
    const testimonials = [
      {
        rating: 5,
        text: "Dann good coffee, rad staff, and a killer atmosphere!",
        name: "Not Dann",
        title: "Coffee Lover",
        initial: "N"
      },
      {
        rating: 5,
        text: "The best coffee on earth! I can't start my day without it.",
        name: "Mr. Nnad",
        title: "Connoisseur of Coffee",
        initial: "M"
      },
      {
        rating: 5,
        text: "Dann Good Coffee is my go-to place for a solid cup of joe.",
        name: "Petty",
        title: "Just A Guy",
        initial: "P"
      }
    ];
  
    // Function to render stars
    const renderStars = (count) => {
      return Array(count).fill('★');
    };
  </script>
  

<div class="bg-[#006764] min-h-[80vh] w-full relative p-16">
    
    <svg class='custom-shape-divider absolute -top-20 left-0' xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path fill="#FFF" fill-opacity="1" d="M0,224L80,224C160,224,320,224,480,197.3C640,171,800,117,960,101.3C1120,85,1280,107,1360,117.3L1440,128L1440,0L1360,0C1280,0,1120,0,960,0C800,0,640,0,480,0C320,0,160,0,80,0L0,0Z"></path>
    </svg>
      <section class=" py-16 px-4 w-full">
        <div class="max-w-6xl mx-auto">
          <h2 class="font-rogBold text-5xl md:text-6xl font-extrabold text-white text-center mb-4">Thrilled Customers</h2>
          
          <p class="text-white text-center text-lg mb-12">Whoa, those are some dann good reviews.</p>
          
          <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
            {#each testimonials as testimonial}
              <div class="rounded-xl border border-teal-600 p-6">
                <!-- Stars -->
                <div class="flex mb-4">
                  {#each renderStars(testimonial.rating) as star}
                    <span class="text-teal-300 text-xl">{star}</span>
                  {/each}
                </div>
                
                <!-- Testimonial text -->
                <p class="text-white text-xl font-semibold mb-8">{testimonial.text}</p>
                
                <!-- Author info -->
                <div class="flex items-center">
                  <div class="w-12 h-12 rounded-full bg-teal-600 flex items-center justify-center text-white font-medium text-lg mr-3">
                    {testimonial.initial}
                  </div>
                  <div>
                    <p class="text-white font-medium">{testimonial.name}</p>
                    <p class="text-teal-300">{testimonial.title}</p>
                  </div>
                </div>
              </div>
            {/each}
          </div>
        </div>
      </section>
    
</div>


  










<style>
.custom-shape-divider{  
   width: 100%;
   overflow: hidden;
   line-height: 0;
}
</style>