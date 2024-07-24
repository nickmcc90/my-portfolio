<script>
  export let y;

  let tabs = [
    {name: 'Projects', link: '#projects'},
    {name: 'About me', link: '#about'},
  ]
</script>

<header class={"sticky top-0 z-[10] duration-200 px-6 flex items-center justify-between border border-solid " + 
`${y > 0 ? ' py-4 bg-[#000080] border-[#008080]' : ' py-6 bg-transparent border-transparent'}`}>
  <h1 class='font-medium'>
    <b class='font-bold poppins'>Nicholas</b> McCarroll
  </h1>
  <div class='sm:flex items-center gap-4 hidden'>
    {#each tabs as tab, index}
      <a href={tab.link} class='duration-200 hover:text-[#ABD7EB]'>
        <p>{tab.name}</p>
      </a>
    {/each}
    <a href='https://www.linkedin.com/in/nicholas-mccarroll/'
    target='_blank'
    class='pinkShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white
  text-slate-950'>
      <div class='absolute top-0 right-full w-full h-full bg-[#008080] opacity-20
      group-hover:translate-x-full z-0 duration-200 '></div>
      <div class='flex items-center'>
        <h4 class='relative z-9'>Get in touch</h4>
        <i class="fa-brands fa-linkedin ml-2 text-xl"></i>
      </div>
    </a>
  </div>
</header>