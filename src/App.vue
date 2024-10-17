<router-link class="" to="/"></router-link> 
<router-view/>
<template>
  <div class="home">
   <div class="container bg-blue-400 justify-between font-bold max-w-full h-11 text-white text-3xl flex flex-row mt-1"> 
    <span class="ml-6" >Ifedollars</span>
    <span class="mr-6">NeedHelp?</span>
   </div>
   
   <div class="max-w-full h-[400px] bg-baddest  bg-no-repeat bg-cover bg-center text-center
    text-white shadow-lg flex flex-col items-center justify-center">
    <h1 class="text-5xl font-bold text-blue-800">Welcome to "IFEDOLLARS" Promo</h1>
    <h1 class="text-2xl pt-6 font-bold mb-4">refer your friends and family to ifedollars promo and earn rewards instantly</h1>
      <a href="" class="bg-orange-500 text-white py-3 px-6 rounded-md text-lg font-semibold hover:bg-yellow-700 mb-9">Get started</a>
   </div>
   <div class="container bg-zinc-900 h-auto max-w-full ">
    <h1 class="text-blue-800 font-bold text-4xl flex justify-center pt-10">How it works</h1> 
    <div class="grid grid-col justify-center items-center md:flex md:flex-row md:gap-24 gap-52 mt-6 text-center px-2">
      <span class=" bg-neutral-700 w-80 h-56 rounded-xl text-white flex flex-col justify-center text-xl"> <i class="fa-solid fa-user-group text-orange-600 text-5xl"></i> invite friends and family and earn $10 for each referral</span> 
      <span class=" bg-neutral-700 w-80 h-56 rounded-xl text-white text-xl flex flex-col justify-center"> <i class="fa-solid fa-pager text-orange-600 text-5xl"></i>Refer 2 people and earn $20 <br> or refer 3 people to get $25</span>
      <span class=" bg-neutral-700 w-80 h-56 rounded-xl text-white text-xl flex flex-col justify-center"> <i class="fa-solid fa-gift text-orange-600 text-5xl"></i> Get your unique referral code <br> and start sharing to win rewards</span>
    </div>
      <div class="bg-neutral-700 w-full h-auto mt-9"> 
          <h1 class=" text-2xl md:text-5xl text-blue-600 font-bold flex justify-center">Frequently Asked Questions</h1 >
            <div class="max-w-3xl mx-auto p-6">
    <!-- First Section -->
    <div class="border-b mb-4">
      <button
        @click="toggleSection(1)"
        class="flex justify-between items-center w-full py-3 text-left text-lg font-semibold text-blue-600 md:text-2xl"
      >
        What is Dexcraft?
        <span :class="isOpen === 1 ? 'rotate-180' : ''" class="transition-transform duration-200">
          ⌄
        </span>
      </button>
      <div v-if="isOpen === 1" class="py-2">
        <p class="text-gray-100">
          Dexcraft is a creative powerhouse built on the idea of designing, developing, and disrupting. It’s a company where cutting-edge design meets innovation in web development. From stunning graphics to sleek, functional websites, Dexcraft offers businesses a fresh take on how their brand should look and feel.
        </p>
        <p class="text-gray-100 mt-2">
          At its core, Dexcraft is about more than just creating websites or logos—it’s about shaking up the industry. We don't settle for ordinary. Our mission is to deliver designs that make a lasting impression and build web experiences that not only engage but set new standards.
        </p>
      </div>
    </div>

    <!-- Second Section -->
    <div class="border-b mb-4">
      <button
        @click="toggleSection(2)"
        class="flex justify-between items-center w-full py-3 text-left text-lg font-semibold text-blue-600 md:text-2xl"
      >
        How do I earn from Dexcraft?
        <span :class="isOpen === 2 ? 'rotate-180' : ''" class="transition-transform duration-200">
          ⌄
        </span>
      </button>
      <div v-if="isOpen === 2" class="py-2">
        <p class="text-gray-100">
          You can earn from Dexcraft by referring new clients, joining affiliate programs, or offering your design and development services through their platform.
        </p>
      </div>
    </div>

    <!-- Third Section -->
    <div class="border-b mb-4">
      <button
        @click="toggleSection(3)"
        class="flex justify-between items-center w-full py-3 text-left text-lg font-semibold text-blue-600 md:text-2xl"
      >
        How do I make use of the referral card?
        <span :class="isOpen === 3 ? 'rotate-180' : ''" class="transition-transform duration-200">
          ⌄
        </span>
      </button>
      <div v-if="isOpen === 3" class="py-2">
        <p class="text-gray-100">
          The referral card can be used to track your earnings by referring new clients. Simply share your referral code, and once a referral is completed, you can monitor your rewards through your Dexcraft account.
        </p>
      </div>
    </div>
  </div>
          </div>
          <div>
            <h1 class="text-4xl md:text-6xl mt-20 text-white font-bold flex justify-center px-1">Get Your referral Card</h1>
            <h1 class="mt-5 text-white text-xl md:text-3xl flex justify-center px-4">Fill out the form below to get your unique  referral card for those you refer </h1>

            <div class=".container bg-neutral-700 rounded-3xl md:w-[750px] w-[350px] h-[700px] mt-10 mx-auto">
              <h1 class="text-white text-2xl md:text-3xl pt-8 pl-5 font-bold">Full Name</h1>
              <input type="text" placeholder="Enter your Full name" class="md:w-[500px] w-[300px] md:h-20
               h-14 mt-2 ml-5 border-2 border-blue-600 rounded-xl 
               bg-neutral-700 text-white placeholder:text-white pl-5">

              <h1 class="text-white text-2xl md:text-3xl pt-8 pl-5 font-bold">Account Number</h1>
              <input type="text" placeholder="Enter your your Account Number" class="md:w-[500px] w-[300px] md:h-20 
              h-14 mt-2 ml-5 border-2 border-blue-600 rounded-xl
               bg-neutral-700 text-white placeholder:text-white pl-5">

              <h1 class="text-white text-2xl md:text-3xl pt-8 pl-5 font-bold">Bank Name</h1>
              <input type="text" placeholder="Choose" class="md:w-[500px] w-[300px] md:h-20
               h-14 mt-2 ml-5 border-2 border-blue-600 rounded-xl
               bg-neutral-700 text-white placeholder:text-white pl-5">

              <h1 class="text-white text-2xl md:text-3xl pt-8 pl-5 font-bold">Email Adress</h1>
              <input type="text" placeholder="Enter your Email" class="md:w-[500px] w-[300px] md:h-20
               h-14 mt-2 ml-5 border-2 border-blue-600 rounded-xl
               bg-neutral-700 text-white placeholder:text-white pl-5">
                <button class="text-white font-bold bg-blue-600 mt-5 w-56 md:w-96 h-11 rounded-xl ml-11 ">Submit</button>
            </div> 
            <input type="text" class="border-b-2 border-blue-600 w-full mt-5 bg-zinc-900">
            <div class="flex flex-row gap-4 justify-center">
            <i class="fa-regular fa-copyright text-white mt-5"></i>
            <h1 class="text-white mt-4">Ifedollars craft 2024. All rights reserved.</h1>
          </div>
            <div class="text-white text-2xl flex justify-center gap-11 mt-5"> 
              <i class="fa-brands fa-facebook"></i>
              <i class="fa-brands fa-twitter"></i>
              <i class="fa-brands fa-square-instagram"></i>
            </div>
          </div> 
   </div>
  </div>
</template>

<style>
.bg-baddest {
  background-image: url(https://i.pinimg.com/enabled_lo/564x/4f/78/a2/4f78a2ac80a385cc2c40e2d633439df7.jpg);
}
</style>

<script>
// @ is an alias to /src

export default {
  name: 'HomeView',
  components: {
  },
  data() {
    return {
      isOpen: null, // Track which section is open
    };
  },
  methods: {
    toggleSection(section) {
      // Toggle between opening and closing sections
      this.isOpen = this.isOpen === section ? null : section;
    },
  },
}
</script>
