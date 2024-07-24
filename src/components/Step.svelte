<script>
  export let step;

  console.log(step.href)
</script>

<a href={step.href} target="_blank" class='p-4 sm:p-6 md:p-8
flex flex-col gap-4 rounded-lg border border-solid border-2 border-[#000080]
text-center group cursor-pointer hover:border-[#000080b2] duration-200'>
  <div class="bg-[#008080] grid place-items-center px-4 text-5xl md:text-6xl
  -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200">
    <i class={step.icon}></i>
  </div>
  <h3 class='font-medium text-xl sm:text-2xl md:text-3xl'>{step.name}</h3>
  <slot/>
  <div class='flex-1 flex justify-center gap-4 items-center'>
    Go to &rarr;
  </div>
</a>