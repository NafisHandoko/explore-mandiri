<template>
  <header class="bg-center bg-cover text-white bg-[url('https://images.unsplash.com/photo-1509023464722-18d996393ca8?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1470&q=80')]">
      <div class='bg-black/50 min-h-screen'>
        <nav class='container mx-auto flex flex-col md:flex-row items-center md:justify-between w-full px-28 py-10'>
          <!-- <h3 class='font-bold text-3xl'>Mountain</h3> -->
          <VLogo white />
          <ul class='flex flex-row gap-x-7 items-center'>
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/products">Products</NuxtLink></li>
            <li><NuxtLink to="/about">About</NuxtLink></li>
          </ul>
        </nav>
        <div class='min-h-[75vh] container mx-auto w-full flex flex-col items-center justify-center gap-y-5 text-center px-10 md:px-0'>
          <h1 class='font-bold text-3xl'>The Dark Mountain</h1>
          <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Odit pariatur unde autem ex commodi facilis?</p>
          <VBtn color="primary"> Get started </VBtn>
        </div>
      </div>
    </header>
  <section class="container mx-auto p-10 flex flex-col items-center">
    <h1 class="text-xl font-bold text-center mb-4">Cards</h1>
    <div class="flex flex-row items-center gap-7">
      <VCard title="Product 1"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Ullam, minima. </VCard>
      <VCard title="Product 2"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium, magni. </VCard>
      <VCard title="Product 3"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi, temporibus? </VCard>
    </div>
  </section>
  <footer></footer>
</template>